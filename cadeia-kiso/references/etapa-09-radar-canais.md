# Etapa 09 — Radar de Canais

## Objetivo
Diagnosticar a **etapa-gargalo da jornada** e priorizar canais via **Matriz Canal × Etapa**, definindo papéis, cadências e riscos. Decide onde investir esforço de distribuição **antes** de escrever o Guia Editorial.

## Entradas
`Variáveis-chave` de todas as etapas anteriores; especialmente 02 (objetivo/KPI), 04 (onde a persona é influenciada), 05 (posicionamento) e 08 (territórios). Veja `glossario.md` para jornada, 5S, Matriz e Score A(c).

## Roteiro de entrevista
1. Qual a **etapa-gargalo** principal e a secundária da jornada (Descoberta, Consideração, Conversão, Experiência Própria, Experiência Compartilhada) — e por quê?
2. Qual o **inventário atual** de canais e o estado de cada um (ativo, parado, consistente, novo)?
3. Em que canais o público-alvo tende a ser **influenciado**?
4. Que **pesos** atribuir a cada etapa na matriz, conforme os gargalos?
5. Para cada canal, qual o **estado mental dominante (5S)**?
6. Qual a **nota (1–5)** de cada canal por etapa da jornada?
7. Qual o **Score de adequação A(c)** e a viabilidade de cada canal?
8. Quais os canais **Top prioritários** e os de **sustentação**, com papel e cadência?
9. Qual a **cadência mínima** para os próximos 30 dias?
10. Quais os **riscos** da decisão e as mitigações? Próximos passos?

## Estrutura do artefato
1. Parte A — Diagnóstico (etapa-gargalo; leitura estratégica; inventário; canais onde o alvo é influenciado)
2. Parte B — Matriz Canal × Etapa (pesos; escala; por canal: 5S dominante, notas por etapa, Score A(c), viabilidade, leitura)
3. Parte C — Conclusões e decisões (prioridade operacional; Top prioritários; canais de sustentação)
4. Parte D — Cadência mínima dos próximos 30 dias
5. Parte E — Riscos da decisão (com mitigações)
6. Parte F — Próximos passos
7. Variáveis-chave

## Bloco Variáveis-chave (contrato de saída)
```yaml
etapa_gargalo_principal: gargalo principal da jornada
etapa_gargalo_secundaria: gargalo secundário
pesos_matriz:
  descoberta: peso
  consideracao: peso
  conversao: peso
  experiencia_propria: peso
  experiencia_compartilhada: peso
prioridade_operacional:
  - posicao: 1
    canal: nome
    score: A(c)
    cadencia: frequência
    papel: função na jornada
canais_sustentacao:
  - canal: nome
    cadencia: frequência
    papel: função
canais_nao_prioritarios: canais fora do ciclo atual
riscos_decisao: riscos identificados
proximos_passos: ações seguintes
```

## Checagens de coerência
- Reconcilie a tensão entre o canal de **maior Score A(c)** e o canal que **ataca o gargalo** declarado — a prioridade operacional pode divergir do score bruto.
- Pondere **viabilidade e hábito já existente** (um canal ótimo no papel, mas insustentável na prática, não é prioridade).
- Sinalize riscos típicos: uma marca satélite diluir a principal; um canal virar venda forçada; descoberta subir sem conversão acompanhar.

## Próxima etapa
Etapa 10 — Guia Editorial. Aprove/estabilize o Radar **antes** de escrever o Guia (o Guia depende destas decisões de canal).
