FROM nginx:stable-alpine
MAINTAINER Etienne Dauvergne <contact@ekyna.com>

ARG gid
ARG uid

RUN groupmod -g $gid \
 && usermod -u $uid -h /var/www www-data
 && mkdir /var/www/web \
 && chown -Rf www-data:www-data /var/www \
 && chmod -Rf 755 /var/www/web

WORKDIR /var/www
