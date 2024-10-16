FROM nginx:latest

# Rimuovi la configurazione predefinita di Nginx
RUN rm -rf /etc/nginx/conf.d/default.conf

# Copia il file di configurazione personalizzato
COPY nginvproapp.conf /etc/nginx/conf.d/vproapp.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]



