# Casos de uso didáticos
Os casos abaixo são propostas de investigação. Não correspondem a regras já implantadas ou validadas.

| Sinal | Contexto a verificar | Decisão inicial |
|---|---|---|
| Falhas repetidas de autenticação | Conta, origem, janela temporal e autenticações bem-sucedidas | Distinguir erro de senha, tarefa desatualizada e tentativa suspeita |
| Alteração de grupo privilegiado | Autor, autorização e janela de mudança | Confirmar mudança aprovada antes de escalar |
| Detecção reportada por EDR | Estado da ação, processo, arquivo e escopo | Confirmar proteção aplicada e necessidade de contenção |
| Alteração de arquivo monitorado | Caminho, usuário e mudança prevista | Correlacionar com manutenção e implantação |
| Agente sem comunicação | Conectividade, serviço e manutenção | Restaurar visibilidade e investigar o alcance |

## Priorização
Considere criticidade do ativo, confiança do sinal, alcance e indícios de atividade em curso. Severidade recebida da ferramenta e prioridade operacional são campos distintos. O exemplo usa prioridades didáticas, sem equivalência com níveis numéricos de regras Wazuh.

## Falhas de autenticação
A janela de cinco minutos e a quantidade de oito eventos do exemplo são arbitrárias. Antes de criar correlação real, defina agrupamento por conta e origem, exclusões justificadas, baseline e cenário de sucesso após falhas. Uma contagem isolada não confirma ataque.

## Critério de validação futura
Documente um teste positivo, um caso benigno, a regra/decoder efetivamente utilizado e o resultado observado. A cobertura só pode ser afirmada após esses testes.
