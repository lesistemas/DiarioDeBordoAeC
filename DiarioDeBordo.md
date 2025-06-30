# 📘 Diario de Bordo – Squad Nexus · AeC

Registro contínuo e estruturado das atividades técnicas realizadas, com foco em contexto, impacto e rastreabilidade.

---
## 🗓️ **30/06**

###  Resumo de Horas do Dia

| Tarefa                                                                 | Tempo |
|------------------------------------------------------------------------|--------|
| 🔧 CNU – Atualização do ChromeDriver - Acompanhamento Release                                  | 02:00 |
| 🚫 Impedimento – Sem Demanda                                           | 03:00 |
| 🚫 Impedimento – Sistema do Cliente IbiPlus (Necessidade de Login)     | 01:00 |
| 🔧 [INCIDENTE NEG.] Mesa de Decisão SAC – Análise inicial do problema | 02:00 |

### 🔧 CNU – Atualização do ChromeDriver 
- **Tarefa:** Acompanhamento da subida da nova versão, após os testes, liberação para produção via Pull Request com acompanhamento técnico.
- **Tempo gasto:** 2h  
- **Resumo anterior:** Atualização do ChromeDriver e testes no robô Blip realizados em 27/06.
- **Status:** Finalizado  

---


### 🔧 Bradesco – PR de Produção IbiPlus (Calculadora)
- **Tarefa:** Criação e aprovação do Pull Request para produção, após confirmação de homologação.  
- **Resumo anterior:** O PR já estava pronto desde quarta-feira às 10h, aguardando a aprovação da homologação por parte da Ana.  
- **Execução:**  
  - Ana solicitou formalmente a PR pela manhã, porém já tinha passado dresde quarta.  
  - No final do dia, após às 17:30h, o PR foi aprovado e iniciou-se a release.  
  - Durante o processo, a esteira apresentou erro.  
- **Status:** Em análise – erro técnico na esteira identificado.  
- **Impacto:** A liberação para produção foi iniciada, mas está pendente de correção técnica. A falha será investigada para permitir a conclusão da entrega.


---
### 🔧 Bradesco – [INCIDENTE NEG.] Mesa de Decisão SAC – Validação do Campo Telefônico
- **Tarefa:** Configuração inicial do projeto para verificar o incidente e relacionado ao campo de telefone no formulário da Mesa de Decisão do SAC.  
- **Descrição:** O formulário estava permitindo avanço mesmo com números inválidos. A tarefa envolve bloquear o prosseguimento do formulário caso o telefone informado não tenha exatamente 11 dígitos válidos.  
- **Ações realizadas:**  
  - Ajustes no projeto para garantir que o fluxo chegue até o formulário da Mesa.  
  - Solicitação e uso de nova senha para acesso ao ambiente IbiPlus.  
  - Acesso técnico validado com sucesso até o formulário final.  
- **Próximo passo:** Início da lógica de bloqueio e validação do campo a partir de amanhã.  
- **Tempo gasto hoje:** 2h  
- **Status:** 🔄 Em andamento – fase de configuração inicial concluída.
---

### 🚫 Impedimento Sem Demanda
- **Tarefa:** Sem demanda entre 11h e 15h. aguardei um pouco para abrir pois estava achando q arrumaria a tarefa rápido, ate 12:30 mais ou menos
-**Tempo Registro:** 3h.   
- **Observação:** Disponibilidade registrada e validada com o time.---

### 🚫 Impedimento Técnico ou Operacional
- **Tarefa:** Sem login e senha ibiplus
-**Tempo Registro:** 1h.   

## 📊 **Resumo da Semana (22/06 - 27/06)**

| Item                             | Quantidade |
|----------------------------------|------------|

---

## 🗓️ **27/06**

### 🔧 CNU – Ajustes ChromeDriver
- **Tarefa:** Validação prévia de compatibilidade local antes da subida final do PR.  
- **Tempo gasto:** 1h  
- **Status:** ✅ Concluído  
- **Impacto:** Garantiu que a atualização não geraria regressões em outras automações do robô.

---
