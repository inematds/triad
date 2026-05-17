# TRIAD — Curso Completo: Implementação Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Criar o curso completo "TRIAD — Automação de IA Multi-Modelo com Hermes Agent" em formato INEMA.CLUB, publicado no GitHub Pages, com 4 trilhas, 24 módulos e landing page.

**Architecture:** Estrutura de arquivos HTML estáticos seguindo o design system INEMA.CLUB (Tailwind CDN, dark/light mode, cores por trilha). Cada trilha tem um index com cards de módulos e navegação rápida. Cada módulo tem mínimo 6 tópicos com 3 seções cada. A landing page apresenta o curso e as 4 trilhas com CTAs.

**Tech Stack:** HTML5, Tailwind CSS (CDN), Inter font (Google Fonts), JavaScript vanilla (theme toggle, modais, expansores de tópico). Referência de template: `/home/nmaldaner/projetos/intelecto-curso/`. Skill de formato: `formato-curso` (MASTER_COMPLETO.md).

**Referência obrigatória antes de implementar:** Ler `/home/nmaldaner/.claude/skills/formato-curso/references/MASTER_COMPLETO.md` e `CHECKLIST_REVISAO.md`.

---

## Estrutura de Arquivos

```
/home/nmaldaner/projetos/triad/
├── index.html                          # Landing page do curso
└── curso/
    ├── index.html                      # Índice geral (4 trilhas)
    ├── trilha1/                        # FUNDAMENTOS (Emerald)
    │   ├── index.html
    │   ├── modulo-1-1.html             # O que é Hermes Agent
    │   ├── modulo-1-2.html             # O problema de um único modelo
    │   ├── modulo-1-3.html             # O Sistema Triad
    │   ├── modulo-1-4.html             # soul.md — Memória persistente
    │   ├── modulo-1-5.html             # OpenRouter — Hub de modelos
    │   └── modulo-1-6.html             # DeepSeek V4 — Executor de baixo custo
    ├── trilha2/                        # IMPLEMENTAÇÃO TÉCNICA (Blue)
    │   ├── index.html
    │   ├── modulo-2-1.html             # Configurando o ambiente Hermes
    │   ├── modulo-2-2.html             # Conectando OpenRouter
    │   ├── modulo-2-3.html             # Integrando DeepSeek V4
    │   ├── modulo-2-4.html             # Gemini CLI multimodal
    │   ├── modulo-2-5.html             # Criando a skill Orpheus
    │   └── modulo-2-6.html             # soul.md na prática
    ├── trilha3/                        # AVANÇADO (Purple)
    │   ├── index.html
    │   ├── modulo-3-1.html             # Engenharia de prompts do Triad
    │   ├── modulo-3-2.html             # Controle de custos e rate limits
    │   ├── modulo-3-3.html             # Monitoramento e saúde do sistema
    │   ├── modulo-3-4.html             # Segurança — Chaves e dados sensíveis
    │   ├── modulo-3-5.html             # Resiliência — Fallbacks e erros
    │   └── modulo-3-6.html             # Expandindo o Pantheon
    └── trilha4/                        # CONSTRUÇÃO E ESCALA (Amber)
        ├── index.html
        ├── modulo-4-1.html             # Arquitetura completa do sistema
        ├── modulo-4-2.html             # Construindo o Pantheon visual
        ├── modulo-4-3.html             # Automação overnight
        ├── modulo-4-4.html             # Integrações externas
        ├── modulo-4-5.html             # Deploy técnico — GitHub Pages
        └── modulo-4-6.html             # Onboarding para não-técnicos
```

**Total: 31 arquivos HTML**

---

## Conteúdo das Trilhas e Módulos

### TRILHA 1 — FUNDAMENTOS (Emerald)
*"Entenda a lógica do Hermes, do Triad e do sistema"*

**M1.1 — O que é Hermes Agent — O agente que aprende com você**
Tópicos (mín. 6):
1. Hermes vs ferramentas comuns de IA — qual a diferença real
2. Persistência — por que importa que o agente lembre
3. Hermes vs Claude Code — papéis distintos, objetivos distintos
4. Como Hermes aprende com cada tarefa
5. Agendamento em background — trabalhe enquanto você dorme
6. O modelo profundo de quem você é — e por que isso muda tudo
7. Casos de uso reais — o que você pode delegar hoje

**M1.2 — O problema de um único modelo — Por que múltiplos cérebros importam**
Tópicos:
1. Viés de confirmação em modelos únicos — o que acontece
2. Por que um modelo não consegue criticar a si mesmo
3. Diferentes arquiteturas, diferentes pontos cegos
4. Pesquisa: Reflexion e multi-agent critique
5. O custo de decisões ruins por falta de revisão
6. O princípio WD-40 — melhoria por loops rápidos
7. Como o Triad resolve o problema de viés único

**M1.3 — O Sistema Triad — Planeje, Execute, Critique**
Tópicos:
1. Visão geral do fluxo: Condutor → Executor → Crítico
2. Opus como Condutor — interrogar, briefar, validar
3. DeepSeek como Executor — volume, custo, resiliência
4. GPT-5.5 como Crítico — rigor, especificidade, aprovação
5. O loop interno DeepSeek ↔ GPT — até o SHIP
6. Por que os modelos devem ser de arquiteturas diferentes
7. Exemplo prático — escolha de nicho de negócio

**M1.4 — soul.md — A memória persistente do seu agente**
Tópicos:
1. O que é o soul.md e por que ele existe
2. Identity — nome, localização, papel, canais públicos
3. Mission & Goals — objetivo do ano, pilares, fora de escopo
4. Business — receita, custos, runway, equipe, métricas
5. Voice — como falar com você, como escrever como você
6. Hard nos — limites que o agente nunca pode cruzar
7. Rhythm — janelas de foco, dias de criação, curva de energia
8. Memory — decisões, pessoas, ferramentas, lições por trimestre

**M1.5 — OpenRouter — Um hub para todos os modelos**
Tópicos:
1. O problema de gerenciar múltiplas APIs
2. Como o OpenRouter funciona — uma chave, todos os modelos
3. Dashboard de custos e rastreamento de uso
4. Roteamento automático — :nitro, :floor, :auto
5. Bring Your Own Keys — integrando sua chave da DeepSeek
6. Fallbacks — resiliência quando um modelo falha
7. Zero completion fee — o que isso significa na prática

**M1.6 — DeepSeek V4 — O executor de alto desempenho e baixo custo**
Tópicos:
1. Por que DeepSeek V4 é diferente dos outros modelos baratos
2. Benchmarks comparativos — o que os números dizem
3. 95% do valor por 1% do preço — a aritmética do custo
4. $0,87 vs $75 por milhão de tokens — impacto real
5. Por que barato significa "executar por horas sem culpa"
6. Casos onde DeepSeek V4 brilha e onde não usar
7. DeepSeek V4 no fluxo Triad — o papel de executor

---

### TRILHA 2 — IMPLEMENTAÇÃO TÉCNICA (Blue)
*"Aprenda e aplique o conhecimento técnico para fazer a solução funcionar"*

**M2.1 — Configurando o ambiente Hermes**
Tópicos:
1. Pré-requisitos — o que você precisa antes de começar
2. Instalação do Hermes Agent — passo a passo
3. Configuração inicial — diretórios, permissões, variáveis
4. Primeiro teste — confirmar que Hermes está funcionando
5. O dashboard do Hermes — visão geral da interface
6. Conectando Claude Code ao Hermes — integração
7. Verificação de saúde — checklist pós-instalação

**M2.2 — Conectando OpenRouter — Chaves, dashboard e roteamento**
Tópicos:
1. Criando sua conta no OpenRouter
2. Gerando a API key principal
3. Configurando OpenRouter no Hermes (`hermes setup model`)
4. Testando a conexão — chamada de verificação
5. Navegando o dashboard — uso, custos, modelos disponíveis
6. Selecionando modelos padrão para cada papel do Triad
7. Troubleshooting — erros comuns e soluções

**M2.3 — Integrando DeepSeek V4 como Worker do Triad**
Tópicos:
1. Por que ter chave própria da DeepSeek no OpenRouter
2. Criando conta e carregando créditos na DeepSeek Platform
3. Gerando API key da DeepSeek
4. Adicionando a chave no OpenRouter (Bring Your Own Keys)
5. Configurando DeepSeek como modelo Worker no Hermes
6. Testando o Worker — tarefa simples ponta a ponta
7. Monitorando uso e custo no primeiro ciclo real

**M2.4 — Gemini CLI — Capacidade multimodal no terminal**
Tópicos:
1. O que é CLI e por que o Gemini CLI é poderoso
2. Instalando o Gemini CLI — clonando o repositório
3. Autenticando com sua conta Google
4. Comandos básicos — primeiras chamadas no terminal
5. Conectando o Gemini CLI ao Hermes como ferramenta
6. Caso de uso: analisar vídeo/imagem via Hermes
7. Expandindo para GitHub CLI, OpenAI CLI e outros

**M2.5 — Criando a skill Orpheus — Seu deep work agent**
Tópicos:
1. O que é uma skill no Hermes e como funciona
2. O Pantheon — o painel de personas e skills
3. Criando a persona Orpheus no Pantheon
4. Os três system prompts do Triad — Conductor, Worker, Critic
5. Sincronizando Orpheus com o Hermes via prompt
6. Testando Orpheus com uma tarefa real
7. Ajustando e refinando a persona após o primeiro uso

**M2.6 — soul.md na prática — Preenchendo e ativando**
Tópicos:
1. Baixando e abrindo o template soul.md
2. Preenchendo Identity e Mission com seus dados reais
3. Documentando seu negócio — receita, custos, métricas
4. Definindo sua voz e seus hard nos
5. Mapeando seu ritmo de trabalho — janelas, dias, energia
6. Registrando decisões, pessoas e ferramentas na seção Memory
7. Fazendo Hermes carregar o soul.md — verificação final

---

### TRILHA 3 — AVANÇADO (Purple)
*"Técnicas, otimização, manutenção e segurança"*

**M3.1 — Engenharia de prompts para o Triad**
Tópicos:
1. Por que o prompt do Condutor define tudo
2. Estrutura do briefing ideal — o que não pode faltar
3. Como formular critérios de sucesso claros
4. Instruções para o Worker — ângulos, volume, paralelismo
5. Calibrando o Crítico — o que "brutalmente criticar" significa
6. Fallbacks no prompt — "se tokens acabarem, default para X"
7. Iterando os prompts — como medir e melhorar

**M3.2 — Controle de custos e gestão de rate limits**
Tópicos:
1. Entendendo tokens — input vs output, cache vs fresh
2. Como calcular custo antes de rodar uma tarefa pesada
3. Rate limits — o que são, quando acontecem, como evitar
4. Estratégias de orçamento por modelo e por semana
5. Alertas de custo no OpenRouter — configurando limites
6. Quando usar free tier vs pago — a decisão certa
7. Otimizando prompts para reduzir tokens sem perder qualidade

**M3.3 — Monitoramento, logs e saúde do sistema**
Tópicos:
1. O que monitorar em um sistema Hermes ativo
2. Logs nativos do Hermes — onde ficam e como ler
3. Dashboard do OpenRouter como painel de saúde
4. Alertas de falha — configurando notificações
5. Revisão diária — o ritual de 5 minutos para saber o que aconteceu
6. Detectando tarefas presas ou loops infinitos
7. Documentando o histórico de decisões do agente

**M3.4 — Segurança — Chaves de API e dados sensíveis**
Tópicos:
1. O risco real de vazar chaves de API
2. Nunca colocar chaves no soul.md — alternativas seguras
3. Variáveis de ambiente — como usar corretamente
4. Rotação de chaves — quando e como trocar
5. Permissões mínimas — dando ao agente apenas o que precisa
6. O que o Hermes pode ver — e o que você nunca deve mostrar
7. Checklist de segurança antes de deixar o agente em produção

**M3.5 — Resiliência — Fallbacks e recuperação de erros**
Tópicos:
1. O que acontece quando um modelo falha ou fica lento
2. Configurando fallbacks no OpenRouter
3. Fallbacks no prompt — instruções defensivas para o Worker
4. Limites de retry — quantas vezes tentar antes de parar
5. Checkpoints — salvando estado parcial em tarefas longas
6. Recuperação manual — como retomar uma tarefa interrompida
7. Testando resiliência — simulando falhas para verificar os fallbacks

**M3.6 — Expandindo o Pantheon — Novas personas e skills**
Tópicos:
1. Quando criar uma nova persona vs usar Orpheus
2. Mapeando seus tipos de trabalho — quais precisam de persona própria
3. Criando uma persona de pesquisa de mercado
4. Criando uma persona de geração de conteúdo
5. Criando uma persona de análise técnica de código
6. Gerenciando múltiplas personas — nomenclatura e organização
7. Compartilhando personas com sua equipe — exportar e importar

---

### TRILHA 4 — CONSTRUÇÃO E ESCALA (Amber)
*"Passo a passo da construção e geração de um sistema para implementar em escala"*

**M4.1 — Arquitetura completa do sistema Hermes + Triad**
Tópicos:
1. Mapa do sistema — todos os componentes e conexões
2. Hermes como orquestrador central — o que ele controla
3. OpenRouter como camada de abstração de modelos
4. soul.md como fonte única de contexto pessoal
5. O Pantheon como interface de controle de personas
6. Gemini CLI como ferramenta multimodal no ecossistema
7. Fluxo completo de uma tarefa do início ao fim
8. Pontos de extensão — onde o sistema pode crescer

**M4.2 — Construindo o Pantheon visual — Dashboard de personas**
Tópicos:
1. O que é o Pantheon e por que ter uma interface visual
2. Estrutura do dashboard — personas, skills, histórico, spend
3. Adicionando personas pelo painel — passo a passo
4. Editando e versionando system prompts de personas
5. Conectando o Pantheon ao Hermes via prompt de sincronização
6. Integrando dados do Claude Code ao Pantheon
7. Customizando o dashboard para o seu fluxo de trabalho

**M4.3 — Automação overnight — Agendando trabalho pesado**
Tópicos:
1. O que pode ser feito enquanto você dorme — exemplos reais
2. Configurando jobs recorrentes no Hermes
3. Definindo entradas e saídas esperadas para jobs overnight
4. Gerenciando memória para tarefas longas — checkpoints
5. Revisão matinal — o protocolo de conferir o que foi feito
6. Combinando Hermes com N8N para automações externas
7. Criando um loop de melhoria contínua — cada tarefa ensina

**M4.4 — Integrações externas — Telegram, N8N, Zapier**
Tópicos:
1. Por que integrar Hermes com ferramentas externas
2. Telegram como canal de comunicação com o Hermes
3. Configurando um bot Telegram para receber tarefas
4. N8N como orquestrador de automações — visão geral
5. Conectando Hermes ao N8N via webhook
6. Zapier para usuários não-técnicos — alternativa simples
7. Criando um pipeline: Telegram → Hermes → Triad → resposta

**M4.5 — Deploy técnico — GitHub Pages e distribuição**
Tópicos:
1. Preparando o repositório para produção
2. Configurando GitHub Pages — branch e diretório raiz
3. Estrutura de arquivos para deploy correto
4. Automatizando deploy com GitHub Actions
5. Versionamento do sistema — tags e releases
6. Distribuindo para uma equipe — guia de onboarding técnico
7. Monitorando uso após o deploy — métricas de adoção

**M4.6 — Onboarding para não-técnicos — Templates e guias**
Tópicos:
1. O desafio de escalar para usuários não-técnicos
2. Simplificando o soul.md — versão para não-técnicos
3. Criando um guia de primeiro uso passo a passo
4. Templates de personas prontas para copiar e usar
5. FAQ — as 10 dúvidas mais comuns de usuários novos
6. Suporte e escalada — quando chamar o técnico
7. Medindo adoção — como saber se o onboarding funcionou

---

## Tasks de Implementação

### Task 0: Setup do projeto e leitura de referências

**Files:**
- Read: `/home/nmaldaner/.claude/skills/formato-curso/references/MASTER_COMPLETO.md`
- Read: `/home/nmaldaner/.claude/skills/formato-curso/references/CHECKLIST_REVISAO.md`
- Create dirs: `triad/curso/trilha1/`, `trilha2/`, `trilha3/`, `trilha4/`

- [ ] Ler MASTER_COMPLETO.md completo (seções 3, 5, 6, 7, 8, 9, 10)
- [ ] Ler CHECKLIST_REVISAO.md
- [ ] Criar estrutura de diretórios:
```bash
mkdir -p /home/nmaldaner/projetos/triad/curso/trilha1
mkdir -p /home/nmaldaner/projetos/triad/curso/trilha2
mkdir -p /home/nmaldaner/projetos/triad/curso/trilha3
mkdir -p /home/nmaldaner/projetos/triad/curso/trilha4
```
- [ ] Verificar checklist crítico do formato-curso antes de iniciar qualquer página

---

### Task 1: Landing Page — `index.html` (raiz do projeto)

**Files:**
- Create: `/home/nmaldaner/projetos/triad/index.html`

**Conteúdo:**
- Hero: "TRIAD — Automação de IA Multi-Modelo com Hermes Agent"
- Subtítulo: "Aprenda a construir um sistema de IA que trabalha por você 24/7, usando múltiplos modelos no papel certo para cada tarefa."
- 4 cards de trilha com cor, título, descrição e CTA para `curso/trilha1/index.html` etc.
- Seção "O que você vai construir" com o diagrama do sistema
- Seção "Para quem é" (iniciantes → avançados → times técnicos)
- Footer com link INEMA.CLUB (`text-sky-400`)
- Dark/light mode toggle

- [ ] Criar `index.html` seguindo base HTML da Sec. 8 do MASTER
- [ ] Adicionar hero section com gradiente e logo TRIAD
- [ ] Adicionar 4 cards de trilha (cores: emerald, blue, purple, amber)
- [ ] Verificar: link INEMA.CLUB presente com `text-sky-400`
- [ ] Verificar: theme toggle funcionando
- [ ] Verificar checklist completo antes de marcar como done

---

### Task 2: Curso Index — `curso/index.html`

**Files:**
- Create: `/home/nmaldaner/projetos/triad/curso/index.html`

**Conteúdo:**
- Header: "TRIAD — Trilhas de Aprendizado"
- Grid 2×2 com os 4 cards de trilha (cada com descrição, módulos listados, CTA)
- Cada card clicável → `trilha1/index.html` etc.
- Barra de progresso visual (decorativa)
- Dark/light mode, link INEMA.CLUB

- [ ] Criar `curso/index.html` com grid de 4 trilhas
- [ ] Verificar botões com `justify-start`
- [ ] Verificar link INEMA.CLUB

---

### Task 3: Trilha 1 Index — `curso/trilha1/index.html`

**Files:**
- Create: `/home/nmaldaner/projetos/triad/curso/trilha1/index.html`

**Conteúdo:**
- Cor: Emerald (`text-emerald-400`)
- Título: "Trilha 1 — Fundamentos"
- Subtítulo: "Entenda a lógica do Hermes, do Triad e do sistema"
- Navegação rápida (grid compacto de 6 cards-âncora) — OBRIGATÓRIA
- 6 cards de módulo expandíveis com tópicos colapsáveis
- Cada card com botão "Ver Completo" → `modulo-1-X.html`
- Dark/light mode, link INEMA.CLUB

- [ ] Criar `trilha1/index.html` com cor emerald
- [ ] Adicionar navegação rápida antes do "Conteúdo detalhado" — OBRIGATÓRIA
- [ ] Adicionar 6 módulos com tópicos expansíveis (mín. 6 tópicos cada)
- [ ] Verificar botão "Ver Completo" em CADA card
- [ ] Verificar checklist completo

---

### Task 4: Módulos da Trilha 1 (M1.1 a M1.6)

**Files:**
- Create: `curso/trilha1/modulo-1-1.html` através de `modulo-1-6.html`

Para cada módulo, seguir estrutura:
- Header: título do módulo + trilha emerald
- Breadcrumb: Curso > Trilha 1 > Módulo X
- Mínimo 6 tópicos expansíveis
- Cada tópico: número em círculo + 3 seções ("O que é / Por que aprender / Conceitos-chave")
- Navegação prev/next entre módulos
- Botão "Voltar à Trilha" → `index.html`
- Modal com `<iframe>` se necessário
- Dark/light mode, link INEMA.CLUB

- [ ] Criar `modulo-1-1.html` (O que é Hermes Agent — 7 tópicos)
- [ ] Criar `modulo-1-2.html` (O problema de um único modelo — 7 tópicos)
- [ ] Criar `modulo-1-3.html` (O Sistema Triad — 7 tópicos)
- [ ] Criar `modulo-1-4.html` (soul.md — 8 tópicos)
- [ ] Criar `modulo-1-5.html` (OpenRouter — 7 tópicos)
- [ ] Criar `modulo-1-6.html` (DeepSeek V4 — 7 tópicos)
- [ ] Verificar checklist em cada módulo antes de marcar como done

---

### Task 5: Trilha 2 Index + Módulos (M2.1 a M2.6)

**Files:**
- Create: `curso/trilha2/index.html` + `modulo-2-1.html` a `modulo-2-6.html`

**Conteúdo:** Cor Blue. Foco técnico. Incluir blocos de código onde relevante (instalação de CLI, configuração de chaves, comandos de terminal). Estilo visual diferenciado para código (`font-mono`, `bg-dark-700`).

- [ ] Criar `trilha2/index.html` com cor blue e navegação rápida
- [ ] Criar `modulo-2-1.html` (Configurando ambiente Hermes)
- [ ] Criar `modulo-2-2.html` (Conectando OpenRouter)
- [ ] Criar `modulo-2-3.html` (Integrando DeepSeek V4)
- [ ] Criar `modulo-2-4.html` (Gemini CLI)
- [ ] Criar `modulo-2-5.html` (Criando skill Orpheus — incluir os 3 system prompts completos do Triad)
- [ ] Criar `modulo-2-6.html` (soul.md na prática — incluir template completo)
- [ ] Verificar checklist em cada arquivo

---

### Task 6: Trilha 3 Index + Módulos (M3.1 a M3.6)

**Files:**
- Create: `curso/trilha3/index.html` + `modulo-3-1.html` a `modulo-3-6.html`

**Conteúdo:** Cor Purple. Foco avançado. Incluir exemplos de configuração, código de monitoramento, checklists de segurança. Tom mais técnico e denso.

- [ ] Criar `trilha3/index.html` com cor purple e navegação rápida
- [ ] Criar `modulo-3-1.html` (Engenharia de prompts)
- [ ] Criar `modulo-3-2.html` (Controle de custos)
- [ ] Criar `modulo-3-3.html` (Monitoramento)
- [ ] Criar `modulo-3-4.html` (Segurança)
- [ ] Criar `modulo-3-5.html` (Resiliência)
- [ ] Criar `modulo-3-6.html` (Expandindo o Pantheon)
- [ ] Verificar checklist em cada arquivo

---

### Task 7: Trilha 4 Index + Módulos (M4.1 a M4.6)

**Files:**
- Create: `curso/trilha4/index.html` + `modulo-4-1.html` a `modulo-4-6.html`

**Conteúdo:** Cor Amber. Foco em construção e escala. Incluir diagramas (SVG ou ASCII), checklists de deploy, templates prontos para copy-paste. Módulo M4.6 deve ser acessível para não-técnicos — linguagem mais simples.

- [ ] Criar `trilha4/index.html` com cor amber e navegação rápida
- [ ] Criar `modulo-4-1.html` (Arquitetura completa — incluir diagrama SVG do sistema)
- [ ] Criar `modulo-4-2.html` (Pantheon visual)
- [ ] Criar `modulo-4-3.html` (Automação overnight)
- [ ] Criar `modulo-4-4.html` (Integrações externas)
- [ ] Criar `modulo-4-5.html` (Deploy GitHub Pages — incluir workflow YAML do Actions)
- [ ] Criar `modulo-4-6.html` (Onboarding não-técnicos — linguagem simplificada)
- [ ] Verificar checklist em cada arquivo

---

### Task 8: Revisão Final e Checklist Global

- [ ] Abrir cada página no browser e verificar dark/light mode
- [ ] Verificar todos os links internos (prev/next, "Ver Completo", "Voltar à Trilha")
- [ ] Confirmar que TODAS as páginas têm link INEMA.CLUB com `text-sky-400`
- [ ] Confirmar navegação rápida em todos os 4 index de trilha
- [ ] Confirmar mínimo 6 tópicos em todos os 24 módulos
- [ ] Confirmar 3 seções por tópico em todos os módulos
- [ ] Confirmar botões com `justify-start` (não `justify-center`)
- [ ] Confirmar números em círculo (não setas `▶`)
- [ ] Verificar responsividade mobile em cada página
- [ ] Preparar para deploy no GitHub Pages

---

## Notas de Implementação

**Conteúdo base disponível:**
- `doc/soul.md` — template completo do soul.md com todos os campos e o fluxo Triad com system prompts
- Transcrição do vídeo — narrativa completa do sistema e casos de uso
- Infográficos em `doc/` — referência visual para diagramas

**Os 3 system prompts do Triad** (usar no M2.5 e M4.1):
- Conductor (Opus): interrogar → briefar → validar, nunca executar o trabalho
- Worker (DeepSeek): 3-5 ângulos, loop com Critic até SHIP
- Critic (GPT-5.5): VERDICT (SHIP/REVISE/FUNDAMENTAL FLAW) + WHAT BREAKS + WHAT'S MISSING + BEST ANGLE

**Comparativo de custo a incluir:**
- DeepSeek V4: $0,87/M tokens out
- Claude Opus 4.7: $75/M tokens out
- Relação: ~100x mais barato, ~95% do valor para trabalho pesado

**Referência de projeto:** `/home/nmaldaner/projetos/intelecto-curso/` para estrutura e padrões HTML.
