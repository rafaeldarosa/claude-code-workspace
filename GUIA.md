# GUIA — Como usar o claude code workspace no dia-a-dia

Este guia assume que você já instalou o Claude Code e o Obsidian (veja README.md). Leia com calma — são uns 10 minutos.

---

## 1. Conceitos básicos (5 min)

### O que é um vault?
Um **vault** é só uma pasta no seu computador que o Obsidian trata como "caderno digital". Nesse template, a pasta se chama `vault/`. Tudo que está lá dentro vira uma nota. Você pode criar, editar e organizar notas como arquivos `.md` (Markdown, que é só texto com formatação simples).

### O que é um slash command?
Dentro do Claude Code, quando você digita uma barra `/` seguida de um nome (ex: `/resumir`), você está chamando um **comando pronto**. É um atalho que já tem um prompt preparado — você só preenche o que falta. Os comandos deste template estão em `.claude/commands/`. Cada arquivo `.md` ali dentro vira um comando.

### Como o Claude "vê" suas notas?
O Claude Code lê os arquivos `.md` que estão na pasta onde você o abriu. Ele não precisa de "sincronização" nem "upload". Se você rodar `claude` dentro da pasta `claude-code-workspace/`, ele enxerga tudo que está ali — incluindo o `vault/`. Quando você pedir "resuma minha nota de ontem", ele vai procurar o arquivo e ler antes de responder.

> **Resumo:** vault = pasta de notas; slash command = atalho de prompt; Claude enxerga tudo que está na pasta aberta.

---

## 2. Rotina sugerida

### Manhã (5-10 min)
1. Abra o terminal na pasta `claude-code-workspace/` e rode `claude`.
2. Abra `vault/Inbox/hoje.md` no Obsidian (crie se não existir).
3. Faça um **brain dump**: escreva tudo que está na sua cabeça sem se preocupar com ordem — tarefas, ideias, sentimentos, compromissos.
4. No Claude Code, rode `/organizar`. Ele vai ler seu Inbox, sugerir pra qual pasta cada anotação deveria ir (Projetos, Notas, Arquivo) e te ajudar a mover.

### Durante o dia
Use as **receitas** do `RECEITAS.md` quando precisar. Exemplos:
- Recebi um email difícil → receita "Responder mensagem difícil"
- Tenho que decidir entre 3 opções → receita "Comparar opções"
- Vou entrar em reunião → receita "Pauta de reunião"

Também use os slash commands direto:
- `/email` quando precisar rascunhar um email
- `/pesquisar` quando quiser um mini-relatório sobre um tópico
- `/reuniao` pra transformar anotações cruas em ata

### Fim do dia (5 min)
1. Rode `/resumir` pedindo "resumo da minha semana" — o Claude vai ler seus arquivos recentes e gerar um apanhado.
2. Anote 1-2 **aprendizados** em `vault/Notas/` com um título descritivo (ex: `2026-04-14 aprendi sobre foco.md`).
3. Se terminou algum projeto, mova a nota dele de `Projetos/` pra `Arquivo/`.

---

## 3. Como criar seu próprio comando

Digamos que toda vez que você vai viajar, você quer um checklist padrão. Em vez de digitar o mesmo prompt toda hora, crie um comando.

**Passo a passo:**

1. Dentro da pasta do projeto, vá em `.claude/commands/`.
2. Crie um arquivo novo chamado `checklist-viagem.md`.
3. Cole isto dentro:

```markdown
---
description: Gera checklist de viagem personalizado
---

Crie um checklist de viagem considerando:
- Destino e duração informados pelo usuário
- Clima esperado
- Documentos necessários
- Itens essenciais (remédios, carregadores, adaptadores)
- Checklist de casa antes de sair (trancar, lixo, plantas)

Se o usuário não informou destino/duração, pergunte antes de gerar.
Salve o resultado em `vault/Notas/checklist-viagem-[destino]-[data].md`.
```

4. Salve. No Claude Code, digite `/checklist-viagem` e pronto — seu comando já está disponível.

Você pode criar quantos quiser. Quanto mais específico ao seu trabalho, mais útil.

---

## 4. Troubleshooting

### "Claude não achou minhas notas"
Você abriu o terminal na pasta certa? Rode `pwd` — o resultado precisa terminar em `/claude-code-workspace`. Se não for, use `cd` pra navegar até a pasta antes de rodar `claude`.

### "Meu comando não aparece quando digito `/`"
O arquivo `.md` está dentro de `.claude/commands/`? Confere o nome do arquivo — ele vira o nome do comando (ex: `meu-comando.md` → `/meu-comando`). Sem espaços, só letras minúsculas e hífens.

### "Claude respondeu em inglês"
Adicione "responda em português do Brasil" no seu prompt. Se acontecer sempre, abra o `CLAUDE.md` na raiz do projeto e confirme que tem a instrução de PT-BR ali. Ela é lida automaticamente.

### "Diz que estou sem créditos"
Vá em [console.anthropic.com](https://console.anthropic.com), entre na sua conta, menu Billing → adicione saldo. O Claude Code usa sua chave da Anthropic.

### "Obsidian não mostra um arquivo que criei pelo terminal"
Dá um `Cmd+R` pra recarregar, ou clica em outra pasta e volta pra original. Às vezes o Obsidian demora pra notar arquivos criados fora dele.

---

## 5. Próximos passos

Quando sentir que dominou o básico:

- **Docs oficiais do Claude Code:** https://docs.claude.com/claude-code
- **Docs do Obsidian:** https://help.obsidian.md
- **Experimente criar skills:** são como comandos mais poderosos, com lógica e sub-etapas. Depois que você estiver confortável com slash commands, vale estudar.
- **Conecte com seu calendário/email:** o Claude tem integrações (MCPs) que permitem ler Gmail, Google Calendar, Slack. Isso é o passo 2 — depois que o workflow básico estiver sólido.

**Regra de ouro:** comece simples. Use 1-2 comandos por semana até virarem hábito antes de tentar automatizar tudo.
