FROM alpine

# Instalamos cliente mysql, samba y mongo.
RUN apk add --no-cache mysql-client
RUN apk add --no-cache samba-client
RUN apk add --no-cache mongodb-tools

##### ZONA HORARIA #####
RUN apk add tzdata
RUN cp /usr/share/zoneinfo/America/Argentina/Buenos_Aires /etc/localtime
#########################

#Archivo de ejecución de cron
COPY crons/root /var/spool/cron/crontabs/root

#Copiamos los Scripts de Backups y Parametros
COPY crons/scripts /home/db-backups/scripts
RUN chmod +x /home/db-backups/scripts/backup

#Creamos Directorio dentro del contenedor para almacenar los Backups de manera temporal.
RUN mkdir /home/db-backups/dumps

CMD crond -l 2 -f