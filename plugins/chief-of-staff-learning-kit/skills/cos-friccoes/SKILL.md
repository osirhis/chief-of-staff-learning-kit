---
name: cos-friccoes
description: Registra ou atualiza uma fricção do Chief of Staff quando algo não sai como esperado — erro, autonomia demais ou de menos, ferramenta que falhou, formato ruim, contexto esquecido. Use quando a pessoa disser fricção, quando ela corrigir o Chief of Staff, ou quando o próprio Chief of Staff perceber que errou.
---

# Registrar fricção

Registre a fricção como aprendizado local e atômico: a diferença entre o que
ocorreu e o que seria esperado. Registro não é tarefa, não é decisão e não
autoriza mudar o sistema. Corrigir fica para a governança, a não ser que a
pessoa peça para corrigir agora.

## Quando registrar

- Quando a pessoa pedir ("registra uma fricção", "isso é uma fricção").
- Quando a pessoa corrigir algo que o Chief of Staff deveria ter acertado, ou
  quando o próprio Chief of Staff perceber o erro. Nesses casos, registre e
  avise em uma linha; se o mandato disser que precisa perguntar antes, pergunte.
- Não registre pedido de teste sem um comportamento concreto. Se faltar o
  sintoma, pergunte o que aconteceu e o que era esperado.

## Escopo: fricção do Chief of Staff, não de outros sistemas

Esta skill registra o que **o Chief of Staff** fez diferente do esperado, na
área de trabalho da pessoa. Antes de registrar:

1. Se o mandato disser para onde vai cada tipo de problema (por exemplo,
   "defeito de plugin ou repositório de trabalho vai para a skill X"), siga o
   mandato.
2. Se o problema for de um sistema, plugin, skill ou repositório de terceiros
   que tem canal próprio de registro (outra skill instalada que abre issue ou
   registra falhas desse sistema), **não registre aqui por conta própria**:
   pergunte à pessoa se é fricção do Chief of Staff ou se deve ir para o canal
   daquele sistema.
3. Uma ferramenta que falhou **durante o trabalho do Chief of Staff** (um
   conector que não abriu, uma busca que não retornou) é fricção do Chief of
   Staff e vai para cá.

## Antes de registrar

1. Localize a área de trabalho do Chief of Staff e a pasta `friccoes/`. Se ela
   não existir, crie `friccoes/` e `friccoes/index.md` (ou sugira rodar
   `cos-setup-aprendizado`).
2. Leia o índice e as fricções em estado `aberta`, `planejada` ou `monitorando`.
3. Se o relato for um novo sintoma de um problema já registrado, **atualize a
   fricção existente** em vez de criar outra. Não deduplique só por palavras
   parecidas; explique a relação em uma frase.

## Registro canônico

Arquivo com nome estável e descritivo:
`friccoes/AAAA-MM-DD-descricao-curta.md`.

```markdown
# <título concreto do que aconteceu>

## Estado
aberta

## O que aconteceu
<fatos observáveis, sem antecipar causa>

## O esperado
<o que deveria ter acontecido>

## Contexto e evidências
- <o que estava sendo feito, conversa, data>
- <referência ou link, quando houver; nada inventado>

## Hipóteses
- Hipótese: <explicitamente marcada como hipótese>

## Impacto e recorrência
- Impacto: baixo | médio | alto
- Recorrência: isolada | ocasional | recorrente

## Primitivos a observar na correção
- <zero ou mais entre propósito, contexto, skill, tool e decisão, com o porquê;
  é hipótese, não diagnóstico>

## Workaround e tentativas anteriores
- <o que permitiu seguir trabalhando, se houver>

## Próximo experimento
<opcional; ainda não é tarefa nem decisão>

## Critério de resolução
<o que precisa ser observado para considerar resolvida>

## Governança
- Data da última sessão: ainda não realizada
- Encaminhamento:
- Estado resultante: aberta
- Primitivos observados:
- Julgamento e raciocínio:
- Ação ou experimento confirmado:
- Próxima revisão:

## Histórico
- AAAA-MM-DD: criada — <resumo>
```

Estados possíveis: `aberta`, `planejada`, `monitorando`, `resolvida`, `aceita`,
`descartada`.

## Privacidade e limites

- Registre um resumo e uma referência ao dado real. Não copie conteúdo pessoal,
  credenciais ou informação sensível sem necessidade concreta.
- Respeite o que o mandato diz sobre o que não se registra.
- Os registros ficam na área de trabalho da própria pessoa. Não envie nada a
  serviços externos.
- Não crie tarefas, não mude o mandato, não ajuste skills nem execute correções.

## Ao concluir

Atualize `friccoes/index.md` (título com link, estado, impacto, recorrência,
última atualização) e informe em poucas linhas:

- se criou ou atualizou uma fricção, e qual arquivo;
- se encontrou possível duplicata;
- que o próximo passo, quando quiser, é a governança (`cos-governanca`).
