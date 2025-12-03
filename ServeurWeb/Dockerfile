# Utiliser l'image officielle Nginx
FROM nginx:alpine

# Supprimer la config par défaut
RUN rm /etc/nginx/conf.d/default.conf

# Copier notre configuration nginx
COPY nginx.conf /etc/nginx/conf.d/

# Copier la page web dans le dossier par défaut de nginx
COPY src/ /usr/share/nginx/html/

# Expose port 80
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

