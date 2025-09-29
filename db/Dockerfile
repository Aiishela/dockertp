FROM postgres:16

# Variables d’environnement
ENV POSTGRES_HOST_AUTH_METHOD=trust

# Copie du script SQL d’initialisation
COPY words.sql ./docker-entrypoint-initdb.d/
# EXPOSE 5432
