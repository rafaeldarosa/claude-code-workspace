---
description: Organiza notas do Inbox movendo para Projetos ou Notas conforme o conteúdo
argument-hint: [opcional: nome de nota específica, senão processa o Inbox todo]
---

# Organizar Inbox

Organize as notas do `vault/Inbox/`. Se `$ARGUMENTS` estiver vazio, processe todas as notas da Inbox. Se tiver um nome, processe só aquela.

Para cada nota:

1. **Leia o conteúdo.**
2. **Classifique** em uma dessas categorias:
   - **Projeto** — se descreve algo com objetivo + próximos passos → mover pra `vault/Projetos/`.
   - **Nota de referência** — conhecimento, ideia, anotação solta → mover pra `vault/Notas/`.
   - **Descartável** — rascunho sem valor → perguntar antes de mover pra `vault/Arquivo/`.
3. **Renomeie** se o título estiver genérico (ex: `nova-nota.md` → `reuniao-cliente-x-2026-04-14.md`). Use kebab-case.
4. **Sugira tags ou links** `[[...]]` pra conectar com notas já existentes no vault.

Regras:
- Sempre **mostre o plano antes de mover** (lista: nota → destino) e peça confirmação.
- Nunca apague nada sem confirmação.
- Respeite PT-BR nos nomes de arquivo.

## Exemplo de uso

`/organizar` (processa tudo)
`/organizar ideia-produto.md` (só essa nota)
