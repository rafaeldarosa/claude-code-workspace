# Receitas

Receitas são prompts prontos pra tarefas que você repete no dia-a-dia. Cada uma resolve uma situação comum: reescrever um texto, organizar ideias soltas, comparar opções, preparar uma reunião.

**Como usar:** encontre a receita, copie o prompt, cole no chat do Claude Code (terminal ou Obsidian) e troque os `[colchetes]` pelo seu contexto. Pronto.

---

## Escrita & Comunicação

### Reescrever texto em outro tom

**Quando usar:** você já tem um rascunho, mas o tom não está certo (muito formal, muito seco, muito longo).

**Prompt pronto:**
> Reescreva o texto abaixo em tom [formal / casual / amigável / direto / empático]. Mantenha o conteúdo e o tamanho parecido, só ajuste a linguagem. Se ficar estranho em algum ponto, me diga.
>
> Texto: [cole aqui]

**Exemplo de resultado:**
Versão reescrita mantendo o mesmo conteúdo, mas com linguagem ajustada. Se o texto original for muito técnico e você pedir "casual", o Claude troca jargões por expressões do dia-a-dia e quebra frases longas.

---

### Responder mensagem difícil

**Quando usar:** cliente chateado, negociação travada, feedback negativo — aquela mensagem que você lê 3 vezes antes de responder.

**Prompt pronto:**
> Preciso responder a mensagem abaixo. Meu objetivo é [acalmar / negociar prazo / recusar sem queimar / pedir mais info]. Quero soar [profissional, firme, empático — escolha 2]. Me dê 2 versões de resposta curtas (máx 6 linhas cada) e aponte qual você recomenda e por quê.
>
> Mensagem recebida: [cole aqui]
> Contexto: [1-2 linhas sobre a situação]

**Exemplo de resultado:**
Duas opções de resposta lado a lado + recomendação do Claude. Uma mais direta, outra mais suave. Geralmente uma frase de abertura que reconhece o problema + proposta concreta + fechamento sem promessa vazia.

---

### Post de LinkedIn a partir de uma ideia

**Quando usar:** você teve um insight ou viveu algo no trabalho e quer virar post, mas não sabe por onde começar.

**Prompt pronto:**
> Transforme a ideia abaixo em um post de LinkedIn. Formato: abertura forte (1-2 linhas), corpo com história/exemplo, insight prático, pergunta no final. Tom conversacional, sem clichê de coach. Máx 150 palavras. Me dê 2 versões com aberturas diferentes.
>
> Ideia: [cole aqui, mesmo que cru]

**Exemplo de resultado:**
Duas versões com hooks diferentes (uma começando com pergunta, outra com afirmação polêmica). Corpo estruturado, sem emoji excessivo, terminando com pergunta que convida comentário.

---

## Análise & Pesquisa

### Comparar 2-3 opções

**Quando usar:** você precisa escolher entre ferramentas, fornecedores, abordagens e está travado.

**Prompt pronto:**
> Compare as opções abaixo pros meus critérios. Monte uma tabela com as opções nas colunas e os critérios nas linhas. No fim, recomende uma e explique em 3 linhas por quê. Se faltar informação, diga o que eu preciso pesquisar.
>
> Opções: [A, B, C]
> Critérios importantes pra mim: [preço, facilidade, suporte, etc]
> Contexto: [por que estou escolhendo, pra quê vou usar]

**Exemplo de resultado:**
Tabela comparativa clara, uma recomendação direta e uma lista curta de "pontos abertos" caso falte informação sua ou pública.

---

### Extrair dados de texto longo pra tabela

**Quando usar:** você tem um email gigante, relatório ou transcrição, e precisa dos dados estruturados.

**Prompt pronto:**
> Leia o texto abaixo e extraia os dados em formato de tabela. Colunas que eu quero: [ex: nome, empresa, pedido, prazo, status]. Se faltar algum campo, marque como "—". Depois da tabela, me diga se notou algo estranho ou inconsistente.
>
> Texto: [cole aqui]

**Exemplo de resultado:**
Tabela markdown limpa, um campo por coluna, linhas organizadas. Abaixo, uma nota do tipo "notei que 2 pedidos estão sem prazo e o cliente X aparece duas vezes com dados diferentes".

---

### SWOT de projeto ou ideia

**Quando usar:** você está avaliando uma oportunidade e quer uma análise rápida antes de decidir.

**Prompt pronto:**
> Faça uma análise SWOT da ideia/projeto abaixo. Seja específico — nada genérico tipo "mercado competitivo". Cada quadrante com 3-5 bullets concretos pro meu contexto. No fim, me dê a pergunta mais importante que preciso responder antes de seguir.
>
> Ideia: [descreva em 3-5 linhas]
> Meu contexto: [experiência, recursos, prazo]

**Exemplo de resultado:**
Quatro blocos (Forças, Fraquezas, Oportunidades, Ameaças) com bullets específicos pro seu caso. Fecha com uma pergunta-chave tipo "você consegue validar demanda em 30 dias sem gastar mais de X?".

---

## Organização

### Brain dump virando plano de ação

**Quando usar:** sua cabeça está cheia, você despeja tudo numa nota e agora precisa virar algo acionável.

**Prompt pronto:**
> Abaixo está meu brain dump. Organize em: (1) próximas ações concretas pra essa semana, (2) coisas pra pensar mais, (3) ruído/pode ignorar. Cada ação tem que ser uma frase que começa com verbo. Se duas ideias são a mesma coisa, junte.
>
> Brain dump: [cole aqui, bagunçado mesmo]

**Exemplo de resultado:**
Três listas. "Próximas ações" com itens tipo "Ligar pro João sobre contrato" — acionáveis de verdade. "Pensar mais" com perguntas, não tarefas. "Ruído" curto, pra você confirmar que pode descartar.

---

### Priorizar tarefas (urgente/importante)

**Quando usar:** sua lista de tarefas cresceu e você não sabe por onde começar.

**Prompt pronto:**
> Classifique as tarefas abaixo numa matriz urgente/importante (4 quadrantes). Pra cada tarefa diga em qual quadrante vai e por quê em 1 linha. No fim, me diga as 3 que eu devo fazer HOJE e qual posso deletar da lista.
>
> Tarefas: [cole a lista]
> Contexto: [prazos, compromissos fixos da semana]

**Exemplo de resultado:**
Quatro grupos com as tarefas distribuídas. No rodapé, recomendação direta: "Hoje faça X, Y, Z. Pode deletar W — não vai gerar impacto real."

---

### Revisão semanal + plano da próxima

**Quando usar:** sexta à tarde ou domingo à noite, quando você quer fechar a semana e começar a próxima com clareza.

**Prompt pronto:**
> Abaixo estão minhas notas da semana. Me ajude a fazer revisão semanal: (1) o que avançou, (2) o que travou e por quê, (3) o que aprendi, (4) 3 prioridades pra próxima semana baseadas no que ficou em aberto. Seja específico e honesto, não puxe saco.
>
> Notas da semana: [cole anotações, tarefas feitas, compromissos]

**Exemplo de resultado:**
Resumo estruturado em 4 blocos. "Avançou" celebra vitórias reais. "Travou" aponta padrões (ex: "3 coisas esperando resposta de cliente"). Prioridades da próxima semana saem do que ficou pendente, não do nada.

---

## Produtividade

### Quebrar projeto grande em passos pequenos

**Quando usar:** você tem um projeto que parece montanha e procrastina porque não sabe onde começar.

**Prompt pronto:**
> Quebre o projeto abaixo em passos pequenos. Regra: cada passo tem que caber em 1-2 horas e ter um resultado visível. Organize em fases se fizer sentido. Marque o primeiro passo que eu faço HOJE pra destravar. Se algum passo depende de outra pessoa, destaque.
>
> Projeto: [descreva em 3-5 linhas: o quê, pra quê, prazo]

**Exemplo de resultado:**
Lista numerada em fases (ex: Preparação → Execução → Lançamento). Primeiro passo destacado tipo "HOJE: escrever rascunho de 1 página do briefing — 45 min". Dependências externas marcadas com aviso.

---

### Checklist a partir de um processo

**Quando usar:** você faz algo recorrente (onboarding de cliente, publicar post, fechar mês) e quer parar de esquecer passos.

**Prompt pronto:**
> Transforme a descrição abaixo em checklist numerada, prática, do tipo "faça isso". Inclua passos óbvios que eu posso esquecer sob pressão. No fim, adicione 2-3 verificações finais ("antes de dar por pronto, confira..."). Formato markdown com caixinhas `- [ ]`.
>
> Processo: [descreva como você faz hoje, mesmo que informal]

**Exemplo de resultado:**
Checklist `- [ ]` numerada, pronta pra colar no Obsidian. Passos na ordem certa, inclui itens tipo "confirmar que arquivo foi salvo" que você esqueceu de mencionar. Bloco de verificação final com 2-3 itens críticos.

---

### Pauta de reunião

**Quando usar:** você tem uma reunião marcada e quer chegar preparado, não improvisando.

**Prompt pronto:**
> Monte a pauta da reunião abaixo. Formato: objetivo em 1 linha, 3-5 tópicos com tempo sugerido em cada, perguntas-chave a fazer, decisões que precisam sair dessa reunião. No fim, liste o que eu preciso ter em mãos antes de começar.
>
> Reunião sobre: [assunto]
> Participantes: [quem vai]
> Duração: [30min / 1h]
> Contexto: [onde estamos, o que já foi discutido]

**Exemplo de resultado:**
Pauta com objetivo claro no topo, cronograma por bloco (ex: "10min — status atual / 15min — opções na mesa / 5min — próximos passos"), perguntas provocativas pra guiar discussão, e checklist de prep ("ter à mão: relatório X, proposta Y").
