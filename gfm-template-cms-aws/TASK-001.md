# REORGANIZAÇÃO DA DOCUMENTAÇÃO — GFM.TEMPLATE.CMS AWS

Você vai reorganizar a documentação existente do projeto para reduzir arquivos `.md` soltos na raiz e estabelecer uma estrutura documental definitiva.

Fale comigo em **português do Brasil**.

## REGRA PRINCIPAL

Esta execução é exclusivamente de:

```text
DOCUMENTATION REORGANIZATION
+
REFERENCE UPDATE
+
>VALIDATION
```

**NÃO EXECUTE NENHUMA TASK DE IMPLEMENTAÇÃO.**

Não criar backend, frontend, `.sln`, `.csproj`, APIs, bancos, Docker da aplicação ou infraestrutura AWS.

Não executar `TASK-001`.

---

# 1. PROJETO

Raiz oficial:

```text
D:\Empresa\GFMaurila\projetos\gfm-template-cms-aws
```

Kit IA Dev:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\Kit-IA-Dev
```

Knowledge Dictionary — Source of Truth externo:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

O Knowledge Dictionary NÃO deve ser movido nem duplicado.

---

# 2. OBJETIVO

A raiz do projeto deve permanecer limpa.

Ao finalizar, manter na raiz principalmente:

```text
gfm-template-cms-aws/
├── .claude/
├── .github/
├── config/
├── docs/
├── tasks/
├── .gitignore
├── README.md
└── prompts.md
```

## EXCEÇÕES

`README.md` deve permanecer na raiz porque é o entry point humano.

`prompts.md` deve permanecer na raiz porque é o entry point/orquestrador principal da IA.

Não mover esses dois arquivos.

---

# 3. ESTRUTURA DOCUMENTAL DESEJADA

Organize `docs/` desta forma:

```text
docs/
│
├── ai/
│   ├── AI_CONTENT_INTELLIGENCE.md
│   └── AUDIO_INTELLIGENCE.md
│
├── architecture/
│   ├── PROJECT_STRUCTURE.md
│   └── diagrams/
│
├── governance/
│   ├── AGENTS_BOOTSTRAP.md
│   ├── GITFLOW_AI_DELIVERY.md
│   ├── EXECUTION_PLAN.md
│   ├── QUALITY_GATES.md
│   └── KNOWLEDGE_QUALITY_GATE.md
│
├── knowledge/
│   ├── PROJECT_KNOWLEDGE_MAP.md
│   ├── KNOWLEDGE_DECISIONS.md
│   └── KNOWLEDGE_CONFLICTS.md
│
├── project/
│   ├── PROJECT_SKILLS.md
│   └── SEED_FAKE_DATA.md
│
├── reports/
│   └── BOOTSTRAP_REPORT.md
│
└── archive/
    └── prompts.md.bootstrap-backup
```

Não recrie arquivos que já estejam corretamente posicionados.

Crie somente os diretórios necessários.

---

# 4. MOVIMENTAÇÕES

Mover:

```text
AI_CONTENT_INTELLIGENCE.md
```

para:

```text
docs/ai/AI_CONTENT_INTELLIGENCE.md
```

Mover:

```text
AUDIO_INTELLIGENCE.md
```

para:

```text
docs/ai/AUDIO_INTELLIGENCE.md
```

Mover:

```text
PROJECT_STRUCTURE.md
```

para:

```text
docs/architecture/PROJECT_STRUCTURE.md
```

Mover:

```text
AGENTS_BOOTSTRAP.md
```

para:

```text
docs/governance/AGENTS_BOOTSTRAP.md
```

Mover:

```text
GITFLOW_AI_DELIVERY.md
```

para:

```text
docs/governance/GITFLOW_AI_DELIVERY.md
```

Mover:

```text
PROJECT_SKILLS.md
```

para:

```text
docs/project/PROJECT_SKILLS.md
```

Mover:

```text
SEED_FAKE_DATA.md
```

para:

```text
docs/project/SEED_FAKE_DATA.md
```

Mover:

```text
BOOTSTRAP_REPORT.md
```

para:

```text
docs/reports/BOOTSTRAP_REPORT.md
```

Mover:

```text
prompts.md.bootstrap-backup
```

para:

```text
docs/archive/prompts.md.bootstrap-backup
```

---

# 5. DOCUMENTOS QUE JÁ ESTÃO EM DOCS

Preserve os documentos já existentes em:

```text
docs/knowledge/
docs/governance/
```

Não sobrescreva conteúdo válido.

Preserve especialmente:

```text
docs/knowledge/PROJECT_KNOWLEDGE_MAP.md
docs/knowledge/KNOWLEDGE_DECISIONS.md
docs/knowledge/KNOWLEDGE_CONFLICTS.md

docs/governance/EXECUTION_PLAN.md
docs/governance/QUALITY_GATES.md
docs/governance/KNOWLEDGE_QUALITY_GATE.md
```

---

# 6. ATUALIZAR TODAS AS REFERÊNCIAS

Após mover os arquivos, faça uma busca global no repositório.

Atualize TODAS as referências aos caminhos antigos.

Procure principalmente em:

```text
README.md
prompts.md

.claude/**
.github/**
config/**
docs/**
tasks/**
```

Além de qualquer outro arquivo textual existente no repositório.

---

# 7. MAPEAMENTO DE CAMINHOS

Utilize:

```text
AGENTS_BOOTSTRAP.md
→ docs/governance/AGENTS_BOOTSTRAP.md

GITFLOW_AI_DELIVERY.md
→ docs/governance/GITFLOW_AI_DELIVERY.md

PROJECT_STRUCTURE.md
→ docs/architecture/PROJECT_STRUCTURE.md

PROJECT_SKILLS.md
→ docs/project/PROJECT_SKILLS.md

SEED_FAKE_DATA.md
→ docs/project/SEED_FAKE_DATA.md

AI_CONTENT_INTELLIGENCE.md
→ docs/ai/AI_CONTENT_INTELLIGENCE.md

AUDIO_INTELLIGENCE.md
→ docs/ai/AUDIO_INTELLIGENCE.md

BOOTSTRAP_REPORT.md
→ docs/reports/BOOTSTRAP_REPORT.md

prompts.md.bootstrap-backup
→ docs/archive/prompts.md.bootstrap-backup
```

---

# 8. CUIDADO COM REFERÊNCIAS

Não faça substituição cega de strings quando o nome estiver sendo usado como conceito e não como caminho.

Exemplo:

```text
Leia PROJECT_STRUCTURE.md
```

deve virar:

```text
Leia docs/architecture/PROJECT_STRUCTURE.md
```

Mas um texto histórico que apenas menciona o nome do documento pode não precisar ser alterado.

Analise o contexto.

---

# 9. PROMPTS.MD

`prompts.md` deve continuar na raiz.

Revise-o cuidadosamente.

Ele deverá carregar documentos utilizando os novos caminhos.

Por exemplo:

```text
docs/architecture/PROJECT_STRUCTURE.md
docs/project/PROJECT_SKILLS.md
docs/project/SEED_FAKE_DATA.md
docs/governance/AGENTS_BOOTSTRAP.md
docs/governance/GITFLOW_AI_DELIVERY.md
docs/governance/EXECUTION_PLAN.md
docs/governance/QUALITY_GATES.md
docs/governance/KNOWLEDGE_QUALITY_GATE.md
docs/knowledge/PROJECT_KNOWLEDGE_MAP.md
docs/knowledge/KNOWLEDGE_DECISIONS.md
docs/knowledge/KNOWLEDGE_CONFLICTS.md
docs/ai/AI_CONTENT_INTELLIGENCE.md
docs/ai/AUDIO_INTELLIGENCE.md
```

Preserve o Knowledge Dictionary externo:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Não trocar esse caminho por algo dentro de `docs/`.

---

# 10. AGENTS E SKILLS

Verifique:

```text
.claude/agents/
.claude/skills/
```

Caso algum Agent ou Skill faça referência aos documentos movidos, atualize o caminho.

Não alterar o comportamento das Skills.

Não modificar conteúdo técnico sem necessidade.

O objetivo aqui é somente corrigir referências documentais.

---

# 11. TASKS

Faça busca completa em:

```text
tasks/
```

Atualize `KnowledgeReferences`, `ArchitectureReferences` e demais referências documentais.

Exemplo:

ANTES:

```yaml
ArchitectureReferences:
  - PROJECT_STRUCTURE.md
```

DEPOIS:

```yaml
ArchitectureReferences:
  - docs/architecture/PROJECT_STRUCTURE.md
```

Não alterar:

- ID da Task;
- objetivo;
- dependências;
- status;
- branch planejada;
- acceptance criteria;

exceto quando alguma referência documental precisar ser corrigida.

---

# 12. KNOWLEDGE DICTIONARY

A fonte oficial continua sendo:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Nunca substituir referências a essa fonte externa por:

```text
docs/dicionario/
```

ou qualquer outra pasta local.

O relacionamento continua:

```text
EXTERNAL KNOWLEDGE DICTIONARY
        ↓
docs/knowledge/
        ↓
Requirements
        ↓
Architecture
        ↓
Backlog
        ↓
Tasks
```

---

# 13. CRIAR ÍNDICE DA DOCUMENTAÇÃO

Crie:

```text
docs/README.md
```

Esse arquivo deve funcionar como índice documental do projeto.

Estrutura sugerida:

```markdown
# Project Documentation

## Architecture
- PROJECT_STRUCTURE
- Diagrams

## Governance
- Agents Bootstrap
- GitFlow AI Delivery
- Execution Plan
- Quality Gates
- Knowledge Quality Gate

## Knowledge
- Project Knowledge Map
- Knowledge Decisions
- Knowledge Conflicts

## AI
- AI Content Intelligence
- Audio Intelligence

## Project
- Project Skills
- Seed Fake Data

## Reports
- Bootstrap Report

## Tasks
See ../tasks/

## External Knowledge Dictionary
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Utilize links relativos corretos entre os documentos internos.

---

# 14. ATUALIZAR README PRINCIPAL

Mantenha:

```text
README.md
```

na raiz.

Adicione ou ajuste uma seção curta:

```markdown
## Documentation

Project documentation is organized under:

`docs/`

Documentation index:

`docs/README.md`

AI orchestration entry point:

`prompts.md`
```

Não transformar o README principal em índice de todos os documentos.

`docs/README.md` será responsável por isso.

---

# 15. VALIDAR LINKS E REFERÊNCIAS

Depois da reorganização, execute uma busca global procurando pelos caminhos antigos.

Procure por referências que ainda apontem incorretamente para:

```text
AGENTS_BOOTSTRAP.md
AI_CONTENT_INTELLIGENCE.md
AUDIO_INTELLIGENCE.md
BOOTSTRAP_REPORT.md
GITFLOW_AI_DELIVERY.md
PROJECT_SKILLS.md
PROJECT_STRUCTURE.md
SEED_FAKE_DATA.md
prompts.md.bootstrap-backup
```

Diferencie:

```text
filename mention
```

de:

```text
file path reference
```

Não deve restar nenhuma referência operacional apontando para um local antigo.

---

# 16. VALIDAR ESTRUTURA FINAL

A estrutura esperada deve ficar aproximadamente:

```text
gfm-template-cms-aws/
│
├── .claude/
│   ├── agents/
│   └── skills/
│
├── .github/
│
├── config/
│
├── docs/
│   ├── README.md
│   │
│   ├── ai/
│   │   ├── AI_CONTENT_INTELLIGENCE.md
│   │   └── AUDIO_INTELLIGENCE.md
│   │
│   ├── architecture/
│   │   ├── PROJECT_STRUCTURE.md
│   │   └── diagrams/
│   │
│   ├── governance/
│   │   ├── AGENTS_BOOTSTRAP.md
│   │   ├── GITFLOW_AI_DELIVERY.md
│   │   ├── EXECUTION_PLAN.md
│   │   ├── QUALITY_GATES.md
│   │   └── KNOWLEDGE_QUALITY_GATE.md
│   │
│   ├── knowledge/
│   │   ├── PROJECT_KNOWLEDGE_MAP.md
│   │   ├── KNOWLEDGE_DECISIONS.md
│   │   └── KNOWLEDGE_CONFLICTS.md
│   │
│   ├── project/
│   │   ├── PROJECT_SKILLS.md
│   │   └── SEED_FAKE_DATA.md
│   │
│   ├── reports/
│   │   └── BOOTSTRAP_REPORT.md
│   │
│   └── archive/
│       └── prompts.md.bootstrap-backup
│
├── tasks/
│   ├── backlog/
│   ├── ready/
│   ├── in-progress/
│   ├── review/
│   ├── blocked/
│   ├── done/
│   └── DEPENDENCY_GRAPH.md
│
├── .gitignore
├── README.md
└── prompts.md
```

---

# 17. NÃO ALTERAR O BACKLOG FUNCIONAL

Esta reorganização NÃO é uma Task funcional do produto.

Não:

```text
executar TASK-001
```

Não promover automaticamente:

```text
TASK-001 → READY
```

Não criar:

```text
feature/task-001-...
```

Não iniciar o loop de desenvolvimento.

O backlog funcional deve permanecer intacto.

---

# 18. GIT

Você pode preparar as alterações no working tree.

Porém, nesta execução:

- não criar branch de implementação;
- não criar Pull Request de implementação;
- não fazer merge da TASK-001;
- não marcar TASK-001 como DONE.

Se houver política existente que exija registrar alterações de bootstrap/documentação, siga a governança existente sem confundir essa reorganização com uma Task funcional.

---

# 19. VALIDAÇÃO FINAL

Antes de concluir, valide:

```text
[ ] README.md permanece na raiz
[ ] prompts.md permanece na raiz
[ ] demais documentos foram organizados em docs/
[ ] docs/README.md foi criado
[ ] referências internas foram atualizadas
[ ] prompts.md aponta para os novos caminhos
[ ] Agents apontam para os novos caminhos
[ ] Tasks apontam para os novos caminhos
[ ] Knowledge References continuam corretas
[ ] caminho externo do dicionário continua correto
[ ] links relativos internos estão válidos
[ ] nenhum documento foi perdido
[ ] nenhuma Task funcional foi executada
[ ] nenhuma branch da TASK-001 foi criada
[ ] nenhuma implementação foi iniciada
```

---

# 20. RELATÓRIO FINAL

Ao terminar, apresente:

```text
DOCUMENTATION REORGANIZATION REPORT

Moved:
- ...

Created:
- ...

Updated References:
- ...

Unchanged:
- README.md
- prompts.md

External Knowledge Source:
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario

Broken References:
- 0 expected

TASK-001:
- NOT STARTED

Implementation:
- NOT STARTED
```

Mostre também a árvore final:

```text
gfm-template-cms-aws/
...
```

---

# 21. CHECKPOINT

Depois da reorganização:

**PARE.**

Não execute a próxima Task.

Finalize com:

```text
DOCUMENTATION REORGANIZATION COMPLETED

ROOT CLEANED AND DOCUMENTATION ORGANIZED

README.md: ROOT
prompts.md: ROOT

KNOWLEDGE SOURCE OF TRUTH:
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario

REFERENCES VALIDATED

TASK-001 NOT STARTED

IMPLEMENTATION NOT STARTED

WAITING FOR AUTHORIZATION TO EXECUTE TASK-001.
```