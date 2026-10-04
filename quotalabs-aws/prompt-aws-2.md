# QUOTA LABS AWS — COMPLETAR SETUP BASE AWS

O setup anterior ficou incompleto.

Você executou corretamente o planejamento e parou no `CLIENT_APPROVAL_GATE`, porém agora deve **completar a configuração estrutural do projeto**, reproduzindo TODA a configuração-base definida para o modelo AWS utilizado como referência.

## PROJETO

Raiz:

```text
D:\Empresa\GFMaurila\projetos\quotalabs-aws
```

## REGRA PRINCIPAL

Faça uma auditoria do setup atual e complete tudo que estiver faltando em relação ao padrão AWS definido anteriormente.

Esta execução é de:

```text
SETUP
CONFIGURATION
DOCUMENTATION
KNOWLEDGE
AGENTS
SKILLS
PROJECT GOVERNANCE
AI ORCHESTRATION
```

NÃO é autorização para implementar as tasks funcionais do produto.

As tasks continuam:

```text
PENDING_CLIENT_APPROVAL
```

E o gate continua:

```text
CLIENT_APPROVAL_GATE = PENDING_APPROVAL
```

---

# 1. AUDITAR O SETUP ATUAL

Analise recursivamente:

```text
D:\Empresa\GFMaurila\projetos\quotalabs-aws
```

Identifique o que já existe e o que ainda está faltando.

NÃO apague nem sobrescreva conteúdo válido sem necessidade.

Use:

```text
READ
COMPARE
MERGE
UPDATE
VALIDATE
```

e não:

```text
DELETE
RECREATE EVERYTHING
```

---

# 2. KIT IA DEV

Utilize como fonte oficial:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev
```

Confirme a instalação e configuração das skills necessárias.

O projeto já reportou:

```text
.claude/skills/
10 skills instaladas
```

Valide se cada skill possui sua estrutura completa:

```text
skill-name/
├── SKILL.md
└── references/
```

Corrija instalações incompletas.

---

# 3. KNOWLEDGE DICTIONARY

ATENÇÃO: ALTERAÇÃO EM RELAÇÃO À EXECUÇÃO ANTERIOR.

A execução anterior apenas LEU externamente:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Agora o projeto também deverá possuir sua própria cópia controlada desse conhecimento.

A fonte original deve permanecer intacta.

NUNCA mova ou apague os arquivos da origem.

Copie os arquivos necessários para uma área de conhecimento do projeto, preferencialmente:

```text
D:\Empresa\GFMaurila\projetos\quotalabs-aws\docs\knowledge\
```

Estrutura sugerida:

```text
docs/
└── knowledge/
    └── dicionario/
        ├── *.md
        └── ...
```

Fonte:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Destino:

```text
D:\Empresa\GFMaurila\projetos\quotalabs-aws\docs\knowledge\dicionario
```

IMPORTANTE:

- copiar;
- não mover;
- não modificar a fonte;
- preservar nomes;
- preservar conteúdo;
- preservar estrutura quando houver subpastas;
- não resumir os arquivos durante a cópia.

Depois valide:

```text
SOURCE FILE COUNT
DESTINATION FILE COUNT
MISSING FILES
EXTRA FILES
COPY ERRORS
```

Os 19 arquivos previamente encontrados devem ser conferidos.

---

# 4. KNOWLEDGE-FIRST LOCAL

A partir desta configuração, os agentes do projeto devem saber que existe uma Knowledge Base local em:

```text
docs/knowledge/dicionario/
```

Antes de atividades importantes de:

```text
Requirements
Architecture
Planning
Backlog
Task Planning
Development
Testing
Review
Documentation
DevOps
Cloud
AI/RAG
```

os agentes devem consultar o conhecimento aplicável.

Atualize as instruções necessárias para registrar essa regra.

---

# 5. CLAUDE.md

Localize o `CLAUDE.md` existente.

Compare com o padrão utilizado pelo setup AWS.

Garanta que ele documente:

```text
Project Context
Project Structure
Technology Stack
Architecture Rules
Coding Rules
Knowledge Rules
Agent Rules
Skill Rules
Testing Rules
Security Rules
Git Rules
AWS Rules
Docker Rules
Documentation Rules
Quality Gates
Client Approval Gate
```

Não substitua conteúdo específico do Quota Labs por conteúdo genérico.

Faça merge das regras.

---

# 6. AGENTS.md

Caso exista ou seja necessário para o ambiente utilizado, configure:

```text
AGENTS.md
```

Ele deverá orientar agentes sobre:

```text
Knowledge First
Requirements
Architecture
Development
Testing
Review
Documentation
Security
DevOps
AWS
Quality Gates
```

E obrigatoriamente:

```text
NO IMPLEMENTATION WITHOUT CLIENT APPROVAL
```

---

# 7. AGENTES

Valide/configure os agentes utilizados pelo Kit IA Dev.

Considere:

```text
Requirements Agent
Architect Agent
Tech Lead Agent
Developer Agent
Tester Agent
Reviewer Agent
Documentation Agent
Security Agent
DevOps Agent
```

Enquanto:

```text
CLIENT_APPROVAL_GATE = PENDING_APPROVAL
```

aplique:

```text
Developer Agent
= PLANNING ONLY

Tester Agent
= TEST PLANNING ONLY

DevOps Agent
= INFRASTRUCTURE PLANNING ONLY

Reviewer Agent
= DOCUMENTATION / ARCHITECTURE REVIEW
```

---

# 8. ORQUESTRAÇÃO

Garanta que o projeto tenha um fluxo claro:

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
ARCHITECTURE
      ↓
BACKLOG
      ↓
TASK DECOMPOSITION
      ↓
TASK READINESS
      ↓
CLIENT APPROVAL GATE
      ↓
IMPLEMENTATION
```

Neste momento:

```text
CLIENT APPROVAL GATE
        ↓
PENDING_APPROVAL
        ↓
STOP
```

---

# 9. DOCUMENTAÇÃO DO PROJETO

Audite `docs/`.

Preserve a documentação existente do Quota Labs.

Garanta organização para:

```text
docs/
├── requirements/
├── architecture/
├── backlog/
├── tasks/
├── testing/
├── security/
├── observability/
├── aws/
├── adr/
├── knowledge/
│   └── dicionario/
└── references/
    └── screens/
```

Não crie diretórios vazios apenas para satisfazer essa árvore se já existir uma organização equivalente.

Adapte ao projeto existente.

---

# 10. REFERÊNCIAS VISUAIS

Preserve integralmente:

```text
docs/references/screens/
```

Principalmente as referências do portal jurídico/LawFirm.

As referências visuais são parte da fonte de requisitos do projeto.

Não renomeie ou reorganize imagens sem necessidade.

---

# 11. ARQUITETURA AWS

Garanta que a documentação registre o princípio:

```text
LOCAL FIRST
CONTAINER FIRST
CLOUD READY
AWS TARGET
```

E considere, conforme aplicável:

```text
SQS
SNS
Lambda
S3
EC2
ECS
```

Além da infraestrutura local correspondente.

Não implemente infraestrutura AWS nesta execução.

---

# 12. DOCKER / AMBIENTE LOCAL

Audite a preparação para:

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

Documente gaps.

Não transforme gaps em implementação automática.

---

# 13. ARQUITETURA

Preserve e consolide:

```text
DDD
CQRS
Vertical Slice
SOLID
Clean Code
Domain Events
Infrastructure Abstractions
Dependency Injection
```

Não refatore código nesta execução.

---

# 14. IA / INTAKE JURÍDICO

Preserve o contexto específico do Quota Labs:

```text
texto
áudio
mensagens
documentos
        ↓
Intake
        ↓
Processing
        ↓
Transcription
        ↓
Analysis
        ↓
Summary
        ↓
Legal Workflow
```

Isso pertence à arquitetura/requisitos.

NÃO implemente essa feature agora.

---

# 15. GIT / GOVERNANÇA

Documente/valide o fluxo Git adotado pelo projeto.

Quando aplicável:

```text
main
develop
hml
```

Fluxo:

```text
develop
   ↓
feature/task-XXX
   ↓
PR
   ↓
develop
   ↓
hml
   ↓
release/x.y.z
   ↓
main
```

Não crie branches de feature nesta execução.

---

# 16. TASKS

Não execute nenhuma task preparada anteriormente.

Todas continuam:

```text
PENDING_CLIENT_APPROVAL
```

É permitido ajustar documentação da task caso a auditoria do setup identifique informações ausentes.

Não alterar para:

```text
IN_PROGRESS
```

---

# 17. VALIDAR PARIDADE DO SETUP

Ao terminar, produza uma matriz:

```text
COMPONENT                         STATUS

Kit IA Dev                       OK/MISSING
Skills                           OK/MISSING
Agents                           OK/MISSING
CLAUDE.md                        OK/MISSING
AGENTS.md                        OK/MISSING
Knowledge Dictionary             OK/MISSING
Knowledge Local Copy             OK/MISSING
Knowledge Rules                  OK/MISSING
Documentation                    OK/MISSING
Architecture                     OK/MISSING
AWS Planning                     OK/MISSING
Docker Planning                  OK/MISSING
Security                         OK/MISSING
Observability                    OK/MISSING
Testing                          OK/MISSING
Git Governance                   OK/MISSING
References/Screens               OK/MISSING
Backlog                          OK/MISSING
Tasks                            OK/MISSING
Client Approval Gate             OK/MISSING
```

Corrija itens de SETUP que estiverem `MISSING`.

Não corrija itens que representem implementação de feature.

---

# 18. VALIDAR O DICIONÁRIO

Apresente explicitamente:

```text
KNOWLEDGE DICTIONARY VALIDATION

Source:
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario

Destination:
D:\Empresa\GFMaurila\projetos\quotalabs-aws\docs\knowledge\dicionario

Source files: XX
Destination files: XX
Missing: XX
Errors: XX

Result: PASS/FAIL
```

Não considere concluído se arquivos esperados estiverem faltando.

---

# 19. RESULTADO FINAL

O relatório final deverá mostrar:

```text
============================================================
QUOTA LABS AWS — AWS BASE SETUP SYNCHRONIZATION
============================================================

Project Audit ................... PASS
Kit IA Dev ...................... PASS
Skills .......................... PASS
Agents .......................... PASS
Knowledge Dictionary ............ PASS
Knowledge Local Copy ............ PASS
Documentation ................... PASS
Architecture Configuration ...... PASS
AWS Configuration Planning ...... PASS
Docker Configuration Planning ... PASS
Security Rules .................. PASS
Observability Rules ............. PASS
Testing Rules ................... PASS
Git Governance .................. PASS
Visual References ............... PASS

Backlog ......................... PREPARED
Tasks ........................... PENDING_CLIENT_APPROVAL

Implementation .................. NOT STARTED
Client Approval Gate ............ PENDING_APPROVAL

============================================================
STOP CONDITION REACHED
============================================================

AWS base setup synchronized.

Knowledge Dictionary copied and validated.

No product implementation task was started.

WAITING FOR EXPLICIT CLIENT APPROVAL.
============================================================
```

---

# REGRA FINAL

Esta autorização serve para:

```text
CONFIGURAR
COPIAR CONHECIMENTO
INSTALAR SKILLS
CONFIGURAR AGENTES
ORGANIZAR DOCUMENTAÇÃO
ATUALIZAR INSTRUÇÕES
VALIDAR SETUP
```

Ela NÃO serve para:

```text
IMPLEMENTAR BACKLOG
EXECUTAR TASK
CRIAR FEATURE
ALTERAR REGRA DE NEGÓCIO
FAZER DEPLOY
CRIAR RELEASE
```

Execute agora a sincronização completa do setup.

Ao terminar:

```text
CLIENT_APPROVAL_GATE = PENDING_APPROVAL
```

e PARE.