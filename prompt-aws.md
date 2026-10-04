# BOOTSTRAP — KIT IA DEV

Você vai inicializar o **Kit IA Dev** no repositório existente, preparando a orquestração para posteriormente construir o projeto baseado na arquitetura definida no projeto de referência **02 - dotnet - AWS**.

Fale comigo em **português do Brasil**.

## 1. CAMINHOS

Kit IA Dev:

`D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\Kit-IA-Dev`

Projeto alvo:

`D:\Empresa\GFMaurila\projetos\gfm-template-cms-aws`

Considere o segundo caminho como a raiz oficial do repositório.

---

# 2. OBJETIVO DESTA EXECUÇÃO

Nesta execução você deve SOMENTE:

1. instalar/inicializar o Kit IA Dev;
2. analisar o repositório;
3. preparar Agents e Skills;
4. preparar a documentação de governança;
5. preparar a estrutura de execução;
6. decompor o projeto em Tasks;
7. definir dependências entre Tasks;
8. preparar GitFlow;
9. definir uma branch própria para cada Task;
10. preparar o fluxo automático de commit, push, PR, validação e merge;
11. deixar o projeto pronto para execução incremental posterior.

## IMPORTANTE

**NÃO IMPLEMENTE O PROJETO NESTA EXECUÇÃO.**

Não criar ainda:

- projetos `.csproj`;
- solution `.sln`;
- APIs;
- backend;
- frontend;
- React;
- banco de dados;
- migrations;
- Docker Compose da aplicação;
- containers da aplicação;
- AWS resources;
- Terraform/CloudFormation/CDK;
- Kafka;
- RabbitMQ;
- Redis;
- MongoDB;
- MySQL;
- endpoints;
- entidades de domínio;
- handlers;
- repositories;
- testes da aplicação;
- código funcional da aplicação.

A execução atual é exclusivamente de **bootstrap, planejamento, governança, Agents/Skills e Tasks**.

---

# 3. FONTE ARQUITETURAL

Todo planejamento futuro deve seguir a arquitetura definida no projeto/conversa de referência:

`02 - dotnet - AWS`

Considere como baseline:

- .NET;
- ASP.NET Core;
- Modular Monolith;
- DDD;
- SOLID;
- Clean Code;
- CQRS;
- Commands;
- Queries;
- Domain Events;
- Vertical Slice quando aplicável;
- Transactional Outbox;
- MySQL;
- MongoDB;
- Redis;
- Kafka;
- RabbitMQ;
- Docker;
- observabilidade;
- OpenTelemetry;
- AWS.

AWS Target:

- SQS;
- SNS;
- Lambda;
- S3;
- EC2;
- ECS.

Evolução arquitetural:

`LOCAL FIRST → CONTAINER FIRST → CLOUD READY → AWS TARGET`

Arquitetura e documentação:

- C4;
- Structurizr DSL;
- Structurizr Lite;
- Draw.io editável;
- ADRs.

Não implemente esses componentes agora.

Eles devem servir para gerar o **backlog estruturado de Tasks**.

---

# 4. KIT IA DEV

Primeiro analise:

`D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\Kit-IA-Dev`

Localize e leia:

- documentação;
- templates;
- `CLAUDE.md`;
- `AGENTS.md`;
- `SKILL.md`;
- `3-Skills`;
- `COMO-INSTALAR.md`;
- Agents;
- referências;
- instruções de instalação.

Não copie arquivos cegamente.

Entenda primeiro como o Kit espera ser instalado.

Preserve:

- `SKILL.md`;
- `references/`;
- estrutura completa das Skills;
- documentação técnica em inglês quando originalmente definida assim.

---

# 5. AGENTS

Prepare os Agents necessários para execução futura.

O workflow deve considerar pelo menos:

`Requirements Agent`

↓

`Architect Agent`

↓

`Tech Lead Agent`

↓

`Developer Agent`

↓

`Tester Agent`

↓

`Reviewer Agent`

↓

`Documentation Agent`

Os Agents devem trabalhar sobre Tasks pequenas e rastreáveis.

Nenhum Agent deve implementar o projeto nesta execução.

---

# 6. TASK-DRIVEN DEVELOPMENT

Crie uma estrutura formal de Tasks.

Sugestão:

```text
tasks/
├── backlog/
├── ready/
├── in-progress/
├── review/
├── done/
└── blocked/
```

Cada Task deverá possuir, no mínimo:

```text
ID
Title
Description
Objective
Scope
Out of Scope
Dependencies
Architecture References
Acceptance Criteria
Tests Required
Documentation Required
Branch
Status
Assigned Agent
Reviewer
Merge Target
```

Utilize IDs sequenciais.

Exemplo:

```text
TASK-001
TASK-002
TASK-003
...
```

---

# 7. GRANULARIDADE

Não crie Tasks gigantes.

Prefira:

```text
1 Task
   ↓
1 objetivo
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

Uma Task só poderá começar quando suas dependências estiverem concluídas.

---

# 8. GITFLOW

O projeto deve utilizar:

```text
main
develop
hml
```

Fluxo normal:

```text
develop
   │
   ├── feature/task-001-...
   ├── feature/task-002-...
   ├── feature/task-003-...
   └── feature/task-xxx-...
```

Cada Task deverá obrigatoriamente possuir sua própria branch:

```text
feature/task-<id>-<descricao-curta>
```

Exemplo:

```text
feature/task-001-bootstrap-documentation
```

Nunca desenvolver diretamente em:

```text
main
develop
hml
```

---

# 9. EXECUÇÃO AUTOMÁTICA DA TASK

Posteriormente, quando for autorizado iniciar a implementação, cada Task deverá executar o seguinte pipeline:

```text
Selecionar próxima Task READY
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
executar testes
        ↓
executar quality gates
        ↓
Reviewer Agent
        ↓
corrigir problemas
        ↓
Documentation Agent
        ↓
git add
        ↓
git commit
        ↓
git push
        ↓
criar Pull Request
        ↓
validação automática da IA
        ↓
merge em develop
        ↓
atualizar Task para DONE
        ↓
selecionar próxima Task
```

---

# 10. MERGE AUTOMÁTICO

O merge automático somente poderá acontecer quando TODOS os Quality Gates estiverem verdes.

Obrigatórios:

```text
Build
Tests
Architecture Validation
Code Review
Security Checks
Documentation
Acceptance Criteria
```

Se qualquer Gate falhar:

```text
NÃO FAZER MERGE
```

Mover a Task para:

```text
blocked
```

ou retornar para:

```text
in-progress
```

dependendo do problema.

Depois:

1. corrigir;
2. executar novamente;
3. revisar novamente;
4. somente então liberar o merge.

---

# 11. PROMOÇÃO

Tasks normais:

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
validação
   ↓
main
   ↓
PROD
```

Não executar uma release nesta etapa.

Apenas documentar/preparar o fluxo.

---

# 12. BACKLOG INICIAL

Analise a arquitetura `02 - dotnet - AWS` e decomponha a construção futura em Tasks.

O backlog deverá contemplar progressivamente:

### Fundação

- estrutura do repositório;
- Solution .NET;
- arquitetura;
- projetos/camadas;
- padrões;
- configurações;
- ambientes.

### Backend

- Domain;
- Application;
- Infrastructure;
- APIs;
- CQRS;
- Domain Events;
- Validation;
- Policies;
- Permissions.

### Persistência

- MySQL;
- MongoDB;
- Redis;
- migrations;
- seeds;
- fake data.

### Segurança

- JWT;
- Refresh Token;
- login;
- forgot password;
- reset password;
- roles;
- permissions.

### Mensageria

- Kafka;
- RabbitMQ;
- Outbox;
- retry;
- idempotência;
- DLQ.

### Frontend

- React Site;
- React Admin;
- autenticação;
- autorização;
- integração com APIs.

### Docker

- DEV;
- TEST;
- HML;
- PROD;
- execução automatizada de testes.

### Observabilidade

- Structured Logging;
- Correlation ID;
- OpenTelemetry;
- Tracing;
- Metrics;
- Health Checks;
- Readiness;
- Liveness.

### AWS

- SQS;
- SNS;
- Lambda;
- S3;
- EC2;
- ECS.

### Qualidade

- Unit Tests;
- Integration Tests;
- Architecture Tests;
- Security Tests;
- Quality Gates.

### Arquitetura

- C4;
- Structurizr;
- Draw.io;
- UML;
- ER;
- ADRs.

Não implemente nenhum desses itens.

Transforme-os em Tasks ordenadas e com dependências.

---

# 13. ORQUESTRADOR

Prepare/ajuste o `prompts.md` para funcionar como o orquestrador principal.

Ele deverá permitir posteriormente algo equivalente a:

```text
START
  ↓
carregar contexto
  ↓
carregar arquitetura
  ↓
carregar backlog
  ↓
identificar próxima TASK READY
  ↓
executar Agents necessários
  ↓
criar branch
  ↓
implementar
  ↓
testar
  ↓
review
  ↓
documentar
  ↓
commit
  ↓
push
  ↓
PR
  ↓
quality gates
  ↓
merge
  ↓
TASK DONE
  ↓
próxima TASK
```

Porém:

**NÃO DISPARAR ESTE LOOP NESTA EXECUÇÃO.**

---

# 14. CHECKPOINT OBRIGATÓRIO

Quando terminar o bootstrap, PARE.

Mostre:

1. arquivos criados;
2. arquivos modificados;
3. Skills instaladas;
4. Agents preparados;
5. estrutura de Tasks;
6. quantidade de Tasks geradas;
7. dependências principais;
8. estratégia GitFlow;
9. branches existentes;
10. próxima Task candidata;
11. riscos ou pendências.

Finalize explicitamente com:

`BOOTSTRAP CONCLUÍDO — IMPLEMENTAÇÃO NÃO INICIADA`

Não crie a branch da primeira Task de implementação.

Não implemente a primeira Task.

Aguarde minha autorização.