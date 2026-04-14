# claude code workspace

**Seu assistente de trabalho com IA, sem precisar ser dev.**

Um kit pronto pra você usar o [Claude Code](https://claude.com/claude-code) (a IA da Anthropic que roda no seu terminal) junto com o [Obsidian](https://obsidian.md) (um app de notas local) como assistente de trabalho no dia-a-dia.

---

## O que é isso?

O `claude-code-workspace` é um repositório-modelo. Você baixa, abre no Obsidian, roda o Claude Code dentro dele — e pronto: tem um assistente que lê suas notas, organiza seu Inbox, resume documentos, rascunha emails, prepara reuniões e responde perguntas sobre o seu trabalho. Tudo offline (as notas ficam no seu computador) e usando IA de verdade (via sua conta Anthropic).

Não precisa programar. Não precisa instalar mil coisas. Precisa só seguir os 4 passos abaixo e saber digitar comandos tipo `/resumir` numa janela. O kit já vem com comandos prontos, receitas copiáveis pros casos mais comuns e uma estrutura de pastas pensada pra quem sempre se perdeu em notas soltas.

## Pra quem é?

- Profissional não-dev (marketing, gestão, conteúdo, vendas, consultoria) que quer produtividade real com IA
- Alguém que já ouviu falar de IA, testou ChatGPT, e agora quer usar de verdade no trabalho
- Quem vive perdido em notas soltas no Notion, Google Docs, post-its e quer um lugar só
- Quem quer organizar o dia, escrever melhor, pesquisar mais rápido e resumir documentos longos

## Pré-requisitos

Antes de começar, você precisa de:

1. **Conta Anthropic com créditos** — crie em [console.anthropic.com](https://console.anthropic.com) e adicione um cartão ou compre créditos. Uso típico custa poucos dólares por semana.
2. **Obsidian instalado** — baixe gratuitamente em [obsidian.md](https://obsidian.md).
3. **macOS** — o kit foi testado em Mac. Windows e Linux devem funcionar, mas ainda não foram validados.

---

## Instalação em 4 passos

### Passo 1 — Instalar o Claude Code

Siga as instruções oficiais da Anthropic: [docs.claude.com/en/docs/claude-code/setup](https://docs.claude.com/en/docs/claude-code/setup).

Ao terminar, você consegue abrir um terminal e digitar `claude` — se aparecer uma tela de boas-vindas, está funcionando.

![screenshot: terminal mostrando `claude` rodando pela primeira vez]

### Passo 2 — Baixar este repositório

Você tem duas opções. Escolha a que for mais confortável:

**Opção A — Git (recomendado):**

```bash
git clone https://github.com/SEU-USUARIO/claude-code-workspace.git
cd claude-code-workspace
```

**Opção B — Download ZIP:**

No GitHub, clique no botão verde **Code → Download ZIP**, descompacte o arquivo e coloque a pasta onde preferir (ex: `~/Documentos/claude-code-workspace`).

![screenshot: botão Code → Download ZIP no GitHub]

### Passo 3 — Abrir o Obsidian no vault

Abra o Obsidian. No menu inicial, clique em **Open folder as vault** (ou **Abrir pasta como vault**) e selecione a pasta `vault/` que está **dentro** do repositório que você baixou.

Pronto — agora o Obsidian está mostrando suas notas de exemplo.

![screenshot: Obsidian com a opção "Open folder as vault" selecionada]

### Passo 4 — Rodar o Claude Code

Abra o terminal **na pasta do repositório** (não na pasta `vault/` — na raiz `claude-code-workspace/`) e digite:

```bash
claude
```

O Claude vai ler o `CLAUDE.md` do projeto, entender que você é um profissional não-dev, e estar pronto pra ajudar em PT-BR.

![screenshot: terminal dentro da pasta claude-code-workspace com Claude Code rodando]

---

## Primeiro teste (2 minutos)

1. No Obsidian, abra a nota `Inbox/exemplo-nota.md` e dê uma olhada no texto.
2. Volte pro terminal onde o Claude está rodando.
3. Digite:

   ```
   /resumir vault/Inbox/exemplo-nota.md
   ```

4. Aperte Enter.

O Claude vai ler a nota e te devolver um resumo em bullets. É isso — você acabou de usar seu primeiro comando. 🎉

## E agora?

- **Aprenda o workflow diário:** leia o [GUIA.md](./GUIA.md) — 10 minutos de leitura, ensina a rotina de manhã/dia/noite com o Claude.
- **Copie casos prontos:** dê uma olhada no [RECEITAS.md](./RECEITAS.md) — tem ~12 receitas copiáveis pros usos mais comuns (reescrever email, brain dump virar plano, comparar opções, etc).

## Precisa de ajuda?

Travou em algum passo? A seção **Troubleshooting** do [GUIA.md](./GUIA.md) cobre os 5 problemas mais comuns. Se nada lá resolver, abra uma issue no repositório descrevendo o que aconteceu.

Boas-vindas — e bom trabalho com seu novo assistente.
