# OBS-Live-Bot — Análise, Refatoração e Padronização

Preciso que você realize uma **análise completa do projeto atualmente desenvolvido**, identifique problemas, gaps técnicos e oportunidades de melhoria e, somente depois dessa análise, execute uma **refatoração e padronização controlada**.

## 1. Projeto alvo

O projeto que deverá ser analisado e ajustado é:

```text
D:\OBS-Live\OBS-Live-Bot
```

Este é um **projeto já existente e parcialmente desenvolvido**.

Portanto:

- NÃO recrie o projeto do zero.
- NÃO substitua automaticamente a arquitetura existente.
- NÃO remova funcionalidades existentes sem justificativa.
- NÃO altere regras de negócio sem necessidade comprovada.
- NÃO copie cegamente estruturas de outros projetos.
- Primeiro compreenda o que já existe.
- Preserve funcionalidades válidas.
- Refatore apenas onde houver benefício técnico comprovado.
- Toda alteração estrutural relevante deverá ser documentada.

---

# 2. Projetos e fontes de referência

Utilize como referência de engenharia o projeto:

```text
D:\Empresa\GFMaurila\projetos\gfm-template-cms-aws
```

Utilize como fonte oficial de padrões, Agents, Skills, documentação e processo de desenvolvimento o:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev
```

O Knowledge Dictionary oficial do Kit deverá ser considerado a partir de:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

IMPORTANTE:

O `gfm-template-cms-aws` é apenas uma **referência de engenharia e organização**.

Não transforme o OBS-Live-Bot em um CMS.

Não copie regras de negócio do GFM.Template.CMS.

Não copie serviços AWS apenas porque existem no projeto de referência.

Não force tecnologias, patterns ou componentes que não façam sentido para o OBS-Live-Bot.

O projeto deverá continuar sendo:

```text
OBS-Live-Bot
```

com suas próprias:

- regras de negócio;
- funcionalidades;
- integrações;
- arquitetura;
- tecnologias;
- dependências;
- fluxos;
- configurações;
- requisitos.

O objetivo é aproveitar o **padrão de engenharia**, e não copiar o domínio do projeto de referência.

---

# 3. Objetivo principal

O objetivo é obter:

```text
OBS-Live-Bot atual
        +
análise técnica
        +
refatoração controlada
        +
Kit IA Dev
        +
padrão de engenharia do gfm-template-cms-aws
        =
OBS-Live-Bot padronizado
```

O projeto de referência deverá servir principalmente para avaliar:

```text
Estrutura
Organização
Governança
Agents
Skills
Knowledge
Quality Gates
GitFlow
Documentação
Testes
Docker
Observabilidade
Segurança
CI/CD
Automação
Processo de desenvolvimento com IA
```

---

# 4. REGRA FUNDAMENTAL — ANALISAR ANTES DE ALTERAR

Não comece refatorando arquivos imediatamente.

Execute obrigatoriamente:

```text
READ
↓
UNDERSTAND
↓
DISCOVER
↓
BASELINE
↓
COMPARE
↓
IDENTIFY GAPS
↓
PLAN
↓
CREATE REFACTOR BRANCH
↓
REFACTOR
↓
TEST
↓
VALIDATE
↓
DOCUMENT
```

Antes de qualquer alteração, faça uma fotografia técnica do estado atual do projeto.

---

# 5. Etapa 1 — Analisar o OBS-Live-Bot

Leia integralmente a estrutura relevante de:

```text
D:\OBS-Live\OBS-Live-Bot
```

Identifique pelo menos:

- linguagem;
- framework;
- versão do runtime;
- arquitetura atual;
- estrutura de diretórios;
- projetos/módulos;
- entry points;
- regras de negócio;
- integrações externas;
- integração com OBS;
- comunicação em tempo real, caso exista;
- APIs;
- workers;
- bots;
- serviços;
- banco de dados;
- persistência;
- cache;
- mensageria;
- configuração;
- secrets;
- variáveis de ambiente;
- logging;
- tratamento de erros;
- autenticação/autorização;
- testes;
- Docker;
- docker-compose;
- CI/CD;
- scripts;
- documentação;
- Git;
- branches;
- dependências;
- pacotes;
- código duplicado;
- acoplamento;
- responsabilidades misturadas;
- possíveis violações de SOLID;
- possíveis problemas de segurança;
- possíveis problemas de performance;
- dívida técnica.

Não presuma tecnologias.

Descubra primeiro o que realmente existe.

---

# 6. Etapa 2 — Ler as referências

Depois de compreender o OBS-Live-Bot, analise:

```text
D:\Empresa\GFMaurila\projetos\gfm-template-cms-aws
```

e:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev
```

Leia também integralmente o Knowledge Dictionary:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev\dicionario
```

Utilize essas fontes para identificar o padrão esperado de engenharia.

---

# 7. Etapa 3 — GAP Analysis

Compare:

```text
OBS-Live-Bot atual
        VS
gfm-template-cms-aws
        VS
Kit IA Dev
```

Crie uma análise de gaps.

Classifique cada item como:

```text
OK
MISSING
PARTIAL
NEEDS_REFACTOR
NOT_APPLICABLE
RISK
```

Para cada gap informe:

```text
Área
Estado atual
Problema
Referência utilizada
Recomendação
Prioridade
Risco
Impacto
Ação proposta
```

Não implemente componentes simplesmente porque eles existem no projeto de referência.

Quando algo não fizer sentido para o OBS-Live-Bot, classifique como:

```text
NOT_APPLICABLE
```

e explique brevemente o motivo.

---

# 8. Etapa 4 — Baseline antes da refatoração

Antes de modificar código:

1. Verifique o estado atual do Git.
2. Identifique a branch atual.
3. Verifique alterações locais não commitadas.
4. Não descarte alterações existentes.
5. Não sobrescreva trabalho do desenvolvedor.
6. Execute build do projeto.
7. Execute os testes existentes.
8. Registre falhas já existentes.
9. Diferencie erros preexistentes de erros introduzidos pela refatoração.

Crie um relatório de baseline.

Sugestão:

```text
docs/reports/BASELINE_REPORT.md
```

O relatório deverá registrar:

```text
Build antes da refatoração
Testes antes da refatoração
Warnings
Erros existentes
Dependências problemáticas
Problemas conhecidos
Dívida técnica identificada
```

---

# 9. Etapa 5 — Criar branch de refatoração

Somente depois da análise inicial e baseline, crie uma nova branch.

Utilize preferencialmente:

```text
refactor/obs-live-bot-standardization
```

A branch deverá ser criada a partir da branch de desenvolvimento correta identificada no repositório.

Se o projeto já possuir:

```text
main
develop
hml
```

respeite o GitFlow existente.

Preferencialmente:

```text
develop
   ↓
refactor/obs-live-bot-standardization
```

Se `develop` não existir, NÃO invente o fluxo silenciosamente.

Documente a situação encontrada e ajuste o GitFlow de maneira controlada.

Antes de criar a branch:

```text
git status
git branch
git branch -a
git log --oneline --decorate -n 20
```

Não execute:

```text
git reset --hard
git clean -fd
git push --force
```

sem autorização explícita.

---

# 10. Etapa 6 — Plano de refatoração

Antes de alterar o código, produza:

```text
docs/ARCHITECTURE_PLAN.md
docs/EXECUTION_PLAN.md
```

Se esses documentos já existirem, atualize-os em vez de criar versões duplicadas.

Organize a execução em tarefas pequenas.

Exemplo:

```text
TASK-001 — Baseline
TASK-002 — Estrutura
TASK-003 — Configuração
TASK-004 — Segurança
TASK-005 — Refatoração
TASK-006 — Testes
TASK-007 — Docker
TASK-008 — Observabilidade
TASK-009 — Documentação
TASK-010 — Quality Gates
```

Adapte as tasks ao que realmente for encontrado.

---

# 11. Arquitetura

Analise a arquitetura atual antes de propor mudanças.

Verifique:

- separação de responsabilidades;
- dependências entre módulos;
- baixo acoplamento;
- alta coesão;
- SOLID;
- Clean Code;
- boundaries;
- domínio;
- application/use cases;
- infraestrutura;
- adapters;
- serviços externos;
- configuração;
- abstrações;
- interfaces;
- dependency injection;
- testabilidade.

Não aplique DDD, CQRS, Clean Architecture, Vertical Slice ou qualquer outro padrão apenas porque existe nas referências.

Adote padrões somente quando trouxerem benefício real para o projeto.

Evite overengineering.

---

# 12. SOLID

Analise especificamente:

```text
S — Single Responsibility Principle
O — Open/Closed Principle
L — Liskov Substitution Principle
I — Interface Segregation Principle
D — Dependency Inversion Principle
```

Identifique violações reais no código.

Quando houver violação relevante:

```text
problema
↓
impacto
↓
solução
↓
refatoração
↓
teste
```

Não crie interfaces artificiais apenas para afirmar que o projeto utiliza SOLID.

---

# 13. Configuração e ambientes

Analise como o projeto trata configuração.

Quando aplicável, padronize ambientes equivalentes a:

```text
dev
test
hml
prod
```

Separe:

```text
configuração
↓
variáveis de ambiente
↓
secrets
```

Nenhum secret real deverá permanecer versionado.

Verifique:

- `.env`;
- `.env.example`;
- `.gitignore`;
- credentials;
- tokens;
- API keys;
- connection strings;
- certificados;
- arquivos locais.

Nunca exponha valores secretos na documentação.

---

# 14. Docker

Analise se Docker realmente faz parte ou deve fazer parte do projeto.

Quando aplicável, padronize:

```text
Dockerfile
docker-compose
healthcheck
environment
network
volumes
startup
shutdown
logs
```

Não introduza containers desnecessários.

O ambiente local deverá continuar simples de executar.

---

# 15. Observabilidade

Avalie e, quando aplicável, padronize:

```text
Structured Logging
Correlation ID
Trace ID
Metrics
Tracing
Health Checks
Readiness
Liveness
Error Handling
Audit
```

Logs não devem expor:

```text
senhas
tokens
API keys
dados sensíveis
```

---

# 16. Testes

Mapeie primeiro os testes existentes.

Depois avalie a necessidade de:

```text
Unit Tests
Integration Tests
Component Tests
E2E Tests
Smoke Tests
```

Priorize testes das regras críticas do OBS-Live-Bot.

A refatoração não poderá ser considerada concluída apenas porque o projeto compila.

Deverá haver validação funcional compatível com as funcionalidades existentes.

---

# 17. Agents

Compare os Agents existentes com o padrão do Kit IA Dev.

Quando aplicável, padronize uma estrutura equivalente a:

```text
agents/
├── requirements
├── architect
├── tech-lead
├── developer
├── tester
├── reviewer
└── documentation
```

Se o projeto utilizar:

```text
.claude/agents/
```

preserve/adapte esse padrão.

Não replique Agents redundantes.

---

# 18. Skills

Compare as Skills existentes com:

```text
D:\Empresa\GFMaurila\projetos\Kit-IA-Dev
```

Padronize somente as Skills aplicáveis ao OBS-Live-Bot.

Mantenha o padrão:

```text
SKILL.md
```

As Skills deverão representar capacidades reutilizáveis e não documentação duplicada.

---

# 19. Knowledge

Padronize o conhecimento do projeto.

Quando compatível com o Kit, utilize:

```text
docs/knowledge/
```

com documentos equivalentes a:

```text
KNOWLEDGE_DECISIONS.md
KNOWLEDGE_CONFLICTS.md
PROJECT_KNOWLEDGE_MAP.md
```

Registre decisões importantes encontradas durante a análise.

Não invente decisões arquiteturais antigas.

Quando a origem de uma decisão não puder ser determinada, marque-a como:

```text
UNKNOWN / REQUIRES VALIDATION
```

---

# 20. Quality Gates

Adapte os Quality Gates do Kit IA Dev ao OBS-Live-Bot.

Considere:

```text
Requirements Gate
Architecture Gate
Implementation Gate
Build Gate
Test Gate
Security Gate
Review Gate
Documentation Gate
Knowledge Gate
```

Nenhuma etapa deverá ser marcada como aprovada sem evidência.

---

# 21. GitFlow

Analise primeiro o GitFlow atual.

Objetivo de padronização, quando compatível:

```text
main
│
├── release/*
│
hml
│
develop
│
├── feature/*
├── fix/*
├── refactor/*
└── task/*
```

Para esta refatoração:

```text
develop
   ↓
refactor/obs-live-bot-standardization
   ↓
commits
   ↓
push
   ↓
Pull Request
   ↓
AI Code Review
   ↓
Quality Gates
   ↓
develop
```

Posteriormente, releases poderão seguir o processo oficial definido para o projeto.

Não faça merge diretamente em `main`.

Não faça push diretamente para produção.

---

# 22. Commits

Faça commits pequenos e semanticamente organizados.

Utilize Conventional Commits quando compatível:

```text
refactor:
fix:
test:
docs:
chore:
build:
ci:
perf:
```

Evite um único commit gigantesco contendo toda a padronização.

---

# 23. Segurança

Faça uma revisão específica procurando:

- secrets versionados;
- credenciais;
- tokens;
- permissões excessivas;
- entrada não validada;
- command injection;
- path traversal;
- SSRF;
- SQL injection, quando aplicável;
- XSS, quando aplicável;
- autenticação fraca;
- autorização incorreta;
- dependências vulneráveis;
- logging de informações sensíveis;
- configuração insegura;
- exposição desnecessária de portas/serviços.

Não exiba secrets encontrados na saída.

Informe apenas:

```text
tipo
arquivo
risco
ação necessária
```

mas mascare o valor.

---

# 24. Dependências

Analise:

```text
dependências utilizadas
dependências não utilizadas
dependências duplicadas
dependências obsoletas
dependências vulneráveis
versões incompatíveis
```

Não atualize indiscriminadamente todas as dependências para as versões mais recentes.

Avalie risco de breaking changes.

---

# 25. Documentação

Compare a documentação atual com o padrão do Kit IA Dev.

Quando aplicável, mantenha ou crie:

```text
README.md

docs/
├── README.md
├── architecture/
├── governance/
├── knowledge/
├── reports/
└── archive/
```

Documente pelo menos:

```text
Visão geral
Arquitetura
Como executar
Dependências
Configuração
Ambientes
Testes
Docker
Observabilidade
GitFlow
Agents
Skills
Quality Gates
Troubleshooting
```

Não crie documentação vazia apenas para reproduzir a estrutura da referência.

---

# 26. Preservação funcional

Esta é uma regra obrigatória.

Para cada refatoração relevante:

```text
Comportamento anterior
        ↓
Refatoração
        ↓
Build
        ↓
Tests
        ↓
Validação
        ↓
Comportamento equivalente ou melhoria aprovada
```

Não altere comportamento funcional silenciosamente.

Mudanças de comportamento deverão ser registradas separadamente.

---

# 27. Relatório final

Ao terminar, gere:

```text
docs/reports/REFACTOR_REPORT.md
```

Inclua:

```text
Estado inicial
Baseline
Arquitetura encontrada
Problemas encontrados
Gaps identificados
Riscos
Alterações realizadas
Arquivos criados
Arquivos alterados
Arquivos removidos
Dependências alteradas
Testes adicionados
Testes executados
Build final
Quality Gates
Débitos técnicos restantes
Recomendações futuras
```

Também gere ou atualize:

```text
docs/reports/TEST_REPORT.md
docs/reports/REVIEW_REPORT.md
```

---

# 28. Validação final

Antes de considerar o trabalho concluído, execute novamente:

```text
Build
↓
Unit Tests
↓
Integration Tests
↓
Outros testes aplicáveis
↓
Lint / Static Analysis
↓
Security Checks
↓
Docker Validation
↓
Documentation Validation
↓
Git Status
```

Compare:

```text
ANTES
VS
DEPOIS
```

O resultado deverá demonstrar melhoria mensurável.

---

# 29. O que NÃO fazer

Não:

- recriar o projeto do zero;
- transformar o OBS-Live-Bot em GFM.Template.CMS;
- copiar regras de negócio do projeto AWS;
- adicionar AWS sem necessidade;
- adicionar Azure sem necessidade;
- aplicar padrões apenas por padronização visual;
- criar abstrações inúteis;
- fazer overengineering;
- remover funcionalidades válidas;
- apagar código sem análise;
- apagar documentação útil;
- sobrescrever alterações locais;
- apagar histórico Git;
- executar force push;
- commitar secrets;
- inventar resultados de testes;
- afirmar que algo funciona sem executar validação.

---

# 30. Resultado esperado

Ao final devemos ter:

```text
OBS-Live-Bot
│
├── funcionalidades existentes preservadas
├── arquitetura compreendida e documentada
├── estrutura organizada
├── código refatorado onde necessário
├── SOLID aplicado onde fizer sentido
├── configuração padronizada
├── segurança revisada
├── testes melhorados
├── Docker padronizado, se aplicável
├── observabilidade adequada
├── Agents adequados ao projeto
├── Skills adequadas ao projeto
├── Knowledge organizado
├── Quality Gates
├── documentação atualizada
├── GitFlow definido
└── branch de refatoração isolando as alterações
```

A equação final deverá ser:

```text
OBS-Live-Bot existente
        +
preservação das regras de negócio
        +
refatoração baseada em evidências
        +
padrão de engenharia do gfm-template-cms-aws
        +
Kit IA Dev
        =
OBS-Live-Bot padronizado
```

---

# 31. REGRA DE EXECUÇÃO

Não comece alterando código.

Comece apresentando:

```text
1. PROJECT DISCOVERY
2. CURRENT ARCHITECTURE
3. BASELINE
4. GAP ANALYSIS
5. RISKS
6. REFACTORING PLAN
7. PROPOSED TASKS
8. PROPOSED BRANCH
```

Depois dessa etapa, aguarde aprovação explícita antes de executar a refatoração.

Utilize:

```text
CLIENT_APPROVAL_GATE
```

Estado inicial:

```text
CLIENT_APPROVAL_GATE: PENDING_APPROVAL
```

Quando a análise estiver concluída:

```text
ANALYSIS: COMPLETED
REFACTORING: NOT_STARTED
CLIENT_APPROVAL_GATE: PENDING_APPROVAL
```

Pare nesse ponto.

Não modifique o projeto até receber aprovação explícita para iniciar a implementação.