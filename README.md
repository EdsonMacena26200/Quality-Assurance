# Quality-Assurance
Trablaho de Quality Assurance
Monitoramento Contínuo de Performance 
Como funciona
A solução coleta métricas de tempo de resposta, latência, disponibilidade e taxa de erros usando Prometheus. Essas métricas são expostas via endpoints e coletadas periodicamente.
Como foi feito
Ferramentas propostas: Prometheus, Grafana e Locust/JMeter. Configuração de exporters, dashboards e regras de alerta. Testes de estresse executados com locust/jmeter contra endpoints críticos.
Como rodar (exemplo prático)
1. Instalar Prometheus e Grafana (ou usar docker-compose). 
2. Configurar targets no prometheus.yml. 
3. Deploy de exporters. 
4. Importar dashboards no Grafana. 
5. Executar locust/jmeter para testes.

Exemplo: (docker-compose):
 prometheus.yml with job targets
 docker-compose up -d prometheus grafana node-exporter
