FROM alpine

COPY crons/root /var/spool/cron/crontabs/root

##### ZONA HORARIA #####
# RUN apk add tzdata
# RUN cp /usr/share/zoneinfo/America/Argentina/Buenos_Aires /etc/localtime
#########################

CMD crond -l 2 -f