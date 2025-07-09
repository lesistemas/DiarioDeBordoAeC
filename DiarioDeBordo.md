# 📘 Diario de Bordo – Squad Nexus · AeC

Registro contínuo e estruturado das atividades técnicas realizadas.

---
## 🗓️ **08/07**

###  Resumo de Horas do Dia
<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#ffffff; color:#000000">
      <td>08/07</td>
      <td>07:00</td>
      <td>Configuração de ambiente, instalação do Miracle e acesso aos sistemas TIM X / Siebel</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>08/07</td>
      <td>01:00</td>
      <td>Subida para Produção – PR dos projetos MESA DE DECISÃO e FRONT DE CONTESTAÇÃO</td>
    </tr>
  </tbody>
</table>

---

### 🛠️ Configuração de ambiente, instalação do Miracle e acesso aos sistemas TIM X / Siebel
- **Tarefa:** Preparo do ambiente e apoio para acesso a sistemas utilizados na TIM.
- **Resumo:**  
  - Acesso às VMs foi normalizado no início do dia.
  - Necessidade de instalar o Miracle dentro da VM para operar certos acessos.
  - Link para instalação fornecido por Letícia.
  - Danilo disponibilizou links diretos para os sistemas **TIM X** e **Siebel**, evitando uso do Miracle em alguns casos.
  - Configuradas as máquinas com login/senha.
  - Acesso ao **Siebel** confirmado; **TIM X** ainda com falhas de autenticação.
- **Tempo gasto:** 7h

---

### 🚀 Subida para Produção – PR dos projetos MESA DE DECISÃO e FRONT DE CONTESTAÇÃO
- **Tarefa:** Geração das PRs de produção para dois projetos com mudanças aprovadas.
- **Resumo:**  
  - Solicitação recebida para gerar as PRs e agendar subida após HMUD.
  - Projetos:
    - **Epic 290682**: [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPOS TELEFÔNICOS
    - **Epic 306779**: [INCIDENTE] FRONT DE CONTESTAÇÃO – API E-MAIL
  - PRs criadas e prontas para o deploy.
- **Tempo gasto:** 1h

## 🗓️ **07/07**

###  Resumo de Horas do Dia
<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#ffffff; color:#000000">
      <td>07/07</td>
      <td>01:00</td>
      <td>[REUNIÃO] Alinhamento inicial da demanda – Contestação TIM (Letícia + Time)</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>07/07</td>
      <td>03:00</td>
      <td style="color:#ff0000">Impedimento – Sem Demanda</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>07/07</td>
      <td>04:00</td>
      <td style="color:#ff0000">Impedimento – Sem Acesso às VMs da TIM</td>
    </tr>
  </tbody>
</table>

---

### 🧠 [REUNIÃO] Alinhamento inicial da demanda – Contestação TIM (Letícia + Time)
- **Tarefa:** Participação em reunião com Letícia e o time para compreender os pontos iniciais da nova demanda de contestação automática para a TIM.
- **Resumo:**  
  - Foram levantados os pontos-chave da contestação automática.
  - Alinhamento da proposta inicial do robô e definições das **duas POCs viáveis** discutidas com base nas informações do cliente:
    - **POC 1:** Análise e extração via planilha + upload manual via Portal TIM.
    - **POC 2:** Automação de leitura de PDF com regras fixas + envio automatizado via API (a depender da validação de viabilidade).
  - Discussão sobre as restrições técnicas de acesso ao ambiente da TIM e limitações iniciais.
- **Resultado:** Criado plano inicial para execução das duas POCs. Aguardar acesso e permissões.
- **Tempo gasto:** 1h

---

### 🚫 Impedimento – Sem Demanda
- **Tarefa:** Ausência total de novas demandas úteis para atuação técnica ao longo da manhã.
- **Tempo Registro:** 3h  
- **Observação:** Aguardando movimentação ou liberação de tarefas em backlog.

---

### 🚫 Impedimento – Sem Acesso às VMs da TIM
- **Tarefa:** Tentativa de acesso às máquinas virtuais para preparação das POCs da contestação TIM, sem sucesso.
- **Descrição:** Todas as tentativas resultaram em falha de autenticação ou erro de rede.
- **Impacto:** Impedimento direto na continuação da tarefa prática para as provas de conceito.
- **Tempo Registro:** 4h  
- **Observação:** Acesso ainda em tratativa com time técnico responsável.


---
### 📊 **Resumo da Semana (30/06 - 04/07)**

<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>02:00</td>
      <td>CNU – Atualização do ChromeDriver – Acompanhamento Release</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>03:00</td>
      <td style="color:#ff0000">Impedimento – Sem Demanda</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>01:00</td>
      <td>Impedimento – Sistema do Cliente IbiPlus (Necessidade de Login)</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>02:00</td>
      <td>Bradesco – [INCIDENTE NEG.] Mesa de Decisão SAC – Análise inicial do problema</td>
    </tr>
    <tr style="background-color:#f0f0f0; color:#000000">
      <td>01/07</td>
      <td>08:00</td>
      <td>Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – lógica de bloqueio implementada</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>02/07</td>
      <td>08:00</td>
      <td>Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – validação funcional e encaminhamento para homologação</td>
    </tr>
    <tr><td>03/07</td><td>04:00</td><td>Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – publicação e início do release</td></tr>
<tr><td>03/07</td><td>04:00</td><td class="impedimento">Impedimento – Sem Demanda</td></tr>

  </tbody>
</table>

## 🗓️ **04/07**

###  Resumo de Horas do Dia
<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#f0f0f0; color:#000000">
      <td>04/07</td>
      <td>08:00</td>
      <td>Bradesco – [INCIDENTE] FRONT DE CONTESTAÇÃO – API E-MAIL</td>
    </tr>
  </tbody>
</table>

### 🔧 Bradesco – [INCIDENTE] FRONT DE CONTESTAÇÃO – API E-MAIL
- **Tarefa:** Correção do envio de e-mails no sistema **bradescard.Contestacao.API**, utilizando nova API para autenticação e disparo.
- **Tempo gasto:** 8h
- **Resumo do dia (04/07):**
  - Recebida demanda para tratar falha no envio de e-mails ao submeter formulário no **FRONT de Contestação**.
  - Analisado o fluxo da aplicação e validada a necessidade de troca do e-mail do remetente.
  - Com orientação do Danilo, foi realizada alteração no código da API, adicionando o novo remetente e integrando com o sistema de autenticação por token.
  - Como era o primeiro uso da **API de e-mail**, foi necessário ajustar permissões e credenciais, garantindo acesso ao token.
  - Nos testes, foi necessário utilizar o e-mail do Danilo, pois o acesso com meu e-mail apresentou falha de navegador.
  - Após validações e correções, o código foi enviado para **homologação**, ficando disponível para os **testes dos clientes**.
  - Testes via Postman foram realizados com sucesso usando a URL da API de envio de e-mail e autenticação com senha de rede (`password`).

- **Demanda vinculada:**  
  - **User Story 306780** – [INCIDENTE] FRONT DE CONTESTAÇÃO – API E-MAIL  
  - **Epic 306779** – [INCIDENTE] FRONT DE CONTESTAÇÃO – API E-MAIL


## 🗓️ **03/07**

###  Resumo de Horas do Dia
<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#f0f0f0; color:#000000">
      <td>03/07</td>
      <td>04:00</td>
      <td>Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – publicação e início do release</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>03/07</td>
      <td>04:00</td>
      <td style="color:#ff0000">Impedimento – Sem Demanda</td>
    </tr>
  </tbody>
</table>

### 🔧 Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – **publicação e início do release**
- **Tarefa:** Finalização dos testes e correção da ausência de versão para publicação em homologação. Liberação da versão aprovada e início do release.  
- **Tempo gasto:** 4h  
- **Resumo do dia (03/07):**  
  - Corrigida a pendência da versão ausente nos arquivos.  
  - Realizados testes com as versões existentes até homologação.  
  - Publicação realizada e aceita com sucesso.  
  - Início do processo de release, que passou completamente sem falhas.  
  - Status comunicado para a PO, que irá encaminhar para validação dos clientes.  
- **Próximos passos:** Aguardar retorno da PO e dos clientes sobre a validação da entrega.

---

### 🚫 Impedimento Sem Demanda
- **Tarefa:** Sem novas demandas após finalização da entrega, entre 13h e 17h.  
- **Tempo Registro:** 4h  
- **Observação:** Disponibilidade registrada e validada com o time. Aguardando nova atribuição.

## 🗓️ **02/07**
<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#ffffff; color:#000000">
      <td>02/07</td>
      <td>08:00</td>
      <td>Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – validação funcional e encaminhamento para homologação</td>
    </tr>
  </tbody>
</table>


### 🔍 Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – **validação funcional e encaminhamento para homologação**
- **Tarefa:** Testes gerais e validação da funcionalidade com a PO, além do processo de publicação para homologação.  
- **Tempo gasto:** 8h  
- **Resumo do dia (02/07):**  
  - Realizados testes locais para verificar o impacto da nova lógica implementada.  
  - Foi apresentado um vídeo demonstrativo à PO Letícia, que **aprovou a validação funcional**.  
  - Iniciado o processo de criação das branches para publicação da versão em ambiente de homologação.  
  - Durante a tentativa de subir as branches na máquina do cliente, foi identificado um problema de acesso.  
  - O analista Danilo interveio e **liberou o acesso necessário** para continuidade.  
- **Próximos passos:**  
  - Testar a versão publicada no ambiente de homologação.  
  - A PO Letícia irá validar diretamente com os clientes o comportamento final do sistema.


---
## 🗓️ **01/07**

###  Resumo de Horas do Dia
<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#f0f0f0; color:#000000">
      <td>01/07</td>
      <td>08:00</td>
      <td>Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – lógica de bloqueio implementada</td>
    </tr>
  </tbody>
</table>


### 🔧 Bradesco – [INCIDENTE NEG.] MESA DE DECISÃO SAC – CAMPO TELEFÔNICO – **lógica de bloqueio implementada** 
- **Tarefa:** Bloquear a continuação do formulário do Mesa de Decisão SAC caso o número de telefone informado não contenha exatamente 11 caracteres válidos (incluindo DDD).  
- **Tempo gasto:** 8h  
- **Resumo anterior (30/06):**  
  - Projeto preparado para alcançar a tela da funcionalidade.  
  - Danilo realizou acesso técnico ao banco utilizado pelo sistema.  
  - Liberação de senha do IbiPlus permitiu o acesso completo à tela com campos dinâmicos.  
- **Status (01/07):**  
  - Analisado o componente `TextBoxDinamico`, com máscara `(00)00000-0000`.  
  - Identificado que a validação anterior apenas marcava como obrigatório, sem verificar quantidade de dígitos.  
  - Implementado ajuste no método `ValorValido(MaskedTextBox item)`, com:  
    - Remoção de todos os caracteres não numéricos.  
    - Verificação de exatamente 11 dígitos.  
    - Exibição da mensagem: _"Telefone (XX)XXXXX-XXXX deve conter exatamente 11 números."_  
    - Bloqueio da continuação do formulário em caso de erro.  
- **Próximos passos:** Início dos testes com a equipe para validar a funcionalidade e verificar necessidade de ajustes finais.  
---

## 🗓️ **30/06**

###  Resumo de Horas do Dia
<table>
  <thead>
    <tr>
      <th style="color:#000000">Dia</th>
      <th style="color:#000000">Tempo</th>
      <th style="color:#000000">Tarefa</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>02:00</td>
      <td>CNU – Atualização do ChromeDriver – Acompanhamento Release</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>03:00</td>
      <td style="color:#ff0000">Impedimento – Sem Demanda</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>01:00</td>
      <td>Impedimento – Sistema do Cliente IbiPlus (Necessidade de Login)</td>
    </tr>
    <tr style="background-color:#ffffff; color:#000000">
      <td>30/06</td>
      <td>02:00</td>
      <td>Bradesco – [INCIDENTE NEG.] Mesa de Decisão SAC – Análise inicial do problema</td>
    </tr>
  </tbody>
</table>

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
- **Observação:** 