Você vai me ajudar a instalar o Kit IA Dev no meu projeto. Fale em português do Brasil.

Contexto:
- Pacotes baixados: Kit IA Dev, Templates por Stack, Skills Avançadas.
- Ferramenta que eu uso: outra ferramenta de IA de código.
- Caminho típico de skills: pergunte à ferramenta onde colocar pastas no padrão Agent Skills (SKILL.md), ou use `3-Skills/COMO-INSTALAR.md`.

Pastas/zips que eu estou passando (ou vou passar) como contexto:
- Pasta do Kit descompactada: `Kit-IA-Dev/` (ou o zip `Kit-IA-Dev.zip` anexado no chat)
- Pasta do SEU projeto (raiz do repositório onde a IA vai instalar)
- Pacote Templates: pasta descompactada `Order-Bump-Templates-por-Stack/` OU zip `Kit-IA-Dev-Templates-por-Stack.zip`
- Pacote Skills Avançadas: pasta `Upsell1-Kit-IA-Dev/` OU zip `Kit-IA-Dev-Skills-Avancadas.zip`

Se algum desses contextos estiver faltando, peça o caminho absoluto ou o anexo do zip antes de copiar arquivos.

Regras da sua condução:
- Um passo de cada vez. Espere eu confirmar antes do próximo.
- Não explique a arquitetura do produto; faça eu concluir o setup.
- Se algo for ambíguo (stack, pasta do projeto, ferramenta), pergunte em 1–2 perguntas curtas.
- Conteúdo técnico dos arquivos (CLAUDE.md, agent_docs, SKILL.md) permanece em inglês; conversa comigo em PT-BR.

Plano que você deve executar comigo:
1) Confirmar que você consegue ver o kit (e os outros pacotes marcados) + a raiz do meu projeto.
2) Template: como eu tenho Templates por Stack, perguntar qual stack (Next.js, Node API, React Native/Expo, Python, Monorepo, Microsserviços, PHP/Laravel). Copiar ESSA pasta de template para a raiz do projeto (não misturar com o template genérico).
   Se a stack não estiver nas 7, usar o template genérico em `Kit-IA-Dev/2-CLAUDE-md-Template/`.
3) Rodar a entrevista de preenchimento: ler o bloco SETUP NOTE do CLAUDE.md, verificar versões atuais da stack na web se possível, preencher os [FILL], apagar o comentário SETUP quando terminar. Se eu uso ferramenta além do Claude Code, seguir o multi-tool setup (AGENTS.md etc.).
4) Instalar as 10 skills do Kit (`3-Skills/`): copiar cada PASTA inteira (SKILL.md + references/). Caminho: pergunte à ferramenta onde colocar pastas no padrão Agent Skills (SKILL.md), ou use `3-Skills/COMO-INSTALAR.md`.
5) Skills Avançadas: instalar as 8 pastas novas; depois SUBSTITUIR os 8 SKILL.md em `2-Atualizacoes-Skills-Existentes/` por cima das skills do kit (code-review e frontend-design não têm patch).
6) Validar com um pedido óbvio (ex.: "revisa esse código" / "escreve o commit" / "isso está lento") e confirmar que a skill certa ativou.

Comece agora pela etapa 1. Se o kit/projeto ainda não estiver no contexto, peça o anexo ou o caminho absoluto antes de qualquer cópia de arquivo.