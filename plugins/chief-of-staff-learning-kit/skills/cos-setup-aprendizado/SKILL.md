---
name: cos-setup-aprendizado
description: Prepara o Chief of Staff para aprender com o uso — cria as pastas friccoes/, diario/ e sonhos/, propõe a seção de aprendizado no mandato e entrega o prompt do dreaming semanal. Use uma vez ao instalar o kit, ao atualizar de versão, ou quando a pessoa pedir para configurar ou revisar o kit.
---

# Configurar o aprendizado do Chief of Staff

Esta skill prepara o Chief of Staff (CoS) da pessoa para os quatro hábitos do
kit: registrar fricções, governá-las, escrever o diário de bordo e sonhar toda
semana. Ela **propõe e só grava com confirmação explícita**. Não altera nada
antes de a pessoa aprovar.

## 1. Encontrar a área de trabalho do CoS

A área de trabalho é a pasta onde o CoS guarda o próprio contexto: normalmente
tem `AGENTS.md` (ou `CLAUDE.md`), um mandato e as pastas `pessoas/`,
`objetivos/` e `projetos/`.

- Se a conversa já está aberta nessa pasta, use-a.
- Se não estiver claro qual é, pergunte à pessoa. Não crie pastas num lugar
  presumido.
- Se não houver acesso a arquivos (por exemplo, um chat sem pasta conectada),
  explique que o kit precisa de uma pasta de trabalho e pare.

## 2. Fazer o diagnóstico (só leitura)

Verifique e anote:

1. **Onde mora o mandato.** Procure `mandato.md`. Se não existir, o mandato pode
   estar dentro do `AGENTS.md` ou do `CLAUDE.md`. Se não houver mandato nenhum,
   diga isso; o kit funciona, mas a seção de aprendizado vai para o `AGENTS.md`.
2. **Se o kit já foi configurado.** Procure no mandato a seção
   `## Como a parceria aprende`. Se existir, compare com o modelo abaixo e
   proponha só o que mudou.
3. **Pastas existentes.** `friccoes/`, `diario/`, `sonhos/` e seus `index.md`.
   Quem usou a versão 0.1 do kit já tem `friccoes/` com registros: **preserve
   tudo**; não renomeie, não reescreva e não apague fricções existentes.
4. **Possível conflito de nomes.** Verifique a lista de skills disponíveis na
   sessão. Se houver outra skill que também registra fricções, atritos, falhas
   ou issues (por exemplo, uma skill de trabalho que abre issues no GitHub),
   anote o nome real: a seção do mandato precisa dizer quando usar cada uma.
5. **Fontes que o dreaming pode ler.** Veja quais conectores e fontes a sessão
   tem (e-mail, chat, agenda, transcrições, gestão de tarefas) e o que o
   mandato já diz sobre eles. Na proposta, pergunte à pessoa quais o dreaming
   pode consultar e se há alguma conta ou pasta proibida.

## 3. Apresentar a proposta

Mostre, numa única mensagem:

- o que encontrou no diagnóstico;
- as pastas e arquivos que vai criar (somente os que faltam);
- o texto exato que vai acrescentar ao mandato, adaptado ao que encontrou;
- o que **não** vai fazer: não apaga nada, não muda propósito,
  responsabilidades ou limites existentes, não cria agendamento.

Peça confirmação explícita ("pode gravar?"). Se a pessoa pedir ajustes, ajuste
e mostre de novo.

### Modelo da seção do mandato

Acrescente ao fim do mandato (antes de uma seção de dúvidas em aberto, se
houver). Substitua `<DATA>` pela data de hoje.

```markdown
## Como a parceria aprende

Acordado em <DATA>. Quatro hábitos, do Chief of Staff Learning Kit:

- **Fricções** — o que sai abaixo da expectativa é registrado na hora em
  `friccoes/` (skill `cos-friccoes`). Fricção é qualquer coisa que o Chief
  of Staff fez diferente do esperado: informação errada, autonomia demais ou de
  menos, ferramenta que falhou, formato ruim, contexto esquecido.
- **Governança** — sob demanda, o Chief of Staff prepara a pauta das fricções
  abertas e recomenda um encaminhamento para cada uma; a pessoa decide (skill
  `cos-governanca`).
- **Diário de bordo** — ao fim de uma sessão com produção significativa, uma
  entrada em `diario/` com o que foi feito, decidido e aprendido (skill
  `cos-diario`).
- **Dreaming semanal** — uma revisão agendada lê o diário, as fricções e as
  fontes da semana e propõe atualizações de contexto em `sonhos/`. Lembrar toda
  semana, esquecer todo mês. O dreaming só propõe; quem aprova é a pessoa
  (skill `cos-sonhar`).

O Chief of Staff pode registrar fricção e escrever diário por iniciativa
própria, avisando em uma linha. Aplicar a correção de uma fricção ou uma
proposta do dreaming exige decisão da pessoa, salvo quando a jurisprudência
abaixo já autorizar.

## Jurisprudência da parceria

Regras de autonomia que nasceram de uma decisão na governança ou na revisão do
dreaming. Cada regra cita a fricção ou o sonho de origem e entra aqui só quando
a pessoa aprovar.

- Nenhuma regra ainda.
```

Acrescente ao fim de `## Como a parceria aprende` a linha das fontes, com o que
a pessoa responder:

```markdown
Fontes que o dreaming pode ler: <lista, por exemplo "e-mail de trabalho,
agenda e transcrições de reunião">. Fora dos limites: <o que a pessoa vetar,
ou "nada além do que o mandato já proíbe">.
```

Se a pessoa não souber ainda, escreva "só os arquivos desta área de trabalho,
até a pessoa autorizar outras fontes".

Se o diagnóstico encontrou conflito de nomes, acrescente ao fim de
`## Como a parceria aprende` um parágrafo dizendo quando usar cada skill, com os
nomes reais encontrados. Exemplo: "Fricção do Chief of Staff vai para
`friccoes/` com `cos-friccoes`; defeito de um repositório ou plugin de
trabalho vai para a skill X, que abre issue."

### Arquivos a criar (só os que faltarem)

- `friccoes/index.md`:

  ```markdown
  # Fricções

  | Fricção | Estado | Impacto | Recorrência | Última atualização |
  |---|---|---|---|---|
  ```

- `diario/index.md`:

  ```markdown
  # Diário de bordo

  Uma entrada por sessão com produção significativa, em
  `diario/AAAA-MM-DD-descricao-curta.md`.
  ```

- `sonhos/index.md`:

  ```markdown
  # Sonhos

  Um arquivo por rodada do dreaming, em `sonhos/AAAA-MM-DD.md`, com as
  propostas numeradas e o desfecho de cada uma.
  ```

Se `friccoes/index.md` já existir, não o recrie.

## 4. Gravar, depois de confirmado

Grave exatamente o que foi aprovado. Depois **releia cada arquivo gravado** (é
obrigatório, não opcional) para conferir que ficou como combinado, e informe o
que mudou, arquivo por arquivo.

## 5. Entregar o agendamento do dreaming

A skill não cria agendamentos: isso é feito pela pessoa na interface. Entregue
o prompt abaixo, pronto para colar, com o caminho da área de trabalho
preenchido, e as instruções da interface que a pessoa usa:

- **ChatGPT (app desktop):** menu *Agendado* → *Criar*. Escolha rodar sempre na
  mesma conversa, toda sexta no fim da tarde, e notificar itens relevantes. O
  computador precisa estar ligado na hora marcada.
- **Claude (app desktop):** menu *Programado* → criar uma tarefa semanal com o
  prompt abaixo. Se a área de trabalho é uma pasta do computador, a tarefa
  precisa rodar nele.
- **Outras interfaces:** use o recurso de tarefa agendada equivalente, ou rode
  manualmente toda sexta pedindo "roda o dreaming".

Prompt:

```text
Rode o dreaming semanal do meu Chief of Staff com a skill cos-sonhar, na área de
trabalho <CAMINHO>. Leia o mandato, as pastas pessoas/, objetivos/ e projetos/,
o diário desde o último sonho e as fricções abertas; consulte as fontes da
semana que estiverem conectadas. Se for a última sexta do mês, inclua o
esquecimento. Escreva o resultado em sonhos/AAAA-MM-DD.md com propostas
numeradas. Não altere nenhum outro arquivo, não escreva em sistemas externos e
não envie mensagens.
```

Sugira testar o agendamento uma vez na hora ("executar agora") e conferir se o
arquivo apareceu em `sonhos/`.

## Ao concluir

Resuma em poucas linhas: o que foi criado, o que foi preservado, o que mudou no
mandato e o próximo passo sugerido (registrar a primeira fricção real ou rodar o
primeiro dreaming).
