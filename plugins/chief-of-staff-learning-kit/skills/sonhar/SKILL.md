---
name: sonhar
description: Roda o dreaming do Chief of Staff — revisão semanal que lê o diário, as fricções e as fontes da semana e propõe atualizações de contexto em sonhos/; na última sexta do mês propõe também o que esquecer. Também revisa com a pessoa as propostas de um sonho já rodado. Use quando a pessoa pedir o dreaming, o sonho ou a revisão semanal de contexto.
---

# Dreaming do Chief of Staff

Quando sonhamos, a memória de curto prazo vai para a de longo prazo. O dreaming
faz o mesmo com o Chief of Staff: transforma o que aconteceu na semana em
contexto durável. **Lembrar toda semana, esquecer todo mês.**

**O dreaming só propõe.** Durante a execução, a única escrita permitida é o
arquivo do sonho em `sonhos/`. Quem aprova é a pessoa, numa conversa depois.

Esta skill tem dois modos: **sonhar** e **revisar o sonho**.

## Modo 1 — Sonhar

### O que ler

1. O mandato e as pastas de contexto (`pessoas/`, `objetivos/`, `projetos/` ou
   as que a área de trabalho usar).
2. `diario/`: as entradas desde o último arquivo em `sonhos/` (ou dos últimos
   sete dias, se for o primeiro sonho).
3. `friccoes/index.md` e as fricções abertas ou em monitoramento.
4. As fontes da semana que o mandato autoriza (linha "Fontes que o dreaming
   pode ler", quando existir) e que estiverem conectadas: e-mail, chat de
   trabalho, agenda, transcrições de reunião, gestão de tarefas. Respeite as
   restrições do mandato sobre contas e dados pessoais. Se o mandato não
   autorizar nenhuma fonte, use só os arquivos e diga isso no sonho. Se uma
   fonte autorizada falhar, anote e siga com as demais.

### O que fazer

1. **O que eu sei.** Resumo curto das prioridades, projetos e pessoas centrais
   segundo os arquivos.
2. **O que a semana desafia ou acrescenta.** Fatos novos, mudanças de estado,
   decisões, pessoas novas relevantes, projetos que surgiram ou terminaram. Cada
   item com a evidência (fonte e data).
3. **Propostas de atualização.** Para cada uma: arquivo, mudança (criar,
   atualizar, marcar como encerrado) e evidência. Separe o que já tem insumo
   suficiente do que ainda é só sinal.
4. **Fricções.** Fricções aparentes na semana que ninguém registrou, e fricções
   paradas há mais de duas semanas sem governança.
5. **Padrões de decisão.** Aprovações que a pessoa deu repetidas vezes e que
   poderiam virar regra de autonomia. É proposta de jurisprudência, não regra.
6. **Esquecimento (só na última sexta-feira do mês, ou quando a pessoa pedir).**
   O que envelheceu: pessoas, projetos ou trechos de contexto sem sinal há mais
   de um mês, ou já encerrados. Proponha arquivar ou enxugar. Nunca apague.

### Onde entregar

Crie `sonhos/AAAA-MM-DD.md` (crie a pasta se faltar):

```markdown
# Sonho de AAAA-MM-DD

## Resumo
<três linhas: o que mais mudou, quantas propostas, o que pede atenção>

## Propostas
1. <arquivo> — <mudança proposta>. Evidência: <fonte, data>.
2. ...

## O que eu sei
## O que a semana trouxe
## Fricções
## Padrões de decisão
## Esquecimento
<só quando aplicável>

## Fontes que falharam
## Desfecho
<preenchido na revisão>
```

Atualize `sonhos/index.md` com uma linha para o sonho, se o índice existir.

### Limites

- Não altere mandato, contexto, fricções nem diário durante o sonho.
- Não escreva em sistemas externos, não envie mensagens, não altere agenda.
- Não registre o que o mandato proíbe (dados sensíveis, avaliações sobre
  pessoas, valores, etc.).

Ao terminar, diga em até cinco linhas: quantas propostas, as duas mais
importantes, fontes que falharam e o caminho do arquivo.

## Modo 2 — Revisar o sonho

Quando a pessoa abrir um sonho para revisar ("vamos revisar o sonho"):

1. Leia o arquivo mais recente de `sonhos/` (ou o indicado).
2. Apresente as propostas por número, com a evidência de cada uma.
3. A pessoa aprova, recusa ou ajusta. Aplique **só o aprovado** nos arquivos de
   contexto.
4. Registre o desfecho de cada proposta na seção `## Desfecho` do sonho.
5. Quando a pessoa disser que um tipo de proposta pode ser aprovado sem
   perguntar ("esse tipo de atualização você pode fazer direto"), proponha o
   texto da regra e, com confirmação, acrescente-o em `## Jurisprudência da
   parceria` no mandato, citando o sonho de origem. É assim que a autonomia
   cresce.
6. Fricção apontada pelo sonho que a pessoa confirmar vira registro com
   `registrar-friccao`.
