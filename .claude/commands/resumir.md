---
description: Resume uma nota ou documento longo em bullets objetivos
argument-hint: [caminho da nota ou cole o texto]
---

# Resumir

Resuma o conteúdo indicado em `$ARGUMENTS` em bullets curtos e diretos, em PT-BR. Foque no que o usuário precisa saber ou decidir, não em repetir tudo.

Siga esta estrutura:

1. **Contexto em 1 linha** — do que se trata.
2. **Pontos-chave** — 3 a 7 bullets, cada um com no máximo 2 linhas.
3. **Ações ou decisões pendentes** (se houver) — lista curta do que precisa ser feito ou respondido.

Regras:
- Se `$ARGUMENTS` for caminho de arquivo, leia o arquivo antes.
- Se for uma nota longa dentro do vault Obsidian, mantenha links `[[...]]` quando relevantes.
- Nada de enrolação, nada de repetir o texto original. Vá direto.
- Se o texto tiver menos de 10 linhas, avise que já está curto e pergunte se quer resumir mesmo assim.

## Exemplo de uso

`/resumir Inbox/reuniao-cliente-x.md`
