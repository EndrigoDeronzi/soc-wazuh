# Coleta Windows em laboratório
O fragmento em [windows-eventchannels.xml](../config/windows-eventchannels.xml) ilustra coleta dos canais Security, System e Application com formato eventchannel.

1. Instale e registre o agente em um laboratório próprio.
2. Consulte a configuração existente: esses canais podem já estar configurados.
3. Faça cópia da configuração e incorpore somente os blocos necessários dentro de ossec_config. O fragmento não é um arquivo completo para substituição.
4. Valide permissões e política de auditoria Windows. Coleta não habilita automaticamente a geração de todos os eventos.
5. Aplique a alteração e reinicie o serviço do agente conforme o procedimento da versão instalada.
6. Gere um evento benigno e autorizado em uma conta de teste; confira o registro Windows e a recepção no Wazuh.
7. Confira também filtros, decoders e regras: um evento coletado pode não gerar alerta.
8. Registre timestamp, canal, host fictício e resultado da validação.

Não provoque bloqueios de contas de produção para demonstrar detecção.

Fonte: [documentação oficial de coleta](https://documentation.wazuh.com/current/user-manual/capabilities/log-data-collection/configuration.html).
