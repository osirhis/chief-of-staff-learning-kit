---
name: governar-friccoes
description: Prepara e conduz, sob demanda, uma revisão de fricções locais do Chief of Staff. Use para priorizar, discutir opções e recomendar formas de resolver fricções; não executa mudanças sem confirmação humana.
---

# Governar fricções

Governança é um ritual sob demanda de reflexão e julgamento. Ela transforma fricções acumuladas em uma pauta clara, recomenda opções de correção e preserva as decisões tomadas como histórico de raciocínio — sem pressupor que todas terão o mesmo tipo de resolução.

## Preparar a sessão

1. Localize `friccoes/index.md` e leia as fricções em estado `aberta` ou `monitorando`.
2. Leia apenas o contexto necessário do Chief of Staff: mandato, projetos e pendências que ajudem a entender as fricções selecionadas. Não modifique esses arquivos.
3. Verifique possíveis duplicatas ou sintomas de uma mesma causa. Proponha consolidação, mas só altere registros canônicos após confirmação humana.
4. Priorize de forma explicável, sem falsa precisão, considerando: impacto, recorrência, urgência, risco, governabilidade/esforço e potencial de eliminar outras fricções.
5. Para cada fricção, indique os primitivos que provavelmente devem ser observados na correção: propósito, contexto, skill, tool e decisão. A indicação é aberta e multivalorada: não exija uma causa única, nem trate a lista como diagnóstico definitivo.

## Pauta de decisão

Para cada fricção priorizada, apresente:

```markdown
### <título da fricção>

- Por que entra agora: <priorização explicável>
- Fatos e contexto relevante: <síntese com referências>
- Hipótese de causa: <se houver>
- Opções de encaminhamento:
  1. endereçar agora
  2. planejar
  3. executar um experimento
  4. monitorar
  5. aceitar conscientemente
  6. descartar
- Recomendação inicial: <opção e justificativa>
- Primitivos a observar: <zero ou mais entre propósito, contexto, skill, tool e decisão; com justificativa breve para cada>
- Possível camada de correção: tool, configuração, skill, contexto, decisão, propósito/mandato ou outra
- Pergunta de julgamento: <pergunta curta para a pessoa>
```

Não trate os primitivos a observar nem a "possível camada" como diagnóstico definitivo. Uma fricção pode derivar da interação entre vários primitivos, exigir mais de uma intervenção ou não demandar nenhuma mudança no Chief of Staff.

## Registrar a decisão

Após a pessoa decidir, atualize a seção `## Governança` da fricção correspondente com data, encaminhamento, estado resultante, primitivos observados, raciocínio, ação ou experimento confirmado e próxima revisão. Uma decisão pode resultar em:

- correção de tool ou configuração;
- criação, revisão ou descarte de uma skill;
- mudança de contexto, decisão, propósito ou mandato;
- experimento limitado;
- monitoramento, aceitação consciente ou descarte.

Use este mapa de estados:

| Encaminhamento escolhido | Estado resultante | Como retorna à governança |
| --- | --- | --- |
| endereçar agora | aberta | até haver evidência de resolução ou novo encaminhamento |
| planejar | planejada | na data/condição registrada para revisão |
| executar um experimento | monitorando | com base no critério e na data de acompanhamento |
| monitorar | monitorando | quando houver novo sinal ou na data de revisão |
| aceitar conscientemente | aceita | somente se a pessoa pedir nova revisão |
| descartar | descartada | não retorna, salvo reabertura explícita |

Use `resolvida` somente quando o critério de resolução registrado na fricção tiver evidência suficiente. Não o use como sinônimo de "já existe um plano".

Não altere `AGENTS.md`, contexto, skills, tools, tarefas, estados externos ou configurações por conta própria. Primeiro peça confirmação explícita para a ação específica. O resultado da governança é uma recomendação e um histórico de julgamento, não uma execução automática.

## Jurisprudência

Jurisprudência é o histórico de decisões que continua útil para orientar casos semelhantes. Nesta versão, ela fica registrada no histórico da fricção canônica e não exige alteração do `AGENTS.md`.

Quando uma decisão for repetidamente validada, proponha — sem executar — onde ela poderia ser formalizada no futuro. Até lá, trate-a como referência revisável, não como regra permanente.

## Ao concluir

Entregue uma pauta ou recapitulação concisa contendo:

- fricções analisadas e a ordem de prioridade;
- decisões tomadas, adiadas ou pendentes;
- propostas de experimentos e seus critérios de acompanhamento;
- confirmações necessárias antes de qualquer ação consequencial.
