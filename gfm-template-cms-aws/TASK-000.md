# CORREÇÃO E VALIDAÇÃO DO BOOTSTRAP

O bootstrap do Kit IA Dev foi concluído, porém precisamos executar uma etapa de **correção, validação e consolidação** antes de autorizar qualquer implementação.

## REGRA ABSOLUTA

**NÃO IMPLEMENTE O PROJETO.**

Não criar:

- `.sln`;
- `.csproj`;
- backend;
- frontend;
- APIs;
- endpoints;
- entidades;
- bancos;
- migrations;
- Docker da aplicação;
- infraestrutura AWS;
- código funcional;
- testes funcionais da aplicação;
- branch da primeira Task de implementação.

Esta execução é exclusivamente de:

```text
CORREÇÃO
+
VALIDAÇÃO
+
KNOWLEDGE CONSOLIDATION
+
BACKLOG
+
TASK PLANNING
+
DEPENDENCY GRAPH
+
GITFLOW PLANNING
```

---

# 1. CAMINHOS OFICIAIS

Utilize exatamente estes caminhos.

## Kit IA Dev

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\Kit-IA-Dev
```

## Knowledge Dictionary — SOURCE OF TRUTH

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

## Projeto

```text
D:\Empresa\GFMaurila\projetos\gfm-template-cms-aws
```

---

# 2. CORRIGIR REFERÊNCIAS AO DICIONÁRIO

O relatório anterior informou:

```text
docs/dicionario/
```

como origem dos 19 documentos.

Isso precisa ser validado.

A fonte oficial é EXCLUSIVAMENTE:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Procure referências incorretas a:

```text
docs/dicionario/
```

em arquivos como:

```text
prompts.md
CLAUDE.md
AGENTS.md
AGENTS_BOOTSTRAP.md
BOOTSTRAP_REPORT.md
PROJECT_KNOWLEDGE_MAP.md
KNOWLEDGE_DECISIONS.md
KNOWLEDGE_CONFLICTS.md
EXECUTION_PLAN.md
QUALITY_GATES.md
KNOWLEDGE_QUALITY_GATE.md
tasks/**/*.md
```

e outros arquivos relacionados.

Quando a referência significar o Knowledge Dictionary oficial, substituir pelo caminho real:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

---

# 3. NÃO DUPLICAR O SOURCE OF TRUTH

O Knowledge Dictionary deve permanecer externo ao projeto.

Portanto:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

é:

```text
SOURCE OF TRUTH
```

O projeto pode possuir:

```text
docs/
└── knowledge/
    ├── PROJECT_KNOWLEDGE_MAP.md
    ├── KNOWLEDGE_DECISIONS.md
    └── KNOWLEDGE_CONFLICTS.md
```

Esses documentos são derivados da análise do dicionário.

Eles NÃO substituem o dicionário.

A relação correta é:

```text
EXTERNAL KNOWLEDGE DICTIONARY
        ↓
PROJECT KNOWLEDGE MAP
        ↓
KNOWLEDGE DECISIONS
        ↓
REQUIREMENTS
        ↓
ARCHITECTURE
        ↓
BACKLOG
        ↓
TASKS
```

Se existir uma cópia física em:

```text
docs/dicionario/
```

não apague automaticamente.

Primeiro determine:

- quem criou;
- se existe alguma referência dependente;
- se contém conteúdo diferente;
- se é cópia integral;
- se pode causar divergência.

Registre a ocorrência em:

```text
docs/knowledge/KNOWLEDGE_CONFLICTS.md
```

A fonte externa deve continuar sendo considerada a oficial.

---

# 4. RELER O KNOWLEDGE DICTIONARY

Leia novamente TODOS os arquivos `.md` existentes em:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Não utilize somente o Knowledge Map já gerado.

Faça a validação diretamente contra os arquivos originais.

Valide a existência dos documentos esperados, incluindo o conteúdo consolidado a partir dos chats do projeto IA Claude.

---

# 5. VALIDAR KNOWLEDGE DECISIONS

Revise:

```text
docs/knowledge/PROJECT_KNOWLEDGE_MAP.md
docs/knowledge/KNOWLEDGE_DECISIONS.md
docs/knowledge/KNOWLEDGE_CONFLICTS.md
```

Cada conhecimento relevante deverá possuir uma classificação:

```text
ADOPT
ADAPT
REFERENCE
FUTURE
NOT_APPLICABLE
```

Confirme se cada decisão possui justificativa.

Não transforme automaticamente todo conteúdo do dicionário em requisito.

---

# 6. VALIDAR BASELINE 02 - DOTNET - AWS

Utilize como baseline arquitetural do projeto:

```text
02 - dotnet - AWS
```

Confirme que o planejamento contempla adequadamente:

```text
.NET
ASP.NET Core
DDD
SOLID
Clean Code
Modular Monolith
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

AWS:

```text
SQS
SNS
Lambda
S3
EC2
ECS
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

Arquitetura:

```text
C4
Structurizr DSL
Structurizr Lite
Draw.io
UML
ER
ADR
```

Estratégia:

```text
LOCAL FIRST
    ↓
CONTAINER FIRST
    ↓
CLOUD READY
    ↓
AWS TARGET
```

Não implemente esses componentes.

Use-os para validar e estruturar o backlog.

---

# 7. VALIDAR DOCUMENTAÇÃO EXISTENTE

Leia e confronte, quando existentes:

```text
README.md
PROJECT.md
PROJECT_STRUCTURE.md
PROJECT_SKILLS.md
prompts.md
CLAUDE.md
AGENTS.md
AGENTS_BOOTSTRAP.md
GITFLOW_AI_DELIVERY.md
SEED_FAKE_DATA.md
AI_CONTENT_INTELLIGENCE.md
AUDIO_INTELLIGENCE.md
ARCHITECTURE_PLAN.md
REQUIREMENTS.md
EXECUTION_PLAN.md
BOOTSTRAP_REPORT.md
```

Além de:

```text
docs/
.claude/
.github/workflows/
tasks/
```

Identifique:

```text
DUPLICATE
COMPLEMENTARY
CONFLICT
OBSOLETE
MISSING
```

Atualize:

```text
docs/knowledge/KNOWLEDGE_CONFLICTS.md
```

---

# 8. KNOWLEDGE QUALITY GATE

Execute novamente:

```text
docs/governance/KNOWLEDGE_QUALITY_GATE.md
```

Valide obrigatoriamente:

```text
[ ] Kit IA Dev analisado
[ ] Skills instaladas corretamente
[ ] Agents preparados
[ ] documentação do projeto analisada
[ ] caminho oficial do dicionário corrigido
[ ] dicionário externo lido integralmente
[ ] Knowledge Map validado
[ ] Knowledge Decisions validadas
[ ] conflitos identificados
[ ] baseline 02 - dotnet - AWS considerado
[ ] requisitos consolidados
[ ] arquitetura consolidada
[ ] nenhuma implementação iniciada
```

Se qualquer item crítico falhar:

```text
KNOWLEDGE GATE = FAILED
```

Nesse caso:

**NÃO CRIAR TASKS DE IMPLEMENTAÇÃO.**

Corrija primeiro o problema.

---

# 9. MATERIALIZAR O BACKLOG COMPLETO

Se o Knowledge Quality Gate estiver aprovado, materialize o backlog completo.

Não deixe apenas:

```text
TASK-000-BOOTSTRAP-KIT-IA-DEV
```

Crie as Tasks necessárias para construir progressivamente o projeto.

Organize por EPICs.

Exemplo:

```text
EPIC-00 — Bootstrap & Governance
EPIC-01 — Repository Foundation
EPIC-02 — Solution & Architecture
EPIC-03 — Domain Foundation
EPIC-04 — Application / CQRS
EPIC-05 — Infrastructure
EPIC-06 — Authentication & Authorization
EPIC-07 — Persistence
EPIC-08 — Cache
EPIC-09 — Messaging
EPIC-10 — Transactional Outbox
EPIC-11 — Site API
EPIC-12 — Admin API
EPIC-13 — Auth API
EPIC-14 — React Site
EPIC-15 — React Admin
EPIC-16 — Docker
EPIC-17 — Observability
EPIC-18 — Testing & QA
EPIC-19 — Architecture Documentation
EPIC-20 — AWS
EPIC-21 — CI/CD
EPIC-22 — Security
EPIC-23 — AI Content Intelligence
EPIC-24 — Audio Intelligence
EPIC-25 — Release & Deployment
```

A lista acima é referência.

Adapte conforme:

- documentação;
- dicionário;
- Knowledge Decisions;
- arquitetura;
- requisitos reais.

---

# 10. TASKS PEQUENAS E EXECUTÁVEIS

Não criar uma Task inteira para um EPIC.

Exemplo INCORRETO:

```text
TASK-010 — Implementar autenticação completa
```

Prefira decomposição:

```text
TASK-010 — Define authentication domain model
TASK-011 — Configure password hashing
TASK-012 — Implement login command
TASK-013 — Implement JWT generation
TASK-014 — Implement refresh token
TASK-015 — Implement forgot password
TASK-016 — Implement reset password
TASK-017 — Implement authorization policies
TASK-018 — Add authentication integration tests
```

Cada Task deve possuir um objetivo claramente verificável.

---

# 11. FORMATO OBRIGATÓRIO DE TASK

Cada Task deverá possuir:

```yaml
ID:
Epic:
Title:

Description:

Objective:

BusinessContext:

KnowledgeReferences:

ArchitectureReferences:

Dependencies:

Scope:

OutOfScope:

AcceptanceCriteria:

TestsRequired:

DocumentationRequired:

AssignedAgent:

Reviewer:

ArchitectureValidation:

QualityGates:

Branch:

MergeTarget: develop

Status:
```

---

# 12. KNOWLEDGE REFERENCES

Quando uma Task tiver origem no dicionário, utilizar o caminho REAL.

Exemplo:

```yaml
KnowledgeReferences:
  - D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario\11-ci-cd.md
  - D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario\20-setup-aws.md
```

Não utilizar:

```text
docs/dicionario/...
```

para representar o Knowledge Dictionary oficial.

---

# 13. DEPENDENCY GRAPH

Depois de gerar todas as Tasks, construa um grafo de dependências.

Crie:

```text
tasks/DEPENDENCY_GRAPH.md
```

Ele deve permitir visualizar:

```text
TASK-001
    ↓
TASK-002
    ↓
TASK-003
   ↙   ↘
TASK-004 TASK-005
   ↓       ↓
TASK-006 TASK-007
     ↘   ↙
     TASK-008
```

O grafo real deverá refletir as Tasks efetivamente criadas.

Não invente dependências apenas para tornar o fluxo linear.

Permita Tasks paralelas quando tecnicamente possível.

---

# 14. TASK STATUS

Utilize:

```text
BACKLOG
READY
IN_PROGRESS
REVIEW
BLOCKED
DONE
```

Uma Task somente poderá ficar:

```text
READY
```

quando todas as dependências obrigatórias estiverem:

```text
DONE
```

Como a implementação ainda NÃO começou, a maioria das Tasks deverá inicialmente estar:

```text
BACKLOG
```

Somente Tasks realmente desbloqueadas podem estar:

```text
READY
```

---

# 15. BRANCH PLANEJADA POR TASK

Toda Task de implementação deve possuir antecipadamente:

```text
feature/task-<id>-<slug>
```

Exemplo:

```text
TASK-001
feature/task-001-create-solution-structure
```

Isso é apenas planejamento.

**NÃO CRIE ESSAS BRANCHES NESTA EXECUÇÃO.**

---

# 16. GITFLOW

Branches permanentes:

```text
main
develop
hml
```

Tasks:

```text
develop
   ↓
feature/task-xxx
   ↓
commit
   ↓
push
   ↓
PR
   ↓
AI Review
   ↓
Quality Gates
   ↓
merge automático
   ↓
develop
```

Release:

```text
develop
   ↓
release/x.x.x.x
   ↓
hml
   ↓
validation
   ↓
main
   ↓
PROD
```

---

# 17. AUTO MERGE

Planeje o merge automático.

Não execute agora.

Uma Task somente poderá sofrer merge quando:

```text
Build = PASS
Unit Tests = PASS
Integration Tests = PASS
Architecture Validation = PASS
Code Review = PASS
Security Checks = PASS
Documentation = PASS
Acceptance Criteria = PASS
Knowledge Compliance = PASS
```

Se qualquer Gate falhar:

```text
NO MERGE
```

A Task deverá retornar para:

```text
IN_PROGRESS
```

ou:

```text
BLOCKED
```

---

# 18. TASK EXECUTION LOOP

Confirme que `prompts.md` e `EXECUTION_PLAN.md` estão preparados para futuramente executar:

```text
START TASK
    ↓
Load Project Context
    ↓
Load Knowledge Context
    ↓
Read Current Task
    ↓
Validate Dependencies
    ↓
Validate Knowledge References
    ↓
Checkout develop
    ↓
Pull
    ↓
Create feature/task-xxx
    ↓
Implement
    ↓
Build
    ↓
Test
    ↓
Review
    ↓
Architecture Validation
    ↓
Documentation
    ↓
Commit
    ↓
Push
    ↓
Create PR
    ↓
Quality Gates
    ↓
Auto Merge
    ↓
TASK DONE
    ↓
Next READY Task
```

Não execute esse loop nesta etapa.

---

# 19. NÃO EXECUTAR TASK-001

Mesmo que a análise determine:

```text
TASK-001 = READY
```

NÃO:

- criar branch;
- modificar código da aplicação;
- executar implementação;
- fazer commit da Task;
- fazer push da Task;
- abrir PR da Task;
- fazer merge da Task.

Apenas informe:

```text
NEXT CANDIDATE TASK: TASK-001
```

e aguarde autorização.

---

# 20. ATUALIZAR BOOTSTRAP REPORT

Atualize:

```text
BOOTSTRAP_REPORT.md
```

para refletir as correções realizadas.

O relatório deve informar explicitamente:

```text
Knowledge Dictionary Source of Truth:
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Também informar:

```text
Dictionary files read:
Knowledge Gate:
Total EPICs:
Total Tasks:
READY:
BACKLOG:
BLOCKED:
DONE:
Dependency Graph:
Planned Task Branches:
Implementation Started:
```

`Implementation Started` deverá continuar:

```text
NO
```

---

# 21. RELATÓRIO FINAL NA TELA

Ao terminar, mostre:

```text
BOOTSTRAP VALIDATION REPORT
```

contendo:

1. correções realizadas;
2. arquivos modificados;
3. caminho oficial do Knowledge Dictionary;
4. quantidade de arquivos do dicionário lidos;
5. resultado do Knowledge Quality Gate;
6. conflitos encontrados;
7. conflitos resolvidos;
8. conflitos pendentes;
9. EPICs criados;
10. quantidade total de Tasks;
11. Tasks READY;
12. Tasks BACKLOG;
13. Tasks BLOCKED;
14. Tasks DONE;
15. Dependency Graph;
16. branches planejadas;
17. próxima Task candidata;
18. motivo dela ser a próxima;
19. dependências da próxima Task;
20. confirmação de que nenhuma implementação foi iniciada.

---

# 22. CHECKPOINT FINAL

Depois do relatório:

**PARE COMPLETAMENTE.**

Finalize exatamente com:

```text
BOOTSTRAP CORRIGIDO E VALIDADO

KNOWLEDGE SOURCE OF TRUTH:
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario

KNOWLEDGE QUALITY GATE: PASSED

BACKLOG E DEPENDÊNCIAS MATERIALIZADOS

IMPLEMENTAÇÃO NÃO INICIADA

NEXT CANDIDATE TASK: TASK-XXX

AGUARDANDO AUTORIZAÇÃO PARA CRIAR A BRANCH E EXECUTAR A PRIMEIRA TASK.
```

Se o Knowledge Quality Gate não passar, substitua `PASSED` por `FAILED`, informe os motivos e NÃO selecione Task para implementação.