# 01 · Fluxo Completo

<!-- Inserir imagem do diagrama aqui -->
![Fluxo Completo](diagrama-01-fluxo-completo.jpg)

---

## Inicialização

O robô carrega os parâmetros do **AutomationRoom** antes de entrar em execução: credenciais do Case Manager e do PW, chave Redis, endpoints da Mesa de Decisão, filas priorizadas com suas regras e parâmetros de RabbitMQ.

---

## Loop principal

O robô entra em loop contínuo. Em cada iteração:

1. **Busca caso no Case Manager** — se não houver caso disponível, volta ao início do loop.
2. **Coleta dados do caso** — identifica o `IdCaso` e as últimas 4 do cartão.
3. **Consulta o PW** — obtém dados do cliente, block code, status do cartão e datas cadastrais. Se falhar, encaminha para tratativa humana e retorna ao loop.
4. **Aplica regra de transações suspeitas** — analisa as transações antes do motor de regras principal.
5. **Executa o motor de regras** — em ordem fixa, decide o destino do caso.

---

## Saídas possíveis do motor de regras

| Saída | O que acontece |
|---|---|
| **Descarte** | Tenta salvar descarte no Case Manager; se falhar, desvia para humano |
| **Tratativa humana** | Registra caso no Gateway, dispara tratativa humana, publica no RabbitMQ |
| **Continuar automático** | Segue para validação de telefone |

---

## Finalização automática

Quando o caso segue o caminho automático:

1. Valida telefone via **Mesa de Decisão** (se cadastro ou alteração cadastral for recente)
2. Consulta **lista negativa** no Redis
3. Aplica **bloqueio preventivo P** no PW, se a fila exigir
4. Salva cartão no **Case Manager**
5. Registra logs no **Gateway**
6. Gera registro de **mailing**
7. Publica evento no **RabbitMQ**
8. Encerra o caso e retorna ao loop
