# 03 · Regras de Transações Suspeitas

<!-- Inserir imagem do diagrama aqui -->
![Regras de Transações Suspeitas](diagrama-03-transacoes-suspeitas.jpg)

---

## Ponto de entrada

Este fluxo é executado antes do motor de regras principal. Recebe as transações coletadas do caso e aplica o filtro `SUSPEITA` para decidir se o caso segue automático ou vai para humano.

---

## Etapa 1 · Filtro SUSPEITA

O robô filtra as transações pela marcação `SUSPEITA`.

- **Nenhuma transação suspeita encontrada →** encaminha para **humano**. Encerra.

---

## Etapa 2 · Suspeita é do dia de hoje?

- **Não → suspeitas antigas** — não geram ação automática. O caso segue para o motor de regras normalmente.

---

## Etapa 3 · Quantas suspeitas hoje?

| Quantidade | Comportamento |
|---|---|
| 1 a 3 suspeitas | Casos do dia — segue para mensageria automática |
| Mais de 3 suspeitas | Entra na avaliação de exceção |

---

## Etapa 4 · Avaliação de exceção (mais de 3 suspeitas)

O robô verifica os 3 critérios abaixo em conjunto:

| Critério | Verificação |
|---|---|
| Mesmo estabelecimento? | Todas as suspeitas no mesmo CNPJ/nome |
| Valores idênticos? | Montantes iguais entre as transações |
| Horários consecutivos < 5 min? | Intervalo menor que 5 minutos entre elas |

- **3 critérios atendidos →** exceção válida. Trata **todas** as suspeitas como um único evento e segue para mensageria automática.
- **Critérios não atendidos →** **humano — risco alto**. Encerra.

---

## Saídas do fluxo

| Saída | Condição |
|---|---|
| **Humano** | Nenhuma suspeita encontrada |
| **Humano — risco alto** | Mais de 3 suspeitas sem exceção válida |
| **Segue mensageria automática** | 1–3 suspeitas hoje, ou exceção válida confirmada |
| **Segue motor de regras** | Apenas suspeitas antigas (sem suspeita do dia) |
