# Cadeia Kiso — Skill

Skill para o Claude (Cowork / Claude Code) que conduz, por **entrevista guiada etapa a etapa**, a construção de um plano de ação de estratégia de marca e conteúdo — do diagnóstico estratégico ao calendário editorial executável.

São **13 etapas encadeadas**: cada etapa termina com um bloco `Variáveis-chave` (YAML) e a etapa seguinte consome essas variáveis como entrada. É isso que torna a metodologia uma *cadeia*, e não uma lista solta de exercícios — as decisões fluem para frente.

A skill é **genérica**: funciona para qualquer profissional, negócio ou marca (inclusive posicionamento médico).

## Estrutura

```
cadeia-kiso/
├── SKILL.md                     # workflow-mestre (modo entrevista, mapa das etapas, princípios)
└── references/
    ├── etapa-01-diagnostico.md
    ├── etapa-02-objetivo.md
    ├── etapa-03-icp.md
    ├── etapa-04-persona.md
    ├── etapa-05-posicionamento.md
    ├── etapa-06-brand-persona.md
    ├── etapa-07-manifesto.md
    ├── etapa-08-territorios.md
    ├── etapa-09-radar-canais.md
    ├── etapa-10-guia-editorial.md
    ├── etapa-11-temas-centrais.md
    ├── etapa-12-banco-de-ideias.md
    ├── etapa-13-calendario.md
    ├── glossario.md             # conceitos próprios (Needscope, arquétipos, 5S, Score A(c), etc.)
    └── modelo-artefato.md       # molde padrão de todo artefato de etapa
```

## As 13 etapas

| # | Etapa | Produz |
|---|-------|--------|
| 01 | Diagnóstico Estratégico | retrato do negócio, diferencial, ambição, exclusões |
| 02 | Objetivo Estratégico | momento, objetivo de 3–6 meses, KPI, viabilidade |
| 03 | ICP | perfil de cliente ideal e anti-ICP |
| 04 | Persona Estratégica | decisor simbólico: dores, desejos, decisão, linguagem |
| 05 | Posicionamento Estratégico | categoria, inimigo, promessa, diferencial, bandeira |
| 06 | Brand Persona | território motivacional, arquétipo, tom de voz |
| 07 | Manifesto de Marca | núcleo ideológico + manifesto público |
| 08 | Territórios de Marca | 3–6 lentes temáticas duradouras (dentro/fora) |
| 09 | Radar de Canais | etapa-gargalo + canais priorizados e cadências |
| 10 | Guia Editorial | regras de conteúdo por etapa da jornada e por canal |
| 11 | Temas Centrais | temas recorrentes por território, priorizados |
| 12 | Banco de Ideias | repositório de ideias executáveis por tema/canal |
| 13 | Calendário de Posts | cronograma editorial sustentável (30/60/90 dias) |

## Como instalar

**Via pacote `.skill` (recomendado):** empacote a pasta `cadeia-kiso/` como um arquivo `.skill` e, no Claude, clique em **Salvar skill** ou vá em **Ajustes › Capacidades**.

Para (re)empacotar a partir do fonte, basta zipar a pasta com a extensão `.skill`:

```bash
cd cadeia-kiso-skill
zip -r cadeia-kiso.skill cadeia-kiso
```

## Como usar

Depois de instalada, é só pedir ao Claude algo como: *"monta o plano de ação (Cadeia Kiso) para [marca/profissional]"* ou *"continua a cadeia a partir da etapa X"*. A skill assume a condução, uma etapa por vez, sempre fechando com as `Variáveis-chave` e confirmando antes de avançar.

## Notas

- As **etapas 12 e 13** (Banco de Ideias e Calendário) foram reconstruídas a partir da lógica da cadeia; ajuste-as se você tiver uma versão-fonte própria.
- Metodologia proprietária **Cadeia Kiso**. Sem arquivo de licença, valem os direitos reservados por padrão — adicione uma licença se quiser abrir o uso.
