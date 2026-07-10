# Modelo de Artefato — padrão de todas as etapas

Todo documento de etapa da Cadeia Kiso segue este molde. Ele existe para que cada artefato seja lido tanto por humanos quanto pela própria cadeia (as `Variáveis-chave` são o contrato entre etapas).

## Estrutura obrigatória

```markdown
# <Nome do Artefato> — <Projeto>

Data: AAAA-MM-DD
Marca/projeto: <projeto>
Etapa Kiso: NN — <Nome da Etapa>
Entrada(s): <arquivo(s) da(s) etapa(s) anterior(es) consumida(s)>
Status: <ex.: rascunho inicial, revisado, com lacunas>

---

# <Corpo>

## <Seção 1 específica da etapa>
...
## <Seção N específica da etapa>
...

---

# Variáveis-chave

```yaml
chave_1: valor conciso
chave_2: valor conciso
# use listas quando fizer sentido
```

---

# Alertas de coerência
- <tensão ou contradição observada com etapas anteriores, se houver>

---

# Próxima etapa sugerida
Executar a Etapa NN+1 — <Nome> para <objetivo>.
```

## Regras de preenchimento

- **Cabeçalho sempre completo.** `Entrada(s)` deve listar exatamente as etapas cujas `Variáveis-chave` foram usadas — é o rastro da cadeia.
- **Frases curtas e verificáveis** no corpo; evite texto decorativo. Cada afirmação deve poder ser justificada pelo que o usuário disse.
- **`Variáveis-chave` é o coração.** São os dados que a próxima etapa vai ler. Nomes de chave em `snake_case`, valores concisos. Não omita este bloco.
- **Lacunas explícitas.** Onde faltar informação, escreva `[LACUNA: o que falta]` no corpo e na variável correspondente. Nunca preencha com suposição apresentada como fato.
- **Alertas de coerência** apontam contradições (ex.: objetivo que exige um público que o ICP excluiu). Mostre-os ao usuário; não os esconda.
