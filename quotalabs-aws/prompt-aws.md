# PROMPT MASTER — QUOTA LABS AWS

Você vai me ajudar a preparar, analisar, documentar e estruturar o projeto **Quota Labs AWS** utilizando o **Kit IA Dev**.

Fale comigo em **português do Brasil**.

Os arquivos técnicos do projeto, como `CLAUDE.md`, `AGENTS.md`, `SKILL.md`, documentação de agentes e instruções técnicas internas, podem permanecer em inglês quando esse for o padrão original do Kit IA Dev.

---

# 1. PROJETO

Nome:

```text
Quota Labs AWS
```

Raiz oficial do projeto:

```text
D:\Empresa\GFMaurila\projetos\quotalabs-aws
```

IMPORTANTE:

Este projeto já possui contexto funcional, documentação, referências visuais, decisões arquiteturais e materiais existentes.

Você NÃO deve tratar o projeto como um projeto vazio.

Antes de propor alterações, leia e compreenda o conteúdo existente.

---

# 2. OBJETIVO DESTA EXECUÇÃO

Esta execução tem como objetivo:

1. instalar/configurar o Kit IA Dev;
2. analisar completamente o projeto existente;
3. analisar a documentação existente;
4. analisar as referências visuais;
5. analisar o Knowledge Dictionary;
6. identificar requisitos funcionais;
7. identificar requisitos não funcionais;
8. consolidar regras de negócio;
9. identificar integrações;
10. identificar gaps;
11. consolidar a arquitetura atual;
12. propor a arquitetura AWS alvo;
13. documentar decisões arquiteturais;
14. gerar ou atualizar diagramas;
15. gerar backlog;
16. decompor o backlog em tasks técnicas;
17. identificar dependências;
18. definir critérios de aceite;
19. definir estratégia de testes;
20. preparar a futura execução.

Porém:

> **NÃO IMPLEMENTE AS TASKS.**

O projeto depende de aprovação do cliente antes do início da implementação.

---

# 3. CLIENT APPROVAL GATE — REGRA ABSOLUTA

Existe um Quality Gate obrigatório:

```text
CLIENT_APPROVAL_GATE
```

Nenhuma task de implementação poderá ser iniciada sem aprovação explícita do cliente.

Até essa aprovação, todas as tasks deverão permanecer como:

```text
PENDING_CLIENT_APPROVAL
```

É permitido:

```text
Requirements
Architecture
Documentation
Architecture Decision Records
Backlog
Epics
Features
User Stories
Tasks
Subtasks
Acceptance Criteria
Technical Analysis
Dependency Mapping
Risk Analysis
Test Planning
Infrastructure Planning
Security Planning
Observability Planning
Cost Planning
Diagrams
API Contracts
Data Modeling
Definition of Ready
Definition of Done
```

É PROIBIDO:

```text
implementar código de produção
alterar funcionalidades
executar tasks do backlog
marcar task como IN_PROGRESS
criar feature branch para implementar task
realizar commit de implementação
realizar push de implementação
abrir PR de implementação
executar migration de produção
alterar infraestrutura real
realizar deploy
criar release
```

Somente a aprovação explícita poderá liberar a próxima fase.

Exemplos de comandos válidos:

```text
CLIENT APPROVED
```

ou:

```text
APROVADO PARA IMPLEMENTAÇÃO
```

Sem essa aprovação, pare obrigatoriamente após a preparação das tasks.

---

# 4. PRINCÍPIO DE EXECUÇÃO

Use como pipeline:

```text
BOOTSTRAP
   ↓
PROJECT DISCOVERY
   ↓
KNOWLEDGE DISCOVERY
   ↓
KNOWLEDGE QUALITY GATE
   ↓
REQUIREMENTS
   ↓
REQUIREMENTS QUALITY GATE
   ↓
ARCHITECTURE
   ↓
ARCHITECTURE QUALITY GATE
   ↓
BACKLOG
   ↓
TASK DECOMPOSITION
   ↓
TASK READINESS GATE
   ↓
CLIENT APPROVAL GATE
   ↓
STOP
```

A implementação NÃO faz parte desta execução.

---

# 5. KIT IA DEV

Pacotes esperados:

```text
Kit IA Dev
Templates por Stack
Skills Avançadas
```

Possíveis origens:

```text
Kit-IA-Dev/
Kit-IA-Dev.zip

Order-Bump-Templates-por-Stack/
Kit-IA-Dev-Templates-por-Stack.zip

Upsell1-Kit-IA-Dev/
Kit-IA-Dev-Skills-Avancadas.zip
```

Se algum pacote necessário não estiver disponível, peça o caminho absoluto.

Não invente arquivos ausentes.

---

# 6. KNOWLEDGE DICTIONARY

O Knowledge Dictionary oficial está em:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Essa pasta é uma fonte de conhecimento externa.

NÃO:

```text
copie
mova
renomeie
duplique
delete
```

o conteúdo dessa pasta para dentro do projeto.

Leia os arquivos diretamente de sua localização original.

---

# 7. KNOWLEDGE-FIRST RULE

ANTES de:

```text
Requirements
Architecture
Backlog
Tasks
```

leia integralmente os arquivos `.md` existentes em:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

O Knowledge Dictionary funciona como:

```text
Engineering Knowledge Base
Architecture Knowledge Base
AI Engineering Knowledge Base
DevOps Knowledge Base
Cloud Knowledge Base
Quality Knowledge Base
```

Não selecione somente arquivos aparentemente relacionados.

Leia o conjunto completo antes da consolidação arquitetural.

---

# 8. KNOWLEDGE QUALITY GATE

Depois da leitura, gere um relatório contendo:

```text
arquivos encontrados
arquivos lidos
arquivos ignorados
falhas de leitura
quantidade aproximada de conteúdo analisado
assuntos identificados
padrões arquiteturais identificados
padrões de IA identificados
padrões DevOps identificados
padrões Cloud/AWS identificados
padrões de segurança
padrões de testes
padrões de observabilidade
```

O gate somente poderá receber:

```text
PASS
```

se o conhecimento necessário tiver sido efetivamente analisado.

Caso contrário:

```text
FAIL
```

e interrompa o pipeline.

---

# 9. PROJECT DISCOVERY

Antes de alterar documentação, analise recursivamente:

```text
D:\Empresa\GFMaurila\projetos\quotalabs-aws
```

Mapeie:

```text
estrutura de diretórios
documentação
código existente
APIs
frontends
infraestrutura
Docker
configurações
bancos
mensageria
testes
CI/CD
scripts
diagramas
referências
prompts
agents
skills
```

Não sobrescreva decisões existentes sem justificativa.

---

# 10. REFERÊNCIAS VISUAIS

Existe material visual importante relacionado ao portal jurídico.

Analise especialmente:

```text
docs\references\screens\5. Back End - LawFirm
```

Considere as telas como fonte de requisitos.

Mapeie pelo menos os domínios encontrados nas referências:

```text
Campanhas / Visibilidade
Clientes
Contatos
Conteúdo Jurídico
Documentos
Estatísticas
Oportunidades Jurídicas
Perfil do Escritório
Planos
Cobrança
```

Não considere apenas nomes de arquivos.

Quando possível, relacione:

```text
Tela
↓
Feature
↓
Regra de negócio
↓
API
↓
Entidade
↓
Evento
↓
Integração
↓
Task futura
```

---

# 11. INTAKE E COMUNICAÇÃO

O sistema deverá considerar infraestrutura para recebimento de conteúdo enviado por clientes.

Tipos esperados:

```text
texto
mensagem
áudio
documentos
```

Pipeline conceitual:

```text
Client
   ↓
Communication / Intake
   ↓
API
   ↓
Storage
   ↓
Queue / Event
   ↓
Processing
   ↓
Transcription (quando necessário)
   ↓
Content Analysis
   ↓
Summary
   ↓
Legal Workflow
```

O conteúdo processado poderá gerar:

```text
transcrição
resumo
classificação
metadados
histórico
notificação
evento
workflow jurídico
```

Documente essa capacidade arquiteturalmente.

Não implemente ainda.

---

# 12. ARQUITETURA BASE

Adote como princípio:

```text
Local First
Container First
Cloud Ready
AWS Target
```

O domínio da aplicação NÃO deverá depender diretamente de AWS.

Use abstrações/adapters para infraestrutura.

Exemplo:

```text
Application
     ↓
Abstractions
     ↓
Infrastructure Adapters
     ↓
Local / AWS Providers
```

Isso deve permitir desenvolvimento e testes locais sem obrigar acesso à AWS.

---

# 13. BACKEND

Considere arquitetura .NET seguindo, quando compatível com o projeto:

```text
ASP.NET Core
DDD
CQRS
Vertical Slice
SOLID
Clean Code
Clean Architecture principles
Domain Events
Dependency Injection
FluentValidation
```

Separação conceitual:

```text
Domain
Application
Infrastructure
API
CrossCutting
```

Não force reorganização caso o projeto possua uma estrutura válida diferente.

Primeiro documente o estado atual.

Depois proponha o estado alvo.

---

# 14. PERSISTÊNCIA

Considere, quando aplicável:

```text
MySQL
MongoDB
Redis
```

Responsabilidades esperadas:

### MySQL

```text
dados transacionais
relacionamentos
integridade
operações de negócio
```

### MongoDB

```text
documentos
histórico
projeções
read models
conteúdo processado
transcrições
resumos
```

### Redis

```text
cache
TTL
sessões quando necessário
read optimization
locks quando necessário
```

Use:

```text
Cache Aside
```

quando apropriado.

Documente também:

```text
cache invalidation
TTL
fallback
consistência
```

---

# 15. DOMAIN EVENTS

Eventos de domínio devem permanecer desacoplados do broker.

Fluxo desejado:

```text
Domain
   ↓
Domain Event
   ↓
Application
   ↓
Integration Event
   ↓
Infrastructure
   ↓
Broker
```

Prepare a arquitetura para:

```text
Transactional Outbox
```

quando necessário.

---

# 16. MENSAGERIA

Considere suporte arquitetural para:

```text
Kafka
RabbitMQ
```

com responsabilidades distintas.

Kafka:

```text
event streaming
integration events
event-driven architecture
```

RabbitMQ:

```text
queues
background processing
work distribution
```

Todo processamento assíncrono deverá considerar:

```text
retry
timeout
idempotency
correlation ID
dead-letter queue
structured logging
observability
```

---

# 17. AWS TARGET

A arquitetura alvo deverá considerar:

```text
AWS SQS
AWS SNS
AWS Lambda
AWS S3
AWS EC2
AWS ECS
```

Mapeie claramente responsabilidades.

Exemplo:

```text
SQS
→ filas e processamento assíncrono

SNS
→ fan-out e notificações

Lambda
→ processamento serverless/event-driven

S3
→ documentos, uploads, áudio e objetos

EC2
→ workloads que necessitem máquinas virtuais

ECS
→ containers da aplicação
```

Não acople o domínio diretamente aos SDKs AWS.

---

# 18. EXECUÇÃO LOCAL

O ambiente local deverá ser capaz de representar os serviços externos necessários.

Avalie:

```text
Docker
Docker Compose
LocalStack
MySQL
MongoDB
Redis
Kafka
RabbitMQ
```

Objetivo:

```text
docker compose up
```

deve ser suficiente, sempre que possível, para subir a infraestrutura de desenvolvimento.

Não altere o ambiente nesta fase se isso representar implementação.

Documente o estado atual e o estado desejado.

---

# 19. SEGURANÇA

Analise:

```text
JWT
Refresh Token
Roles
Permissions
Policies
Secrets
Environment Variables
AWS IAM
Least Privilege
Encryption
PII
LGPD
Audit
Logging
```

Como se trata de contexto jurídico, trate dados de clientes e documentos como informações potencialmente sensíveis.

Nunca grave secrets reais na documentação.

---

# 20. OBSERVABILIDADE

Prepare arquitetura para:

```text
Structured Logging
Metrics
Tracing
Correlation ID
Health Checks
Distributed Tracing
OpenTelemetry
Dashboards
Alerts
```

Para operações assíncronas:

```text
Request
↓
Correlation ID
↓
API
↓
Event
↓
Queue
↓
Worker
↓
Database
```

deve ser rastreável.

---

# 21. TESTES

Defina estratégia para:

```text
Unit Tests
Integration Tests
Architecture Tests
Contract Tests
API Tests
End-to-End Tests
```

Quando houver infraestrutura:

```text
Testcontainers
```

poderá ser considerado.

Não execute implementação de testes das tasks nesta fase.

Apenas prepare:

```text
test strategy
test scenarios
acceptance tests
quality gates
```

---

# 22. DOCUMENTAÇÃO

Localize primeiro a documentação existente.

Não crie arquivos duplicados desnecessariamente.

Quando apropriado, consolide ou atualize:

```text
README.md
REQUIREMENTS.md
ARCHITECTURE.md
ARCHITECTURE_PLAN.md
PROJECT_STRUCTURE.md
EXECUTION_PLAN.md
BACKLOG.md
TASKS.md
TEST_STRATEGY.md
SECURITY.md
OBSERVABILITY.md
AWS_ARCHITECTURE.md
LOCAL_DEVELOPMENT.md
```

Se já existir documento equivalente, atualize-o em vez de criar outro com o mesmo propósito.

---

# 23. DIAGRAMAS

Preserve os diagramas existentes.

Quando necessário, proponha ou atualize diagramas em:

```text
draw.io
```

Diagramas esperados:

```text
System Context
Application Architecture
Backend Architecture
Frontend Architecture
AWS Infrastructure
Messaging
Data Architecture
Authentication
Client Intake
AI Processing
Deployment
Git Flow
CI/CD
```

Não apague diagramas existentes sem autorização.

---

# 24. REQUIREMENTS DISCOVERY

Consolide requisitos provenientes de:

```text
documentação
código
referências visuais
Knowledge Dictionary
arquitetura existente
regras já documentadas
```

Classifique:

```text
Functional Requirements
Non-Functional Requirements
Business Rules
Security Requirements
Infrastructure Requirements
Integration Requirements
Data Requirements
AI Requirements
Compliance Requirements
Observability Requirements
```

Para cada requisito, registre sua origem quando possível.

---

# 25. GAP ANALYSIS

Compare:

```text
CURRENT STATE
        ↓
TARGET STATE
```

Classifique gaps como:

```text
CRITICAL
HIGH
MEDIUM
LOW
```

Não corrija os gaps ainda.

Transforme-os em backlog.

---

# 26. BACKLOG

Estruture:

```text
Epic
  ↓
Feature
    ↓
User Story
      ↓
Task
        ↓
Subtask
```

Cada item deverá possuir, quando aplicável:

```text
ID
Title
Description
Business Value
Priority
Dependencies
Acceptance Criteria
Technical Notes
Security Impact
Infrastructure Impact
Test Requirements
Documentation Impact
```

---

# 27. TASK DECOMPOSITION

As tasks devem estar suficientemente detalhadas para futura execução por agentes de IA.

Formato sugerido:

```text
TASK-XXX
```

Cada task deverá conter:

```text
Objective
Context
Dependencies
Files/Areas potentially affected
Implementation Notes
Acceptance Criteria
Tests Required
Security Considerations
Observability Requirements
Documentation Requirements
Definition of Done
Status
```

Status obrigatório nesta fase:

```text
PENDING_CLIENT_APPROVAL
```

---

# 28. DEPENDENCY GRAPH

Gere o grafo lógico:

```text
TASK-001
   ↓
TASK-002
   ↓
TASK-003
```

Identifique tasks que podem futuramente ser executadas em paralelo.

Exemplo:

```text
TASK-001
 ├── TASK-002
 ├── TASK-003
 └── TASK-004
```

Mas NÃO execute nenhuma delas.

---

# 29. DEFINITION OF READY

Uma task somente poderá chegar ao Client Approval Gate se possuir:

```text
Requirement identified
Business rule identified
Architecture impact known
Dependencies known
Acceptance criteria defined
Test strategy defined
Security impact analyzed
Documentation impact analyzed
```

Caso contrário:

```text
NOT_READY
```

---

# 30. TASK READINESS GATE

Ao final da preparação, produza:

```text
Total Epics
Total Features
Total Stories
Total Tasks
Tasks Ready
Tasks Not Ready
Blocked Tasks
Dependencies
Critical Risks
```

Somente tasks `READY` poderão ser apresentadas para aprovação do cliente.

Mesmo as tasks `READY` permanecem:

```text
PENDING_CLIENT_APPROVAL
```

---

# 31. GIT

Analise o Git existente.

Considere como padrão alvo, se compatível:

```text
main
develop
hml
```

GitFlow:

```text
develop
   ↓
feature/task-XXX-description
   ↓
Pull Request
   ↓
develop
   ↓
hml
   ↓
release/x.y.z
   ↓
main
```

Porém:

NÃO crie branches de implementação nesta fase.

NÃO faça commits de implementação.

NÃO abra PRs de implementação.

Apenas documente o fluxo esperado.

---

# 32. AGENTES

Utilize o modelo de agentes do Kit IA Dev quando disponível.

Papéis esperados:

```text
Requirements Agent
Architect Agent
Tech Lead Agent
Security Agent
Developer Agent
Tester Agent
Reviewer Agent
Documentation Agent
```

Nesta execução:

```text
Developer Agent = PLANNING ONLY
Tester Agent = TEST PLANNING ONLY
Reviewer Agent = DOCUMENT/ARCHITECTURE REVIEW
```

Nenhum agente está autorizado a implementar features.

---

# 33. INSTALAÇÃO DAS SKILLS

Instale as skills do Kit seguindo as instruções oficiais.

Para cada skill:

copie a pasta completa:

```text
skill-name/
├── SKILL.md
└── references/
```

Não copie apenas o `SKILL.md`.

Consulte:

```text
3-Skills/COMO-INSTALAR.md
```

quando necessário.

---

# 34. SKILLS AVANÇADAS

Depois das skills básicas:

1. instalar as novas skills do pacote avançado;
2. aplicar os patches das skills existentes;
3. preservar `references/`;
4. substituir somente os `SKILL.md` indicados pelo pacote;
5. não sobrescrever skills sem verificar a instrução correspondente.

---

# 35. MULTI-TOOL

Caso a ferramenta não seja Claude Code, adapte o setup.

Verifique necessidade de:

```text
CLAUDE.md
AGENTS.md
tool-specific instructions
Agent Skills
```

Não assuma automaticamente que todas as ferramentas usam o mesmo diretório.

---

# 36. VALIDAÇÃO DAS SKILLS

Após instalação, faça validações simples.

Exemplos:

```text
"revisa esse código"
"escreve o commit"
"isso está lento"
"analise essa arquitetura"
```

Confirme se a skill adequada é ativada.

Isso é validação de setup e NÃO implementação do backlog.

---

# 37. QUALITY GATES

Use no mínimo:

```text
GATE-01 — Environment
GATE-02 — Kit Installation
GATE-03 — Knowledge
GATE-04 — Requirements
GATE-05 — Architecture
GATE-06 — Security
GATE-07 — Test Strategy
GATE-08 — Backlog
GATE-09 — Task Readiness
GATE-10 — Client Approval
```

Estados:

```text
PASS
FAIL
BLOCKED
PENDING_APPROVAL
```

---

# 38. REGRA CONTRA INVENÇÃO

Nunca invente:

```text
requisito
regra jurídica
regra de negócio
API
integração
credencial
segredo
serviço AWS existente
banco existente
decisão do cliente
```

Use:

```text
CONFIRMED
INFERRED
PROPOSED
UNKNOWN
```

para diferenciar o nível de certeza.

Itens `INFERRED` ou `PROPOSED` devem ser apresentados para validação.

---

# 39. REGRA DE PRESERVAÇÃO

Antes de alterar qualquer documento:

```text
READ
UNDERSTAND
COMPARE
THEN MODIFY
```

Nunca:

```text
DELETE AND RECREATE
```

automaticamente.

Preserve:

```text
documentação existente
diagramas existentes
referências
screenshots
decisões arquiteturais
histórico relevante
```

---

# 40. EXECUTION REPORT

Ao concluir a preparação, apresente:

```text
PROJECT ANALYSIS
KNOWLEDGE ANALYSIS
REQUIREMENTS
ARCHITECTURE
AWS TARGET
LOCAL ENVIRONMENT
SECURITY
OBSERVABILITY
TEST STRATEGY
GAP ANALYSIS
BACKLOG
TASKS
DEPENDENCIES
RISKS
QUALITY GATES
CLIENT APPROVAL STATUS
```

---

# 41. RESULTADO FINAL OBRIGATÓRIO

A execução deve terminar aproximadamente assim:

```text
============================================================
QUOTA LABS AWS — ENGINEERING PREPARATION
============================================================

Project Discovery ............... PASS
Kit IA Dev ...................... PASS
Knowledge Dictionary ............ PASS
Requirements .................... PASS
Architecture .................... PASS
Security Analysis ............... PASS
Test Strategy ................... PASS
Backlog ......................... PASS
Task Decomposition .............. PASS
Task Readiness .................. PASS

Implementation .................. NOT STARTED

Client Approval Gate ............ PENDING_APPROVAL

Tasks Ready: XX
Tasks Blocked: XX
Tasks Pending Client Approval: XX

============================================================
STOP CONDITION REACHED
============================================================

No implementation task has been started.

Waiting for explicit client approval.
============================================================
```

---

# 42. PROIBIÇÃO DE CONTINUAÇÃO AUTOMÁTICA

Depois de chegar ao:

```text
CLIENT_APPROVAL_GATE
```

NÃO pergunte:

```text
"Posso começar a TASK-001?"
```

NÃO inicie automaticamente.

NÃO interprete conclusão da documentação como autorização.

Apenas informe:

```text
CLIENT_APPROVAL_GATE = PENDING_APPROVAL
```

e encerre a execução.

---

# 43. APÓS FUTURA APROVAÇÃO

Esta seção define apenas o comportamento futuro.

Somente após comando explícito:

```text
CLIENT APPROVED
```

ou:

```text
APROVADO PARA IMPLEMENTAÇÃO
```

poderá ser iniciado um novo ciclo:

```text
Task
↓
Feature Branch
↓
Implementation
↓
Tests
↓
Review
↓
Quality Gate
↓
Commit
↓
Push
↓
Pull Request
```

Essa etapa NÃO pertence à execução atual.

---

# 44. INÍCIO DA EXECUÇÃO

Comece agora.

Primeiro valide:

```text
D:\Empresa\GFMaurila\projetos\quotalabs-aws
```

Depois localize e valide os pacotes do Kit IA Dev.

Em seguida leia:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Depois execute:

```text
Project Discovery
↓
Knowledge Quality Gate
↓
Requirements
↓
Architecture
↓
Gap Analysis
↓
Backlog
↓
Task Decomposition
↓
Task Readiness Gate
↓
CLIENT_APPROVAL_GATE
```

Execute todo o pipeline de preparação.

**PARE OBRIGATORIAMENTE NO CLIENT_APPROVAL_GATE.**

Não implemente nenhuma task.