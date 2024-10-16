FROM mysql:8.0.33
LABEL "Project"="vprofile"
LABEL "Author"="Denis"

# Copia il file di backup SQL nella directory di inizializzazione di Docker
ADD  db_backup.sql /docker-entrypoint-initdb.d/
# non c'è differenza se scrivo COPY db_backup.sql /docker-entrypoint-initdb.d/
# Entrambe le versioni copieranno il file db_backup.sql nella directory /docker-entrypoint-initdb.d/ dell'immagine.


# Espone la porta standard di MySQL
EXPOSE 3306

# Il comando predefinito per avviare MySQL
CMD ["mysqld"]