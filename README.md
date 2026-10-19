# Chief of Staff Learning Kit

Quatro hábitos para o seu Chief of Staff de IA aprender com o uso, mantendo o
julgamento humano no centro. Faz parte da mentoria de Chief of Staff (aula 4,
Decisions).

| Skill | O que faz |
|---|---|
| `configurar-aprendizado` | Prepara a área de trabalho: cria `friccoes/`, `diario/` e `sonhos/`, propõe a seção de aprendizado no seu mandato e entrega o prompt do dreaming semanal. **Comece por aqui.** |
| `registrar-friccao` | Registra o que saiu diferente do esperado, na hora, com o contexto da conversa. |
| `governar-friccoes` | Prepara a pauta das fricções abertas com recomendações; você decide o encaminhamento de cada uma. Decisões repetidas viram jurisprudência no mandato. |
| `escrever-diario` | Ao fim de uma sessão com produção significativa, registra o que foi feito, decidido e aprendido. |
| `sonhar` | Dreaming semanal: lê o diário, as fricções e as fontes da semana e propõe atualizações de contexto. Lembra toda semana, esquece todo mês. Só propõe; quem aprova é você. |

## Como os hábitos se encaixam

1. No dia a dia, algo sai errado → **fricção** registrada.
2. Quando houver tempo → **governança**: você decide o que corrigir.
3. Ao fim de uma sessão importante → **diário de bordo**.
4. Toda sexta → **dreaming**: o Chief of Staff lê a semana e propõe o que
   lembrar e o que esquecer. Você revisa e aprova.
5. Quando você aprova o mesmo tipo de coisa várias vezes, a regra vai para a
   **jurisprudência** do mandato, e o Chief of Staff ganha autonomia ali.

Tudo fica na pasta da sua área de trabalho. O kit não envia dados para lugar
nenhum e não altera o seu mandato sem sua confirmação.

## Instalar

### ChatGPT / Codex (app desktop)

1. Em **Plugins**, clique em **Adicionar** → **Adicionar marketplace**.
2. Cole na origem: `https://github.com/osirhis/chief-of-staff-learning-kit`
3. Instale o plugin **Chief Of Staff Learning Kit**.

### Claude Code

```text
/plugin install chief-of-staff-learning-kit --marketplace osirhis/chief-of-staff-learning-kit
```

Ou em dois passos:

```text
/plugin marketplace add osirhis/chief-of-staff-learning-kit
/plugin install chief-of-staff-learning-kit@chief-of-staff-learning
```

Para receber atualizações automaticamente: em `/plugin`, aba **Marketplaces**,
selecione `chief-of-staff-learning` e ative **Enable auto-update**. Sem isso,
atualize com `/plugin marketplace update chief-of-staff-learning`.

## Depois de instalar

Abra uma conversa com o seu Chief of Staff, na pasta da área de trabalho dele, e
peça:

> Configure o aprendizado do meu Chief of Staff.

Ele vai mostrar o que encontrou, o que pretende criar e o texto que quer
acrescentar ao mandato. Só grava depois que você confirmar. No fim, entrega o
prompt do dreaming para você agendar em **Agendado** (ChatGPT) ou
**Programado** (Claude).

## Vindo da versão 0.1

Suas fricções em `friccoes/` são preservadas: o formato e os estados são os
mesmos. Depois de atualizar o plugin, rode `configurar-aprendizado` uma vez para
criar `diario/` e `sonhos/` e acrescentar a seção de aprendizado ao mandato.

## Princípios

- Fricção é aprendizado, não tarefa. Registrar não autoriza corrigir.
- A governança recomenda; a pessoa decide.
- `resolvida` só com evidência contra o critério de resolução.
- O dreaming só propõe. Nada muda no contexto sem aprovação.
- Autonomia cresce por jurisprudência explícita, nunca por suposição.

Veja o [CHANGELOG](CHANGELOG.md).
