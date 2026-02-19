FROM alpine:latest

RUN apk add --no-cache apache2

COPY config/apache2.conf /etc/apache2/httpd.conf
COPY html/ /var/www/localhost/htdocs/

EXPOSE 80

CMD ["httpd", "-D", "FOREGROUND"]
