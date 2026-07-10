# Etapa 12 — Banco de Ideias

> Esta e a Etapa 13 são "massa editorial executável": salve-as em subpastas próprias (`bancos-de-ideias/`), separadas do núcleo estratégico (Etapas 01–11).

## Objetivo
Converter os Temas Centrais num repositório de **ideias de conteúdo executáveis** (ganchos, ângulos, formatos), organizadas por tema, território, etapa da jornada e canal — pronto para virar calendário. Aqui a cadeia sai da estratégia e entra na produção.

## Entradas
`Variáveis-chave` das Etapas 08 (territórios: dentro/fora), 10 (guia editorial: distribuição, frequência, código) e 11 (temas: prioridade, canais, jornada). Também o Radar (09) para os canais.

## Como conduzir
Diferente das etapas anteriores, esta é mais **generativa** do que de entrevista. O grosso das ideias você **gera** a partir das variáveis acumuladas; a entrevista serve para calibrar volume e coletar matéria-prima real. Depois de gerar, o usuário **cura** (mantém, corta, ajusta).

## Roteiro de entrevista (calibração)
1. Quantas ideias por tema (ou no total) você quer neste primeiro banco?
2. Que **formatos** priorizar por canal (carrossel, reel, vídeo longo, newsletter, thread, etc.)?
3. Tem **matéria-prima real** para semear ideias? (casos, histórias, bastidores, perguntas frequentes de clientes, erros comuns, dúvidas recorrentes.)
4. Algum tema que você quer **carregar** mais no começo (por causa do gargalo)?
5. Há assuntos ou abordagens **proibidos** (sensíveis, fora de compliance, fora do território)?

## Como gerar
Para cada tema priorizado (Etapa 11), gere ideias que:
- nasçam de um **território** e respeitem seu `dentro/fora`;
- cubram as **etapas da jornada** na proporção definida no Guia Editorial (mais peso no gargalo);
- casem **formato × canal × estado mental (5S)**;
- tenham um **gancho/ângulo** claro (a tensão que abre a peça) e um **objetivo cognitivo**;
- respeitem tom, código editorial e compliance.

## Estrutura do artefato
1. Como usar este banco (legenda dos campos, prioridade)
2. Ideias por tema/território — cada ideia com os campos abaixo
3. Resumo de cobertura (quantas ideias por etapa da jornada e por canal vs. a distribuição-alvo)
4. Variáveis-chave

Cada ideia:
```
- id: BI-001
  tema: <tema central>
  territorio: <território>
  etapa_jornada: Descoberta | Consideração | Conversão | Exp. Própria | Exp. Compartilhada
  canal: <canal>
  formato: <formato>
  gancho: <a tensão/ângulo que abre a peça>
  objetivo_cognitivo: <o que a pessoa deve pensar/sentir depois>
  observacao: <CTA, referência a semear, cuidado de compliance>
```

## Bloco Variáveis-chave (contrato de saída)
```yaml
total_ideias: quantidade gerada
ideias:
  - id: BI-001
    tema: ...
    territorio: ...
    etapa_jornada: ...
    canal: ...
    formato: ...
    gancho: ...
cobertura_por_etapa: nº de ideias por etapa da jornada (vs. distribuição-alvo)
cobertura_por_canal: nº de ideias por canal
```

## Checagens de coerência
- **Sem ideia órfã:** toda ideia mapeia para um Tema Central e um Território (e respeita o `fora`).
- **Cobertura proporcional:** a distribuição por etapa da jornada segue o Guia Editorial; o gargalo recebe mais ideias.
- **Formato × canal × 5S** coerentes; nada que viole tom ou compliance.
- **Teste do "sem logo":** um concorrente genérico não poderia assinar essas ideias.

## Próxima etapa
Etapa 13 — Calendário de Posts, para distribuir estas ideias no tempo de forma sustentável.
