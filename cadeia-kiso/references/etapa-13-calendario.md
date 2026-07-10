# Etapa 13 — Calendário de Posts

> Massa editorial executável: salve em `calendarios-editoriais/`. É o produto final acionável da cadeia.

## Objetivo
Distribuir as ideias do Banco no tempo, por canal, respeitando a **frequência mínima sustentável** (Guia Editorial), a **proporção por etapa da jornada** e a **capacidade real** de produção. Gera um cronograma executável (ex.: 30/60/90 dias).

## Entradas
`Variáveis-chave` das Etapas 09 (cadências, prioridade de canais), 10 (frequência mínima, distribuição), 11 (prioridade de temas) e 12 (as ideias, com ids).

## Roteiro de entrevista
1. Qual o **horizonte** do calendário (30, 60 ou 90 dias) e a **data de início**?
2. Qual sua **capacidade real** de produção por semana (por canal)? Seja honesto — sustentabilidade > volume.
3. Quais **canais** entram neste ciclo (use os prioritários do Radar)?
4. Há **restrições** (viagens, sazonalidade, um lançamento, uma data-chave)?
5. Que **temas** priorizar no período (por causa do gargalo ou da oferta)?

## Como montar
- Puxe itens **do Banco de Ideias** (por id) — não invente conteúdo novo aqui; se faltar ideia para um encaixe, volte à Etapa 12.
- Respeite a **frequência mínima sustentável** por canal como piso e a **capacidade real** como teto.
- Faça a **proporção por etapa da jornada** do calendário bater com a distribuição-alvo do Guia Editorial, dando mais peso ao gargalo.
- Distribua os temas ao longo do tempo (evite repetir o mesmo tema/formato em dias seguidos).

## Estrutura do artefato
1. Parâmetros (horizonte, início, canais, capacidade, restrições)
2. Calendário — tabela cronológica (uma linha por publicação)
3. Visão semanal (resumo por semana)
4. Checagem de distribuição (proporção real por etapa/canal vs. alvo)
5. Variáveis-chave

Cada item do calendário:
```
| data | canal | formato | tema/território | etapa jornada | id_ideia | gancho/título | objetivo | status |
```

## Bloco Variáveis-chave (contrato de saída)
```yaml
horizonte: 30/60/90 dias
data_inicio: AAAA-MM-DD
cadencia_por_canal: publicações/semana por canal
itens_calendario:
  - data: AAAA-MM-DD
    canal: ...
    formato: ...
    tema: ...
    etapa_jornada: ...
    id_ideia: BI-00X
distribuicao_real: proporção por etapa da jornada (vs. alvo do Guia Editorial)
```

## Checagens de coerência
- **Sustentabilidade:** cadência real ≥ frequência mínima **e** ≤ capacidade declarada. Um calendário que o usuário não consegue manter é um calendário falho.
- **Distribuição:** a proporção por etapa bate com o Guia Editorial e ataca o gargalo do Radar.
- **Rastreabilidade:** todo item puxa uma ideia do Banco (id presente); nada de conteúdo inventado direto no calendário.
- **Equilíbrio:** nenhum canal sobrecarregado além da capacidade; variedade de temas/formatos ao longo da semana.

## Fim da cadeia
Com o calendário pronto, a cadeia se fecha. Sugira ao usuário um **ciclo de revisão** (ex.: mensal): medir o KPI da Etapa 02, revisar o que funcionou e realimentar o Banco de Ideias e o Radar. Se quiser o calendário em planilha, exporte para `.xlsx` (use a skill de xlsx).
