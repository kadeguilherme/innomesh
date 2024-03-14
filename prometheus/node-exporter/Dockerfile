# Use uma imagem base do node-exporter
FROM nginx/nginx-prometheus-exporter:latest

# Adicione o argumento --nginx.scrape-uri ao CMD
ENTRYPOINT ["/usr/bin/nginx-prometheus-exporter", "--nginx.scrape-uri=http://nginx:80/status"]