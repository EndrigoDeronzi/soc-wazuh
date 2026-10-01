# Arquitetura e escopo
Os agentes coletam informações dos endpoints. O Wazuh server analisa os dados; o indexer armazena e permite consultar os alertas; o dashboard apresenta os resultados. O desenho do README é uma referência, não uma declaração da topologia de produção.

## Fontes e requisitos
| Fonte | Uso previsto | Pré-requisito |
|---|---|---|
| Windows Security | Autenticação e alterações de contas | Política de auditoria e permissões de leitura |
| Windows System | Contexto de serviços e sistema | Coleta habilitada |
| Windows Application | Contexto de aplicações | Canal e aplicação relevantes |
| EDR | Alertas de proteção e detecção | Transporte, formato, decoder e regra validados |
| Integridade de arquivos | Alterações em caminhos monitorados | Política FIM definida e habilitada |

Receber uma mensagem TCP não garante que ela seja interpretada ou gere alerta. Para EDR, confirme transporte protegido, campos, timestamp, decoder e regras usando logs de laboratório. Não exponha um receptor indiscriminadamente.

## Operação
Defina sincronização de relógios, retenção, acesso por função e monitoramento de saúde dos componentes. Agente desconectado é um sinal de perda de visibilidade, não prova de comprometimento.

## Grafana
Etapa futura: consultar indicadores com identidade de leitura e validar compatibilidade de versões, índice e esquema. Não há datasource, dashboard Grafana nem integração concluída neste repositório.
