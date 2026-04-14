---
description: Transforma anotações cruas de reunião em ata organizada + próximos passos
argument-hint: [caminho da nota crua ou cole as anotações]
---

# Reunião → Ata

Transforme as anotações cruas em `$ARGUMENTS` numa ata de reunião clara e acionável, em PT-BR. Se for um caminho de arquivo, leia antes.

Entregue no formato:

```
# Ata — [Assunto da reunião]

**Data:** YYYY-MM-DD
**Participantes:** [lista, se mencionado]

## Contexto
[1 parágrafo curto — por que a reunião aconteceu]

## Decisões tomadas
- [bullet objetivo por decisão]

## Pontos discutidos
- [tópicos importantes que não viraram decisão]

## Próximos passos
- [ ] [Ação] — responsável: [nome] — prazo: [data ou "a definir"]
- [ ] ...

## Pendências e dúvidas
- [perguntas em aberto]
```

Regras:
- Seja fiel às anotações — não invente decisões ou prazos que não foram ditos.
- Se algo estiver ambíguo, liste em **Pendências** em vez de chutar.
- Pergunte se quer salvar em `vault/Notas/ata-[assunto]-YYYY-MM-DD.md`.
- Se a nota crua for muito bagunçada, faça 1 pergunta pra esclarecer o essencial antes de gerar a ata.

## Exemplo de uso

`/reuniao Inbox/reuniao-equipe-2026-04-14.md`
