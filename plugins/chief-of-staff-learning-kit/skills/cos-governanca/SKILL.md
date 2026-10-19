---
name: cos-governanca
description: Conduz a governança das fricções do Chief of Staff — prepara a pauta das fricções abertas com recomendações, registra o que a pessoa decidir e transforma decisões repetidas em jurisprudência. Use quando a pessoa pedir governança, revisão das fricções, ou quiser decidir o que fazer com elas.
---

# Governar fricções

Governança é um ritual sob demanda de reflexão e julgamento. O Chief of Staff
prepara a pauta e recomenda; **a pessoa decide**. Nada é corrigido sem
confirmação explícita da ação específica.

## 1. Preparar a pauta

1. Leia `friccoes/index.md` e as fricções em `aberta`, `planejada` ou
   `monitorando` cuja próxima revisão chegou.
2. Leia só o contexto necessário: mandato, a seção `## Jurisprudência da
   parceria` e os arquivos que ajudem a entender cada fricção. Não os modifique
   nesta etapa.
3. Aponte possíveis duplicatas ou sintomas de uma mesma causa e proponha
   consolidar; só consolide após confirmação.
4. Priorize de forma explicável, sem falsa precisão: impacto, recorrência,
   urgência, risco, esforço e potencial de eliminar outras fricções.

Para cada fricção da pauta:

```markdown
### <título da fricção>

- Por que entra agora: <priorização explicável>
- O que aconteceu: <síntese com referência ao arquivo>
- Hipótese de causa: <se houver>
- Primitivos a observar: <propósito, contexto, skill, tool, decisão — com o porquê>
- Correção proposta: <o que mudaria, e em qual componente>
- Encaminhamento recomendado: <um dos seis abaixo, com justificativa>
- Pergunta de julgamento: <pergunta curta para a pessoa>
```

Encaminhamentos possíveis:

| Encaminhamento | Estado resultante | Volta à governança |
|---|---|---|
| endereçar agora | aberta, até haver evidência de resolução | na próxima ocorrência ou revisão |
| planejar | planejada | na data ou condição registrada |
| experimentar | monitorando | pelo critério e data do experimento |
| monitorar | monitorando | com novo sinal ou na data de revisão |
| aceitar conscientemente | aceita | só se a pessoa pedir |
| descartar | descartada | não volta, salvo reabertura |

Termine a pauta pedindo a decisão de forma simples, por exemplo: "responda com o
número e o encaminhamento de cada uma".

## 2. Aplicar o que foi decidido

Depois que a pessoa decidir:

1. Para **endereçar agora**, descreva a mudança concreta (no mandato, num
   arquivo de contexto, numa skill, numa configuração) e peça confirmação dessa
   mudança específica antes de fazê-la, a não ser que a pessoa já a tenha
   aprovado na própria decisão. Mudança em sistema externo segue a regra do
   mandato.
2. Atualize a seção `## Governança` de cada fricção: data, encaminhamento,
   estado resultante, primitivos observados, decisão e raciocínio da pessoa,
   ação confirmada, próxima revisão. Acrescente uma linha ao `## Histórico`.
3. Atualize `friccoes/index.md`. Fricção consolidada em outra **continua no
   índice**, com o estado da principal e a indicação "consolidada em" com o
   link; o arquivo dela é preservado com uma nota apontando para a principal.

Use `resolvida` somente quando o critério de resolução tiver evidência em uma
ocorrência real. Um plano ou uma correção sem reteste não resolve.

## 3. Jurisprudência

Jurisprudência é o histórico de decisões que orienta casos parecidos.

- Quando a decisão da pessoa criar uma **regra de autonomia** ("daqui pra
  frente, pode fazer X sem me perguntar", "nesse caso, sempre pergunte"),
  proponha o texto da regra e, com a confirmação, acrescente-o em
  `## Jurisprudência da parceria` no mandato, citando a fricção de origem.
- Se o mandato ainda não tiver essa seção, sugira rodar `cos-setup-aprendizado`
  ou peça para criá-la.
- Quando a mesma decisão aparecer pela segunda ou terceira vez em fricções
  diferentes, proponha transformá-la em regra. Até a pessoa aprovar, é só
  referência.

## Ao concluir

Entregue uma recapitulação curta: fricções analisadas, decisões tomadas,
mudanças aplicadas, experimentos em curso, regras novas de jurisprudência e o
que ficou pendente.
