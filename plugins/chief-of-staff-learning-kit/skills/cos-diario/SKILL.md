---
name: cos-diario
description: Escreve o diário de bordo de uma sessão de trabalho com o Chief of Staff — o que foi produzido, decidido, mudado e aprendido — para alimentar o dreaming semanal. Use quando a pessoa pedir o diário ou para fechar a sessão, e ofereça ao fim de uma sessão com produção significativa.
---

# Escrever o diário de bordo

O diário é a memória das sessões. Sem ele, o dreaming semanal só enxerga as
fontes externas e perde o que foi decidido e aprendido nas conversas.

## Quando escrever

- Quando a pessoa pedir ("escreve o diário", "fecha o diário", "/diário").
- Ao fim de uma sessão com produção significativa (um entregável, uma decisão,
  uma mudança no sistema do Chief of Staff), ofereça em uma linha. Não escreva
  diário de conversa rápida.

## Onde

Um arquivo por entrada em `diario/AAAA-MM-DD-descricao-curta.md`, na área de
trabalho do Chief of Staff. Se `diario/` não existir, crie (ou sugira rodar
`cos-setup-aprendizado`). Mais de uma entrada no mesmo dia é normal.

Não edite entradas de sessões anteriores. Uma correção vira entrada nova que
aponta para a anterior.

## Formato

Use as seções que fizerem sentido; **Progresso** é obrigatória.

```markdown
# AAAA-MM-DD — <assunto da sessão>

## Progresso
- O que foi produzido ou mudou, e por que importa.
- Estado: rascunho, entregue, publicado, aguardando.

## Decisões e contexto
- O que a pessoa decidiu e por quê. Distinguir proposta de aprovação.

## Mudanças na área de trabalho
- Arquivos do Chief of Staff criados ou atualizados.

## Fricções
- Links para fricções registradas ou atualizadas na sessão.

## Lacunas de contexto
- Conhecimento sem casa: fato ou decisão que só existe na conversa.
- Processo improvisado que vai se repetir: candidato a skill ou rotina.
- Estrutura que atrapalhou: pasta, arquivo ou regra que faltou.
  Para cada uma: o que foi descoberto e onde deveria morar.

## Referências
- Documentos, tarefas, mensagens, reuniões. Só o que existe.

## Pendências
- O que ficou aberto e quem destrava.
```

## Regras

- Separe fato, interpretação e proposta. O diário não torna nada verdade nem
  regra aprovada.
- Não invente evidência, horário ou identificador.
- Respeite o que o mandato diz sobre informação sensível.
- Se a sessão revelou uma fricção ainda não registrada, registre-a com
  `cos-friccoes` e coloque o link no diário.
- O diário não substitui atualizar pessoas, objetivos e projetos durante a
  conversa, quando o mandato pede isso.

## Ao concluir

Informe em uma linha o caminho do arquivo criado.
