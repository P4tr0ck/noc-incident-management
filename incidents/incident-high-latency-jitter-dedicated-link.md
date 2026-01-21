# Incidente – Alta Latência e Perda de Pacotes em Link Dedicado

> **Nota:** Este incidente foi documentado com base em uma experiência real em ambiente de provedor de internet. Todos os dados, nomes e identificadores foram **anonimizados** para fins de estudo, documentação e portfólio profissional.

---

## 📌 Contexto do Ambiente

- **Tipo de ambiente:** Provedor de internet local de pequeno/médio porte  
- **Tipo de serviço:** Link Dedicado  
- **Responsabilidade do NOC:**  
  - Realizar tratativa remota inicial  
  - Caso não resolvido, abrir chamado para deslocamento de equipe técnica em até **4 horas**  
- **Ferramentas envolvidas:**  
  - Grafana (monitoramento, ping)  
  - Telegram (alertas)  
  - Telefone (contato com responsável técnico do cliente)

---

## 🚨 Descrição do Incidente

- **Tipo de incidente:** Alta latência / Perda de pacotes (Jitter)  
- **Data/Horário:** Domingo pela manhã  
- **Origem do alerta:**  
  - Alerta sonoro e visual via Grafana  
  - Notificação simultânea via Telegram  
- **Serviço/Elemento afetado:**  
  - Conexão de internet de cliente corporativo (link dedicado)  
- **Status inicial:**  
  - Serviço operava normalmente antes de apresentar **quedas abruptas no gráfico de tráfego** e instabilidade na conectividade

---

## 📉 Impacto

- **Usuários afetados:** Cliente corporativo (posto de gasolina)  
- **Impacto operacional:**  
  - Lentidão em pagamentos eletrônicos  
  - Emissão de notas fiscais intermitente  
  - Redução da qualidade de transmissão das câmeras de segurança  
- **Impacto em SLA:**  
  - Risco de violação de SLA devido à degradação do serviço  
- **Classificação de criticidade:** Média / Alta  

---

## 🔍 Diagnóstico Inicial

### Validação do alerta
- Confirmação do alerta no Grafana  
- Análise dos gráficos de tráfego, latência e perda de pacotes  
- Identificação de comportamento instável e intermitente  

### Verificações iniciais
- Testes de conectividade remota (ping)  
- Verificação de latência elevada e perda de pacotes  
- Avaliação das métricas de interface no período do alerta  

### Análise de histórico recente
- Consulta ao histórico do link  
- Identificação de estabilidade anterior ao incidente  
- Ausência de ocorrências recorrentes no mesmo período  

### Hipóteses iniciais
- Falha em equipamento de rede local do cliente  
- Degradação lógica ou física no ambiente interno  
- Possível saturação ou defeito em dispositivo de acesso  

---

## 🛠️ Ação Tomada

### Registro do incidente
- Abertura de chamado interno para registro e acompanhamento da ocorrência  

### Contatos realizados
- Contato telefônico com o responsável pela TI do cliente, conforme cadastro  

### Ajustes aplicados
- Orientações remotas para verificação de equipamentos locais  
- Solicitação de reinício controlado de dispositivos de rede internos  

### Escalonamento técnico
- Avaliação da necessidade de deslocamento técnico  
- Manutenção da tratativa remota antes da abertura de chamado externo  

### Ações de mitigação
- Monitoramento contínuo após ajustes iniciais  
- Acompanhamento do comportamento do link em tempo real  

---

## 📞 Comunicação

- **Forma de comunicação:** Telefonema  
- **Quem foi informado:** Responsável pela TI do cliente  
- **Frequência de atualização:**  
  - Comunicação inicial durante a tratativa  
  - Monitoramento contínuo ao longo da semana seguinte  
- **Registro em chamados:**  
  - Todas as interações e ações devidamente registradas  

---

## ✅ Resolução

### Descrição da resolução
Após a tratativa remota, foi identificado que a degradação estava relacionada a um **equipamento de rede local**, causando alta latência e perda de pacotes.

### Causa raiz
- Switch do cliente apresentando falha operacional  

### Ação corretiva
- Substituição do switch defeituoso no ambiente do cliente  

### Validações pós-correção
- Testes de ping remoto sem perda de pacotes  
- Verificação da estabilidade do tráfego no Grafana  
- Confirmação da normalização dos serviços críticos no local  

### Status final do serviço
- Serviço normalizado e estável  

---

## 📚 Lições Aprendidas

### O que funcionou bem
- Detecção rápida via monitoramento  
- Comunicação direta com o responsável técnico  
- Resolução eficiente após identificação da causa raiz  

### O que poderia ser melhor
- Diagnóstico mais rápido de equipamentos internos do cliente  
- Documentação prévia mais detalhada do ambiente  

### Pontos de atenção futuros
- Atenção especial a clientes com operação crítica  
- Monitoramento contínuo de padrões de latência e jitter  

---

## 🧩 Melhorias Propostas

### Monitoramento
- Criação de alertas específicos para jitter e latência elevada  

### Processo
- Padronização de checklist para incidentes de degradação  

### Documentação
- Atualização do inventário de equipamentos do cliente  

### Infraestrutura
- Recomendação de equipamentos mais confiáveis para clientes críticos  

---

## 🏷️ Habilidades Demonstradas

- Monitoramento de métricas de rede  
- Análise de incidentes de degradação  
- Comunicação com cliente corporativo  
- Escalonamento técnico  
- Documentação operacional  

---

## 🔚 Conclusão

Este incidente demonstra a importância da atuação do NOC na **detecção, análise e resposta a degradações de serviço**, mesmo sem indisponibilidade total.

A resposta rápida e a comunicação eficaz contribuíram para a **continuidade da operação do cliente** e para a **confiabilidade do ambiente**, reforçando a importância de processos bem definidos em operações de TI.
