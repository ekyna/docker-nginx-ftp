FROM nginx:stable-alpine
MAINTAINER Etienne Dauvergne <contact@ekyna.com>

RUN addgroup www-data -g 1000 \
 && adduser -D -u 1000 -h /var/www -G www-data www-data \
 && mkdir /var/www/web \
 && chown -Rf www-data:www-data /var/www/web \
 && chmod -Rf 755 /var/www/web

WORKDIR /var/www
