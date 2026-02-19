FROM debian:stable-slim

RUN apt update && apt install -y apache2 && apt clean

COPY config/apache2.conf /etc/apache2/apache2.conf
COPY html/ /var/www/html/

EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]
