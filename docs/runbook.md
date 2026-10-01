# Roteiro de investigação e resposta
1. **Confirmar o sinal:** valide timestamp, origem, agente e integridade dos dados.
2. **Determinar alcance:** busque eventos correlatos na mesma conta, ativo e janela.
3. **Consultar contexto:** manutenção, mudanças aprovadas e criticidade.
4. **Classificar:** erro operacional, evento legítimo, suspeita ou incidente confirmado.
5. **Escalar:** encaminhe evidências e impacto ao responsável.
6. **Conter quando autorizado:** registre decisão, escopo e impacto da ação.
7. **Validar recuperação:** confirme serviço funcional, retomada da coleta e ausência de sinais relacionados.
8. **Encerrar:** registre causa, conclusão, lacunas e melhoria de detecção.

## Evidências mínimas
- Identificador do caso e horário com timezone.
- Host e conta do laboratório.
- Fonte, evento observado e consulta utilizada.
- Fatos separados de hipóteses.
- Responsável e ações autorizadas.
- Resultado e limitações.

Não isole um endpoint automaticamente apenas pela severidade. Este projeto não implementa Active Response ou SOAR.

## Indicadores propostos
Quantidade de casos por prioridade, tempo de triagem, casos encerrados por classificação e agentes sem comunicação. As definições e o período devem acompanhar cada indicador; não há métricas de produção neste repositório.
