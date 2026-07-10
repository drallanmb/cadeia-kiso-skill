---
name: cadeia-kiso
description: >-
  Metodologia Cadeia Kiso — conduz, por entrevista guiada etapa a etapa, a
    construção de um plano de ação de estratégia de marca e conteúdo, do
      diagnóstico estratégico ao calendário editorial executável. São 13 etapas
        encadeadas em que cada etapa consome as "Variáveis-chave" das anteriores.
          Use SEMPRE que o usuário quiser montar, estruturar ou revisar posicionamento
            de marca, autoridade, plano de conteúdo ou plano de ação estratégico para um
              profissional, negócio ou marca (inclusive posicionamento médico/profissional),
                ou quando mencionar: Cadeia Kiso, etapa Kiso, diagnóstico estratégico,
                  objetivo estratégico, ICP, persona estratégica, posicionamento estratégico,
                    brand persona, manifesto de marca, territórios de marca, radar de canais,
                      guia editorial, temas centrais, banco de ideias ou calendário de posts.
                        Use também quando pedirem para "continuar a cadeia", "avançar uma etapa",
                          ou gerar/revisar qualquer um desses artefatos.
                          ---

                          # Cadeia Kiso

                          A Cadeia Kiso é uma **metodologia encadeada** que transforma um profissional, negócio ou marca — de um diagnóstico estratégico inicial até um calendário editorial pronto para executar. São **13 etapas em sequência**. O que torna isto uma *cadeia*, e não uma lista solta de exercícios, é o **contrato de dados**: cada etapa termina com um bloco `Variáveis-chave` (YAML), e a etapa seguinte **consome** essas variáveis como entrada. Nada é decidido do zero duas vezes; cada decisão flui para frente.

                          Esta skill é **genérica**: funciona para qualquer marca ou profissional. Onde um exemplo ajuda, use um marcador neutro entre colchetes (ex.: `[segmento]`, `[categoria de mercado]`), nunca um caso real embutido.

                          ## Como esta skill opera: entrevista guiada, etapa a etapa

                          O modo padrão é **entrevista**. O material desta metodologia nasce de perguntas bem feitas, não de suposições. Para **cada** etapa, siga este ciclo:

                          1. **Anuncie a etapa** e diga, em uma frase, o que ela vai produzir e por quê.
                          2. **Carregue a referência** da etapa em `references/etapa-NN-*.md` e siga o roteiro de lá.
                          3. **Reancore nas entradas.** Releia (dos arquivos já salvos ou da conversa) as `Variáveis-chave` que esta etapa consome e resuma-as em 2–4 linhas antes de perguntar qualquer coisa. Isto mantém a cadeia coerente.
                          4. **Entreviste.** Faça as perguntas do roteiro **em blocos pequenos** (2 a 4 por vez), como uma conversa — não despeje o questionário inteiro. Aprofunde onde a resposta for rasa. Se o usuário não souber algo, registre `[LACUNA: ...]` em vez de inventar.
                          5. **Sintetize o artefato** no formato de `references/modelo-artefato.md`, usando as seções específicas da etapa.
                          6. **Feche com o bloco `Variáveis-chave`** (YAML) — o contrato que alimenta a próxima etapa. É obrigatório; sem ele a cadeia quebra.
                          7. **Rode as checagens de coerência** da etapa e sinalize contradições com etapas anteriores antes de seguir.
                          8. **Salve o arquivo** (ver "Onde salvar") e **confirme com o usuário** antes de avançar. O usuário pode pedir para ir mais rápido, gerar um rascunho para ele editar, ou pular uma etapa — respeite, mas avise quando pular uma etapa deixar a próxima sem uma entrada necessária.

                          Se o usuário quiser começar e não disser onde está, ofereça começar pela **Etapa 01 — Diagnóstico Estratégico**. Se ele já tem artefatos prontos de etapas anteriores, peça para colá-los (ou aponte os arquivos) e retome da etapa seguinte, extraindo as `Variáveis-chave` do que já existe.

                          ## As 13 etapas

                          | # | Etapa | Consome (entradas) | Produz (essência) | Referência |
                          |---|-------|--------------------|-------------------|------------|
                          | 01 | Diagnóstico Estratégico | — (entrevista inicial) | retrato do negócio, diferencial, ambição, exclusões | `references/etapa-01-diagnostico.md` |
                          | 02 | Objetivo Estratégico | 01 | momento, objetivo de 3–6 meses, KPI, viabilidade | `references/etapa-02-objetivo.md` |
                          | 03 | ICP | 01, 02 | perfil de cliente ideal e anti-ICP | `references/etapa-03-icp.md` |
                          | 04 | Persona Estratégica | 03 | decisor simbólico: dores, desejos, decisão, linguagem | `references/etapa-04-persona.md` |
                          | 05 | Posicionamento Estratégico | 01, 03, 04 | categoria, inimigo, promessa, diferencial, bandeira | `references/etapa-05-posicionamento.md` |
                          | 06 | Brand Persona | 05, 03, 04 | território motivacional, arquétipo, tom de voz | `references/etapa-06-brand-persona.md` |
                          | 07 | Manifesto de Marca | 01, 03, 04, 05, 06 | núcleo ideológico + manifesto público | `references/etapa-07-manifesto.md` |
                          | 08 | Territórios de Marca | 01, 03, 04, 05, 06, 07 | 3–6 lentes temáticas duradouras (dentro/fora) | `references/etapa-08-territorios.md` |
                          | 09 | Radar de Canais | 02, 04, 05, 08 (todas) | etapa-gargalo + canais priorizados e cadências | `references/etapa-09-radar-canais.md` |
                          | 10 | Guia Editorial | 05, 06, 07, 08, 09 (todas) | regras de conteúdo por etapa da jornada e por canal | `references/etapa-10-guia-editorial.md` |
                          | 11 | Temas Centrais | 08, 09, 10 (todas) | temas recorrentes por território, priorizados | `references/etapa-11-temas-centrais.md` |
                          | 12 | Banco de Ideias | 08, 10, 11 | repositório de ideias executáveis por tema/canal | `references/etapa-12-banco-de-ideias.md` |
                          | 13 | Calendário de Posts | 09, 10, 11, 12 | cronograma editorial sustentável (30/60/90 dias) | `references/etapa-13-calendario.md` |

                          Conceitos próprios do método (jornada de 5 etapas, Needscope, arquétipos, 5S, Score A(c), Matriz Canal × Etapa, teste do "sem logo", etapa-gargalo) estão definidos em `references/glossario.md`. Leia-o na primeira vez que um conceito aparecer.

                          ## Princípios inegociáveis da cadeia

                          - **O contrato manda.** Toda etapa consome `Variáveis-chave` anteriores e entrega as suas. Se uma entrada estiver faltando, resolva a etapa que falta antes (ou registre `[LACUNA: ...]` e siga com cautela).
                          - **Não invente dados.** Preço, faturamento, concorrentes, números — só entram se vierem do usuário. Onde faltar, use `[LACUNA: ...]`. É melhor uma lacuna explícita do que um número inventado que contamina todas as etapas seguintes.
                          - **Coerência antes de avançar.** Cada etapa tem checagens próprias (ex.: promessa sustentável? território sem sobreposição? cadência é viável?). Rode-as e mostre as tensões ao usuário.
                          - **Nunca prometa resultado garantido.** A metodologia constrói autoridade de substância, não hype. Evite linguagem de garantia ("resultado certo", "sucesso garantido").
                          - **Respeite o setor.** Em domínios regulados (saúde, jurídico, financeiro), aplique as regras de compliance que aparecem no Guia Editorial e não produza conteúdo que viole normas do conselho/categoria.
                          - **Teste do "sem logo".** Territórios, temas e conteúdo devem ser reconhecíveis como *desta* marca mesmo sem assinatura. Se qualquer concorrente genérico pudesse ter dito o mesmo, refine.

                          ## Modelo de artefato

                          Todo artefato de etapa segue o mesmo formato — cabeçalho, corpo em seções, bloco `Variáveis-chave`, alertas de coerência e próxima etapa. O molde completo está em `references/modelo-artefato.md`. Use-o sempre para que os documentos fiquem consistentes e legíveis pela própria cadeia.

                          ## Onde salvar e como nomear

                          Salve os artefatos como Markdown, para que virem a memória viva do projeto:

                          - **Etapas 01–11:** em uma pasta do projeto (ex.: `cadeia-kiso/`), no formato `AAAA-MM-DD-<etapa-slug>-<projeto-slug>.md` (ex.: `2026-06-01-diagnostico-estrategico-<projeto>.md`).
                          - **Etapa 12 (Banco de Ideias):** em `bancos-de-ideias/` (é massa editorial executável, separada do núcleo estratégico).
                          - **Etapa 13 (Calendário):** em `calendarios-editoriais/`.
                          - Mantenha um **`MAPA.md`** na pasta do projeto: índice das etapas, ordem de leitura e o que já foi concluído vs. pendente.

                          Se o usuário tiver uma pasta conectada, salve lá. Caso contrário, salve na pasta de trabalho e ofereça o arquivo. Ao final da cadeia, o calendário pode ser exportado para planilha se o usuário quiser (então use a skill de xlsx).

                          ## Começando

                          Pergunte apenas o essencial para arrancar: **qual marca/profissional** e **qual etapa** (ou "começar do zero" → Etapa 01). Depois entre no ciclo de entrevista da etapa correspondente. Conduza uma etapa por vez, sempre fechando com as `Variáveis-chave` e a confirmação do usuário antes de seguir.
                          
