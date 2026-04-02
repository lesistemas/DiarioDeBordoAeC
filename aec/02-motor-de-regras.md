# 02 · Motor de Regras Detalhado

<!-- Inserir imagem do diagrama aqui -->
![Motor de Regras Detalhado](diagrama-02-motor-de-regras.jpg)

---

## Ponto de entrada

O motor recebe os dados já coletados do Case Manager e do PW e executa as regras em **ordem fixa**. A ordem importa: uma regra encerrada antes impede a execução das seguintes.

---

## Ordem de execução

### 1 · Não passível / Bloqueado / Bypass

Compara o `blockCode` retornado pelo PW com a lista de códigos não passíveis carregada do AutomationRoom. Também verifica se o cartão está bloqueado ou se o bypass está ativo há menos de 2 dias.

- **Se cair aqui →** tenta salvar descarte no Case Manager. Se não conseguir, desvia para humano. **Encerra.**

---

### 2 · Fila exige humano

Verifica o parâmetro `filaRegra.ExigeHumano` da fila coletada.

- **Se ativo →** encaminha para tratativa humana. **Encerra.**

---

### 3 · Regra de suspeitos exige humano?

Lê o resultado de `analiseCartao.TransacoesNaRegraSuspeitos`.

- **Se `HouveErro = true` ou `SegueTratativaHumano = true` →** encaminha para humano. **Encerra.**

---

### 4 · Cliente tem telefone válido?

Verifica se o PW retornou telefone.

- **Se ausente →** aplica a política `RegraSemTelefone` da fila: pode ir para humano ou salvar resposta específica no Case Manager. **Encerra.**

---

### 5 · Mesa de Decisão

Consulta obrigatória apenas quando:
- cadastro foi criado há menos de 2 meses, **ou**
- houve alteração cadastral há menos de 2 meses.

Valida se o telefone do alerta é confiável para aquele CPF.

- **Se reprovado →** encaminha para humano. **Encerra.**

---

### 6 · Lista negativa — Redis

Consulta se o telefone está na lista negativa. A lista é alimentada por outro robô que busca da Mesa de Decisão periodicamente e disponibiliza via Redis.

- **Se bloqueado →** encaminha para humano. **Encerra.**

---

### 7 · Preventivo P

Se `BloqueioPreventivoP == NoInicio` na regra da fila, aplica o bloqueio P no PW antes de salvar o cartão.

---

### 8 · Salvar cartão — Case Manager

Registra a resposta do cartão no Case Manager.

Resultados possíveis:

| Resultado | Consequência |
|---|---|
| Sucesso | Segue para mailing e RabbitMQ |
| Outro analista | Encerra sem publicar |
| Transações já modificadas | Encerra sem publicar |
| Falha genérica | Desvia para humano |

---

### 9 · Disparo de mailing — Gateway

Registra o disparo do tipo mailing no Gateway junto ao log do caso.

---

### 10 · Publicar RabbitMQ

Publica o payload operacional. **Fim do caso.**
