# BOOTSTRAP — KIT IA DEV + KNOWLEDGE DICTIONARY

Você vai inicializar o **Kit IA Dev** no repositório existente.

Esta execução tem como objetivo preparar o ambiente de IA, Agents, Skills, documentação, conhecimento, governança, GitFlow e backlog de Tasks.

## REGRA CRÍTICA

**NÃO IMPLEMENTE O PROJETO NESTA EXECUÇÃO.**

O projeto NÃO deve ser criado ainda.

Primeiro devemos instalar/configurar o Kit IA Dev, carregar todo o conhecimento disponível e somente depois estruturar o backlog e as Tasks que serão executadas futuramente.

Fale comigo em **português do Brasil**.

Conteúdo técnico de:

- `CLAUDE.md`
- `AGENTS.md`
- `SKILL.md`
- `agent_docs`
- instruções técnicas para Agents

deve permanecer em inglês quando o padrão do Kit assim determinar.

---

# 1. CAMINHOS OFICIAIS

## Kit IA Dev

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\Kit-IA-Dev
```

## Projeto alvo

```text
D:\Empresa\GFMaurila\projetos\gfm-template-cms-aws
```

O segundo caminho é a raiz oficial do repositório.

---

# 2. OBJETIVO DESTA EXECUÇÃO

Nesta execução você deve SOMENTE:

1. analisar e instalar/inicializar o Kit IA Dev;
2. analisar a estrutura atual do repositório;
3. localizar e carregar o Knowledge Dictionary;
4. ler TODA a documentação relevante;
5. consolidar os requisitos encontrados;
6. preparar Agents;
7. preparar Skills;
8. preparar documentação de governança;
9. preparar estrutura de execução;
10. preparar GitFlow;
11. criar o backlog;
12. decompor o backlog em Tasks;
13. identificar dependências;
14. definir branch para cada Task;
15. preparar automação futura de execução;
16. preparar commit/push/PR/review/merge automático;
17. parar antes da implementação.

---

# 3. NÃO CRIAR O PROJETO AINDA

É PROIBIDO nesta execução criar ou implementar:

- `.sln`;
- `.csproj`;
- APIs;
- backend;
- frontend;
- React;
- entidades;
- endpoints;
- handlers;
- repositories;
- migrations;
- bancos;
- Docker Compose da aplicação;
- containers da aplicação;
- recursos AWS;
- Terraform;
- CloudFormation;
- CDK;
- Kafka;
- RabbitMQ;
- Redis;
- MongoDB;
- MySQL;
- código funcional;
- testes funcionais da aplicação.

Esta execução é exclusivamente:

```text
BOOTSTRAP
+
KNOWLEDGE LOADING
+
PLANNING
+
GOVERNANCE
+
AGENTS
+
SKILLS
+
TASKS
+
GITFLOW
```

---

# 4. INSTALAR E ANALISAR O KIT IA DEV

Primeiro analise:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\Kit-IA-Dev
```

Localize e leia, quando existirem:

```text
README.md
PROJECT.md
PROJECT_STRUCTURE.md
PROJECT_SKILLS.md
prompts.md
CLAUDE.md
AGENTS.md
3-Skills/
3-Skills/COMO-INSTALAR.md
agent_docs/
references/
templates/
SKILL.md
```

Não copie arquivos cegamente.

Primeiro entenda como o Kit funciona e como espera ser instalado.

Preserve integralmente a estrutura das Skills:

```text
skill-name/
├── SKILL.md
└── references/
```

Quando houver arquivos adicionais pertencentes à Skill, preserve-os também.

---

# 5. KNOWLEDGE DICTIONARY — REGRA OBRIGATÓRIA

Antes de criar, alterar, ordenar ou remover qualquer Task, procure no projeto/Kit o diretório:

```text
docs/dicionario/
```

Esse diretório representa o **Knowledge Dictionary do projeto**.

Ele foi construído a partir dos chats e estudos anteriores do projeto **IA Claude**.

Os documentos desse diretório NÃO são documentação opcional.

Eles são:

```text
PROJECT KNOWLEDGE SOURCE
```

e devem ser tratados como entrada obrigatória para planejamento.

---

# 6. LEITURA OBRIGATÓRIA DO DICIONÁRIO

Leia TODOS os arquivos `.md` existentes em:

```text
docs/dicionario/
```

Não leia apenas arquivos cujo nome aparentemente tenha relação com a Task.

Nesta etapa de bootstrap, faça uma leitura completa.

O dicionário contém conhecimento relacionado a assuntos como:

- estrutura de projetos;
- Agentic Workflow;
- RAG;
- Agentic RAG;
- Graph RAG;
- Agents;
- Skills;
- Plugins;
- MCP;
- conectores;
- frameworks;
- CI/CD;
- LLM local;
- microsserviços;
- arquitetura;
- aplicações;
- SEO/AEO;
- Free LLM APIs;
- LinkedIn Manager Agent;
- ferramentas de escritório;
- observabilidade;
- AWS;
- setup AWS;
- práticas de desenvolvimento;
- padrões arquiteturais;
- ideias que podem ser aplicadas ao projeto.

Não assuma que todos os itens deverão ser implementados.

Primeiro classifique sua relevância.

---

# 7. KNOWLEDGE DISCOVERY

Para cada documento do dicionário, identifique:

```text
Concept
Purpose
Project Relevance
Architecture Impact
Infrastructure Impact
Development Impact
AI/Agent Impact
Security Impact
Testing Impact
DevOps Impact
Documentation Impact
Possible Tasks
Dependencies
Priority
Decision
```

`Decision` deverá ser uma destas:

```text
ADOPT
ADAPT
REFERENCE
FUTURE
NOT_APPLICABLE
```

---

# 8. CONSOLIDAÇÃO DO CONHECIMENTO

Depois de ler o dicionário inteiro, produza um mapa consolidado.

Crie:

```text
docs/knowledge/PROJECT_KNOWLEDGE_MAP.md
```

Ele deverá relacionar:

```text
Dicionário
    ↓
Conceitos
    ↓
Requisitos
    ↓
Arquitetura
    ↓
Decisões
    ↓
Tasks
```

Também crie:

```text
docs/knowledge/KNOWLEDGE_DECISIONS.md
```

registrando:

- o que será adotado;
- o que será adaptado;
- o que será apenas referência;
- o que ficará para versões futuras;
- o que não se aplica;
- justificativa.

---

# 9. NÃO TRANSFORMAR TODO O DICIONÁRIO EM TASK

O dicionário é uma fonte de conhecimento.

Ele NÃO é automaticamente um backlog.

Exemplo:

```text
Conhecimento encontrado
        ↓
analisar relevância
        ↓
comparar com arquitetura
        ↓
identificar benefício
        ↓
identificar dependências
        ↓
tomar decisão
        ↓
somente então
        ↓
criar Task
```

Evite transformar estudos ou conceitos puramente informativos em funcionalidades sem necessidade.

---

# 10. FONTE ARQUITETURAL PRINCIPAL

Depois do Knowledge Dictionary, utilize como baseline arquitetural:

```text
02 - dotnet - AWS
```

A arquitetura definida nessa referência tem prioridade para estruturar o projeto AWS.

Considere:

```text
.NET
ASP.NET Core
Modular Monolith
DDD
SOLID
Clean Code
CQRS
Commands
Queries
Domain Events
Vertical Slice quando aplicável
Transactional Outbox
```

Persistência:

```text
MySQL
MongoDB
Redis
```

Mensageria:

```text
Kafka
RabbitMQ
```

Cloud Target:

```text
AWS
├── SQS
├── SNS
├── Lambda
├── S3
├── EC2
└── ECS
```

Observabilidade:

```text
Structured Logging
Correlation ID
OpenTelemetry
Distributed Tracing
Metrics
Health Checks
Readiness
Liveness
```

Arquitetura/documentação:

```text
C4
Structurizr DSL
Structurizr Lite
Draw.io
UML
ER
ADR
```

Evolução:

```text
LOCAL FIRST
     ↓
CONTAINER FIRST
     ↓
CLOUD READY
     ↓
AWS TARGET
```

Não implemente nada disso agora.

Use essas informações para planejamento.

---

# 11. ORDEM DE PRECEDÊNCIA DAS INFORMAÇÕES

Ao planejar o projeto, siga esta hierarquia:

```text
1. Instruções explícitas deste prompt
          ↓
2. Documentação oficial existente do projeto
          ↓
3. Arquitetura 02 - dotnet - AWS
          ↓
4. Knowledge Dictionary
          ↓
5. Kit IA Dev
          ↓
6. Boas práticas gerais
```

Não substitua uma decisão específica do projeto por uma recomendação genérica encontrada no dicionário.

---

# 12. DETECÇÃO DE CONFLITOS

Antes das Tasks, procure conflitos entre:

```text
PROJECT.md
PROJECT_STRUCTURE.md
prompts.md
CLAUDE.md
AGENTS.md
Architecture
Knowledge Dictionary
Kit IA Dev
GitFlow
```

Classifique-os como:

```text
DUPLICATE
COMPLEMENTARY
CONFLICT
OBSOLETE
MISSING
```

Documente em:

```text
docs/knowledge/KNOWLEDGE_CONFLICTS.md
```

Não resolva silenciosamente conflitos arquiteturais importantes.

Registre a decisão tomada e a justificativa.

---

# 13. AGENTS

Prepare o workflow:

```text
Requirements Agent
        ↓
Knowledge Agent
        ↓
Architect Agent
        ↓
Tech Lead Agent
        ↓
Developer Agent
        ↓
Tester / QA Agent
        ↓
Reviewer Agent
        ↓
Architecture Validation Agent
        ↓
Documentation Agent
```

## Knowledge Agent

Inclua explicitamente um `Knowledge Agent`.

Responsabilidades:

```text
ler docs/dicionario/
        ↓
ler documentação do projeto
        ↓
consolidar conhecimento
        ↓
detectar conflitos
        ↓
identificar decisões anteriores
        ↓
fornecer contexto aos demais Agents
```

Nenhum Agent deve implementar funcionalidades nesta execução.

---

# 14. KNOWLEDGE GATE

Adicione um novo Quality Gate antes da criação das Tasks:

```text
KNOWLEDGE QUALITY GATE
```

Ele deverá confirmar:

- [ ] Kit IA Dev analisado
- [ ] documentação principal lida
- [ ] `docs/dicionario/` lido completamente
- [ ] arquitetura `02 - dotnet - AWS` considerada
- [ ] decisões consolidadas
- [ ] conflitos identificados
- [ ] duplicidades identificadas
- [ ] requisitos consolidados
- [ ] impactos arquiteturais avaliados
- [ ] Knowledge Map criado

Se qualquer item obrigatório falhar:

```text
STOP
```

Não criar Tasks.

---

# 15. ORDEM OBRIGATÓRIA PARA CRIAÇÃO DAS TASKS

A criação das Tasks deve acontecer SOMENTE nesta ordem:

```text
KIT IA DEV
    ↓
DOCUMENTAÇÃO DO PROJETO
    ↓
KNOWLEDGE DICTIONARY
    ↓
02 - DOTNET - AWS
    ↓
KNOWLEDGE CONSOLIDATION
    ↓
CONFLICT ANALYSIS
    ↓
REQUIREMENTS
    ↓
ARCHITECTURE
    ↓
KNOWLEDGE QUALITY GATE
    ↓
BACKLOG
    ↓
TASKS
```

É proibido pular diretamente para:

```text
PROMPT → TASKS
```

---

# 16. TASK-DRIVEN DEVELOPMENT

Depois que o Knowledge Gate estiver aprovado, crie:

```text
tasks/
├── backlog/
├── ready/
├── in-progress/
├── review/
├── blocked/
└── done/
```

Cada Task deverá possuir:

```text
ID
Title
Description
Objective
Business Context
Knowledge References
Architecture References
Scope
Out of Scope
Dependencies
Acceptance Criteria
Tests Required
Documentation Required
Branch
Status
Assigned Agent
Reviewer
Quality Gates
Merge Target
```

---

# 17. KNOWLEDGE REFERENCES NAS TASKS

Toda Task deverá indicar de onde veio sua necessidade.

Exemplo:

```text
Knowledge References:
- docs/dicionario/02-rag.md
- docs/dicionario/15-rag-system.md

Architecture References:
- ARCHITECTURE_PLAN.md
- ADR-XXX
```

Isso cria rastreabilidade:

```text
CONHECIMENTO
     ↓
DECISÃO
     ↓
REQUISITO
     ↓
TASK
     ↓
CÓDIGO
```

---

# 18. GRANULARIDADE DAS TASKS

Utilize:

```text
1 Task
   ↓
1 objetivo claro
   ↓
1 branch
   ↓
implementação
   ↓
testes
   ↓
review
   ↓
PR
   ↓
merge
```

Evite Tasks gigantes.

Utilize IDs:

```text
TASK-001
TASK-002
TASK-003
...
```

---

# 19. DEPENDÊNCIAS

Crie um Dependency Graph.

Exemplo:

```text
TASK-001
   ↓
TASK-002
   ├── TASK-003
   └── TASK-004
          ↓
      TASK-005
```

Uma Task somente poderá assumir:

```text
READY
```

quando todas as dependências obrigatórias estiverem:

```text
DONE
```

---

# 20. GITFLOW

Branches permanentes:

```text
main
develop
hml
```

Desenvolvimento:

```text
develop
   │
   ├── feature/task-001-...
   ├── feature/task-002-...
   ├── feature/task-003-...
   └── feature/task-xxx-...
```

Cada Task possui obrigatoriamente:

```text
feature/task-<id>-<descricao-curta>
```

Nunca implementar diretamente em:

```text
main
develop
hml
```

---

# 21. EXECUÇÃO FUTURA AUTOMATIZADA

Quando posteriormente for autorizada a implementação:

```text
Knowledge Context
       ↓
Selecionar próxima TASK READY
       ↓
Validar dependências
       ↓
git checkout develop
       ↓
git pull
       ↓
criar feature/task-xxx
       ↓
executar Task
       ↓
build
       ↓
tests
       ↓
quality gates
       ↓
Reviewer Agent
       ↓
Architecture Validation
       ↓
Documentation Agent
       ↓
git add
       ↓
git commit
       ↓
git push
       ↓
criar PR
       ↓
AI Review
       ↓
Quality Gates
       ↓
merge automático em develop
       ↓
TASK DONE
       ↓
próxima TASK READY
```

---

# 22. MERGE AUTOMÁTICO

Merge automático somente quando TODOS estiverem verdes:

```text
Build
Unit Tests
Integration Tests
Architecture Validation
Code Review
Security Checks
Documentation
Acceptance Criteria
Knowledge Compliance
```

Se qualquer Gate falhar:

```text
NO MERGE
```

A Task retorna para:

```text
in-progress
```

ou:

```text
blocked
```

Depois:

```text
corrigir
   ↓
testar
   ↓
review
   ↓
validar
   ↓
PR
   ↓
merge
```

---

# 23. PROMOÇÃO

Tasks:

```text
feature/task-*
      ↓
develop
```

Homologação:

```text
develop
   ↓
hml
```

Release:

```text
develop
   ↓
release/1.0.0.0
   ↓
hml
   ↓
validation
   ↓
main
   ↓
PROD
```

Não execute release nesta etapa.

---

# 24. BACKLOG INICIAL

Depois da leitura do dicionário e aprovação do Knowledge Gate, decomponha o projeto considerando:

## Foundation

- repository;
- Solution;
- architecture;
- environments;
- configuration.

## Backend

- Domain;
- Application;
- Infrastructure;
- APIs;
- CQRS;
- Domain Events;
- validation;
- policies;
- permissions.

## Persistence

- MySQL;
- MongoDB;
- Redis;
- migrations;
- seeds;
- fake data.

## Security

- JWT;
- Refresh Token;
- Login;
- Forgot Password;
- Reset Password;
- Roles;
- Permissions.

## Messaging

- Kafka;
- RabbitMQ;
- Outbox;
- Retry;
- Idempotency;
- DLQ.

## Frontend

- React Site;
- React Admin;
- Authentication;
- Authorization;
- API integration.

## Docker

- DEV;
- TEST;
- HML;
- PROD.

## Observability

- Structured Logging;
- Correlation ID;
- OpenTelemetry;
- Tracing;
- Metrics;
- Health Checks.

## AWS

- SQS;
- SNS;
- Lambda;
- S3;
- EC2;
- ECS.

## AI / Knowledge

Considere os conceitos relevantes encontrados em:

```text
docs/dicionario/
```

principalmente quando houver decisões relacionadas a:

- LLM;
- RAG;
- Agentic RAG;
- Agents;
- Skills;
- MCP;
- AI workflows;
- integrations;
- local LLM;
- AI APIs.

Somente crie Tasks para esses componentes quando a análise indicar:

```text
ADOPT
```

ou:

```text
ADAPT
```

---

# 25. PROMPTS.MD COMO ORQUESTRADOR

Atualize/prepare:

```text
prompts.md
```

para futuramente executar:

```text
START
   ↓
LOAD PROJECT
   ↓
LOAD KIT
   ↓
LOAD KNOWLEDGE DICTIONARY
   ↓
LOAD ARCHITECTURE
   ↓
RUN KNOWLEDGE AGENT
   ↓
VALIDATE KNOWLEDGE GATE
   ↓
LOAD BACKLOG
   ↓
SELECT NEXT READY TASK
   ↓
VALIDATE DEPENDENCIES
   ↓
CREATE TASK BRANCH
   ↓
RUN REQUIRED AGENTS
   ↓
IMPLEMENT
   ↓
TEST
   ↓
REVIEW
   ↓
ARCHITECTURE VALIDATION
   ↓
DOCUMENT
   ↓
COMMIT
   ↓
PUSH
   ↓
PR
   ↓
QUALITY GATES
   ↓
AUTO MERGE
   ↓
TASK DONE
   ↓
NEXT READY TASK
```

## MUITO IMPORTANTE

NÃO execute esse loop agora.

Somente prepare o mecanismo.

---

# 26. REGRA PARA TODAS AS EXECUÇÕES FUTURAS

Antes de qualquer Agent trabalhar em uma Task futura, ele deverá carregar:

```text
README.md
PROJECT.md
PROJECT_STRUCTURE.md
prompts.md
CLAUDE.md
AGENTS.md
REQUIREMENTS.md
ARCHITECTURE_PLAN.md
EXECUTION_PLAN.md
PROJECT_KNOWLEDGE_MAP.md
KNOWLEDGE_DECISIONS.md
ADRs relevantes
Task atual
Knowledge References da Task
```

Quando necessário, consultar novamente:

```text
docs/dicionario/
```

Isso evita decisões desconectadas do conhecimento acumulado do projeto.

---

# 27. CHECKPOINT FINAL OBRIGATÓRIO

Ao terminar o bootstrap, PARE.

Apresente:

```text
BOOTSTRAP REPORT

Kit IA Dev:
- status

Skills:
- instaladas
- atualizadas

Agents:
- preparados

Knowledge Dictionary:
- arquivos encontrados
- arquivos lidos
- conceitos identificados

Knowledge:
- ADOPT
- ADAPT
- REFERENCE
- FUTURE
- NOT_APPLICABLE

Conflicts:
- encontrados
- resolvidos
- pendentes

Architecture:
- status

Tasks:
- total
- backlog
- ready
- blocked

Dependencies:
- resumo

GitFlow:
- status

Branches:
- existentes
- planejadas

Next Candidate Task:
- TASK-XXX

Implementation:
- NOT STARTED
```

Finalize obrigatoriamente com:

```text
BOOTSTRAP CONCLUÍDO
KNOWLEDGE DICTIONARY CARREGADO
TASKS E DEPENDÊNCIAS PREPARADAS
IMPLEMENTAÇÃO NÃO INICIADA

AGUARDANDO AUTORIZAÇÃO PARA EXECUTAR A PRIMEIRA TASK.
```

Não crie a branch da primeira Task de implementação.

Não implemente a primeira Task.

Não inicialize automaticamente o loop.

Aguarde autorização.