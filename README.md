# Desafio 2 - Hora de Estruturar a Área de Testes da Empresa

![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)
![Mentoria](https://img.shields.io/badge/Mentoria-Julio%20de%20Lima-blue)
![Tipo](https://img.shields.io/badge/Tipo-Estrutura%20de%20QA-yellow)
![Atividade](https://img.shields.io/badge/Atividade-Refinamento-red)
![Atividade](https://img.shields.io/badge/Atividade-Modelagem-purple)
![Atividade](https://img.shields.io/badge/Atividade-Execução-blue)
![Atividade](https://img.shields.io/badge/Atividade-Automação-green)

---

## Visão Geral do Projeto  

Este repositório contém a entrega do **Desafio 2 da Mentoria de Teste de Software do Julio de Lima**.  

O objetivo do desafio foi **estruturar a área de QA da empresa fictícia "Clebinho Soluções em Pagamentos"**, que não possuía práticas de teste e trabalha exclusivamente com APIs.

Nosso grupo definiu processos, responsabilidades, atividades, dependências e ferramentas para:  

- **Refinamento com foco em testes**  
- **Modelagem de testes**  
- **Execução com gestão de defeitos**  
- **Automação de testes**

A entrega final está disponível na [Planilha](https://docs.google.com/spreadsheets/d/1Lx6TYFZ2wgXCl01ShrnJNi0V3JGHb9_w/edit?gid=1668832291#gid=1668832291)

---

## Objetivos do Projeto  

- Estruturar a área de QA dentro da empresa "Clebinho Soluções em Pagamentos".  
- Definir responsabilidades dos membros da equipe.  
- Criar fluxos detalhados para **refinamento, modelagem, execução e automação**.  
- Mapear **dependências e ferramentas** necessárias para cada atividade.  

---

## Tecnologias e Ferramentas  

- **Notion** → Organização das atividades e responsabilidades.  
- **Google Sheets** → Estruturação final da entrega em formato tabular.  

---

## Resultados  

### Estrutura do Processo de **Refinamento** (foco em testes)

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
|-----------|-----------|--------------|------------|-------------|
| Solicitar ao PO as User Stories | Antes de iniciar o processo | User Stories definidas e priorizadas pelo PO | Jira, Zephyr | QA |
| Estudo preliminar de mercado | Após receber User Stories | User Stories recebidas | Notepad++ | QA |
| Verificar DoR definida pelo time | Após estudo preliminar | Documentos de negócio e técnicos | Swagger | TIME |
| Levantar Riscos | Antes da reunião com o time | Informações das etapas anteriores | ChatGPT, Excel | QA + PO |
| Perguntas ao PO | Durante reunião | Critérios de aceitação iniciais | Jira | QA |
| Verificar e sugerir melhorias nos CA | Durante reunião | User Stories e CA iniciais | Cucumber, Jira | TIME |
| Validar riscos com o time | Durante reunião | Levantamento de Riscos | Jira, Excel | TIME |
| Estimar esforço de teste | Durante reunião | Discussões e User Stories validadas | Jira, Excel | QA + SM |
| Estimar esforço de implementação | Durante reunião | Discussões e User Stories validadas | Jira, Excel | DEV + PO + SM |
| Revisar artefatos | Após reunião | Registros anteriores | Notepad++ | QA + DEV |

---

### Estrutura do Processo de **Modelagem de Testes**

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
|-----------|-----------|--------------|------------|-------------|
| Verificar regras de negócio | Antes da modelagem | Documentação do produto | Notion, Jira, Docs | QA |
| Verificar critérios de aceitação | Após validação das regras | Documentação do produto | Notion, Jira, Docs | QA |
| Analisar documentação Swagger | Após análise dos critérios | Disponibilidade do Swagger atualizado | Swagger | QA | 
| Definir modelagem dos casos de teste | Após entendimento da API | Critérios acordados | Notion, Jira, Docs | QA + PO |
| Definir registro dos casos | Junto da modelagem | Ferramenta disponível | Jira, TestRail, Planilha | QA + PO |
| Definir ferramentas e linguagens | Antes da criação dos casos | Alinhamento com QA e Dev | Postman, Python, Java, JS | QA + QA Lead |
| Definir dados de teste | Antes da escrita dos cenários | Base de dados configurada | Jira, TestRail, Planilha | QA + Dev |
| Aplicar técnica Partição de Equivalência | Após dados de teste | Documentação e CA | Jira, TestRail, Planilha | QA |
| Criar casos de teste VADER | Durante escrita | Critérios de aceitação e ferramentas | Jira, TestRail, Planilha | QA |
| Revisar cenários com o time | Após elaboração inicial | Alinhamento com Dev + PO | Reuniões, Jira | QA + Dev + PO |
| Definir casos a serem automatizados | Após revisão | Critérios de priorização | Reuniões, Jira | QA + QA Lead |

---

### Estrutura do Processo de **Execução com gestão de defeitos**

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
|-----------|-----------|--------------|------------|-------------|
| Obter documentação/Especificação da API | Após desenvolvimento | Documentação Swagger | Swagger | DEV |
| Configurar ambiente de testes | Após liberação da implementação | Infraestrutura liberada | AWS | Infra + DEV + QA |
| Verificar ambiente de teste | Após configuração | Configuração validada | AWS | QA |
| Criar massa de dados | Após ambiente validado | Documentação Swagger | AWS | QA |
| Executar testes via Postman | Após revisão dos casos | Casos + ambiente + massa de dados | AWS / Jira / Postman | QA |
| Registrar resultados | Após execução | Resultado dos testes | Jira | QA |
| Relatar bug | Após bug encontrado | Resultado dos testes | Jira | QA |
| Corrigir bug | Após registro | Atribuição ao DEV | IDE, GitHub, Jira | DEV |
| Atualizar ambiente | Após correção | Nova versão da tarefa | AWS | Infra + DEV + QA |
| Criar novo ciclo de teste | Após liberação da correção | Bug corrigido | Jira | QA |
| Testar bugs corrigidos | Após atualização do ambiente | Ambiente atualizado | AWS / Jira | QA |
| Teste de regressão | Após bug corrigido | Ambiente atualizado | AWS / Jira | QA |
| Registrar testes realizados | Após regressão | Testes concluídos sem bugs | Jira | QA |

---

### Estrutura do Processo de **Automação**

| Atividade | Sequência | Dependências | Ferramentas | Responsável |
|-----------|-----------|--------------|------------|-------------|
| Desenvolvimento de testes unitários | Após tarefa iniciada | Tarefa pronta | Mocha, Chai, Sinon | DEV |
| Desenvolvimento de testes de integração | Após tarefa iniciada | Tarefa pronta | Mocha, Chai, Sinon | DEV |
| Auxílio na elaboração de testes | Após DEV iniciar criação | Tarefa iniciada | Meet, Teams, Zoom, Discord | QA |
| Revisão de código dos testes | Após pull request | Implementação pronta | GitHub | QA/DEV |
| Avaliação dos testes existentes | Após liberação da tarefa | Aprovação PR | Jira, Swagger | QA |
| Criação de testes E2E para API | Após avaliação | Testes anteriores | Supertest, Mocha, Chai | QA |
| Acompanhamento CI | Após pull request dos testes E2E | Criação dos testes E2E | GitHub Actions | QA |

---

## O que aprendi

- A importância de estruturar a área de QA.
- Compreender as etapas de cada processo de QA: refinamento, modelagem, execução e automação.
- Planejar a ordem das atividades para que o processo seja eficiente e completo.
- Identificar responsabilidades, dependências e ferramentas necessárias para cada etapa.
- Organização de processos de QA em equipes ágeis.

---

## Melhorias Futuras  

- Expandir o processo de QA para outros tipos de testes além de API, como UI, mobile ou integração.
- Criar documentação padronizada e templates para cada atividade, facilitando onboarding de novos QAs.

---

## Arquivos do Projeto  
- `Desafio 2.pdf` → Relatório completo do desafio
- `Desafio 2.xlsx` → Relatório completo do desafio em formato xlsx
- `README.md` → Documentação do projeto

**Equipe**: Celia Bruno, Geissy Araujo, Igor Andrade, Pamela Persuhn, Patricia Possari

Projeto completo também disponível no Notion: [Link para o Notion](https://www.notion.so/Desafio-2-Hora-de-Estruturar-a-rea-de-Testes-da-Empresa-276a3634ecc380379a05c455def952f3?source=copy_link)
