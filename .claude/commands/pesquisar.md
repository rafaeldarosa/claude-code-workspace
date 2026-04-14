---
description: Pesquisa estruturada sobre um tópico e salva como nota no vault
argument-hint: [tópico ou pergunta, ex: "tendências de marketing B2B 2026"]
---

# Pesquisar

Faça uma pesquisa estruturada sobre o tópico em `$ARGUMENTS` e salve o resultado como nota em `vault/Notas/`. Responda em PT-BR.

Estrutura da nota final:

```
# [Título do tópico]

**Data:** YYYY-MM-DD
**Fonte:** Pesquisa com IA (revisar antes de usar)

## Resumo em 3 linhas
[O essencial]

## Pontos principais
- [5 a 8 bullets]

## Dados e números relevantes
[Se houver]

## Perspectivas diferentes
[Visões opostas ou nuances]

## Próximos passos pra aprofundar
- [Livros, sites, pessoas a consultar]

## Tags
#pesquisa #[area-do-tópico]
```

Regras:
- Use WebSearch se tiver disponível pra trazer informação atual. Se não, use seu conhecimento e **avise claramente** que não foi validado na web.
- Cite fontes quando possível (links).
- Nome do arquivo: `pesquisa-[slug-do-tópico]-YYYY-MM-DD.md`.
- Confirme o caminho final antes de salvar.

## Exemplo de uso

`/pesquisar como precificar serviço de consultoria para PMEs`
