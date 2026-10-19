# Roteiro de testes

Casos que validam uma versão antes de ir para a turma. Rodar no Claude Code com
uma área de trabalho sintética (mandato, `pessoas/`, `projetos/`, `objetivos/`),
de preferência versionada em git para ver exatamente o que mudou.

Resultado da 0.2.0, em 19/10/2026, no Claude Code 2.1.303: **todos passaram**.

| # | Caso | Esperado |
|---|---|---|
| 1 | Setup, aluna vinda da 0.1 (`friccoes/` com registros) | Diagnóstico, proposta com o texto exato, **nenhuma escrita** antes do "pode gravar"; depois cria `diario/` e `sonhos/`, acrescenta a seção ao mandato e preserva as fricções |
| 2 | Setup, mandato dentro do `AGENTS.md` | Seção vai para o `AGENTS.md`; respeita limites existentes (no teste, propôs manter "perguntar antes de registrar colaboradores") |
| 3 | Setup com outra skill de fricção instalada | Detecta a skill e propõe a cláusula de quando usar cada uma; pergunta quais fontes o dreaming pode ler |
| 4 | "Registra uma fricção" com sintoma concreto | Arquivo novo no formato, linha no índice, aviso em poucas linhas |
| 5 | Nova ocorrência de fricção existente | Atualiza a existente, não duplica |
| 6 | Correção sem a palavra "fricção" | Corrige, confere os arquivos, registra por iniciativa e avisa; não cria regra sozinho |
| 7 | Fricção sem setup feito | Cria `friccoes/` e o índice |
| 8 | Falha de plugin de terceiros com canal próprio | Segue o mandato ou pergunta; não registra como fricção do Chief of Staff por conta própria |
| 9 | Governança — pauta | Pauta priorizada com recomendação e pergunta de julgamento; **nenhuma escrita** |
| 10 | Governança — decisões | Aplica só o decidido; consolida mantendo a secundária no índice; regra aprovada entra na jurisprudência citando a origem |
| 11 | Diário de bordo | Entrada fiel à sessão, com decisões, mudanças, fricções, lacunas e pendências |
| 12 | Dreaming | Escreve **só** em `sonhos/`; separa proposta firme de sinal; sem fonte autorizada, diz que usou só os arquivos |
| 13 | Dreaming com esquecimento e contexto envelhecido | Propõe arquivar o encerrado; nunca apaga |
| 14 | Revisão do sonho | Aplica só o aprovado, registra o desfecho; autonomia nova vira regra na jurisprudência após confirmar o texto |

Não testado automaticamente: instalação e uso no ChatGPT/Codex desktop e nas
interfaces de agendamento (Agendado/Programado). Validar manualmente.
