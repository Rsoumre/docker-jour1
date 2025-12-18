# Image Nginx officielle
FROM nginx:alpine

# Supprimer la config par défaut
RUN rm -rf /usr/share/nginx/html/*

# Copier les fichiers du jeu
COPY index.html /usr/share/nginx/html/
COPY save.php /usr/share/nginx/html/

# Copier les fichiers persistants dans le volume
VOLUME /usr/share/nginx/html/data

# Exposer le port 80
EXPOSE 80
