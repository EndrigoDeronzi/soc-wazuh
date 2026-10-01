# Caso fictício SOC-LAB-001
**Exercício de raciocínio. Nenhuma consulta ou resposta real foi executada.**

| Campo | Valor fictício |
|---|---|
| Sinal | DEMO-001: oito falhas em cinco minutos |
| Ativo | LAB-WS01 |
| Conta | lab.usuario01 |
| Origem de documentação | 192.0.2.25 |
| Prioridade inicial | Alta, para triagem |
| Hipóteses | Senha desatualizada em tarefa; tentativa de acesso indevido |
| Evidência complementar simulada | Tarefa de laboratório com credencial antiga |
| Classificação final do exercício | Erro operacional |
| Contenção | Não aplicada |
| Ação proposta | Responsável atualizar credencial da tarefa e validar execução |
| Critério de encerramento | Ausência de novas falhas e retomada da tarefa na simulação |

## Perguntas de investigação
Houve login bem-sucedido após as falhas? A origem é esperada? Há outras contas ou ativos envolvidos? Existia mudança aprovada? Os eventos têm o mesmo canal e contexto?

## Lição
A severidade inicial ajuda a ordenar a triagem. A conclusão precisa de contexto e evidências adicionais; o alerta não demonstra comprometimento por si só.
