---
name: registrar-friccao
description: Registra ou atualiza uma fricção local do Chief of Staff quando algo não ocorre como esperado. Use para capturar o problema e seu contexto, sem criar tarefas ou alterar outras regras.
---

# Registrar fricção

Registre uma fricção como aprendizado local e atômico: a diferença entre o que ocorreu e o que seria esperado. Não trate o registro como uma tarefa, uma decisão ou autorização para alterar o sistema.

## Antes de registrar

1. Descubra o diretório de trabalho do Chief of Staff. Use `friccoes/` nele; crie a pasta e `friccoes/index.md` se não existirem.
2. Leia o índice e as fricções abertas ou monitoradas antes de criar qualquer arquivo.
3. Procure uma causa ou contexto já conhecido. Se o relato for um novo sintoma do mesmo problema, atualize a fricção canônica existente em vez de criar outra.

Não deduplique apenas pela semelhança de palavras. Explique brevemente a relação quando atualizar uma fricção existente.

## Registro canônico

Crie um arquivo com nome estável e descritivo em `friccoes/`, por exemplo `2026-09-08-conexao-slack-instavel.md`. Use esta estrutura:

```markdown
# <título curto>

## Estado
aberta | planejada | monitorando | resolvida | aceita | descartada

## O que aconteceu
<fatos observáveis>

## O esperado
<resultado ou comportamento esperado>

## Contexto e evidências
- <resumo útil>
- <referência local, URL ou identificador da fonte, quando houver>

## Hipóteses
- <hipótese explicitamente marcada como hipótese>

## Impacto e recorrência
- Impacto: baixo | médio | alto
- Recorrência: isolada | ocasional | recorrente

## Primitivos a observar na correção
- <zero ou mais entre: propósito, contexto, skill, tool, decisão>
- <por que cada primitivo pode estar contribuindo; trata-se de uma hipótese, não de diagnóstico definitivo>

## Workaround e tentativas anteriores
- <o que permitiu seguir trabalhando, se houver>

## Próximo experimento
<opcional; ainda não é tarefa nem decisão>

## Critério de resolução
<como saberemos que deixou de ser uma fricção>

## Governança
- Data da última sessão: <data ou ainda não realizada>
- Encaminhamento: <endereçar agora | planejar | executar experimento | monitorar | aceitar conscientemente | descartar>
- Estado resultante: <aberta | planejada | monitorando | resolvida | aceita | descartada>
- Primitivos observados: <zero ou mais, com justificativa curta>
- Julgamento e raciocínio: <o que foi decidido e por quê>
- Ação ou experimento confirmado: <se houver; não criar tarefa sem confirmação explícita>
- Próxima revisão: <data, condição ou não se aplica>

## Histórico
- <data>: criada ou atualizada — <resumo da mudança>
```

## Privacidade e limites

- Registre um resumo e uma referência para o dado real; não copie conteúdo pessoal, credenciais ou informação sensível sem necessidade concreta para compreender a fricção.
- Preserve os registros na máquina e no projeto da própria pessoa. Não centralize nem envie conteúdo a serviços externos.
- Não crie tarefas, mude o `AGENTS.md`, altere contexto, ajuste uma skill ou execute uma correção. Essas são possibilidades a avaliar em governança.
- Não force uma fricção a caber em um único primitivo. Uma mesma fricção pode resultar da interação entre dois ou mais deles.

## Ao concluir

Atualize `friccoes/index.md` com título, estado, impacto, recorrência, última atualização e link para a fricção canônica. Informe:

- se criou ou atualizou uma fricção;
- qual evidência ou referência foi preservada;
- se encontrou possível duplicata;
- que o próximo passo, se desejado, é chamar `governar-friccoes`.
