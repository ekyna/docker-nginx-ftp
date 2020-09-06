FROM nginx:stable-alpine
MAINTAINER Etienne Dauvergne <contact@ekyna.com>

ARG gid
ARG uid

RUN apk --no-cache add shadow \
 && mkdir -p /var/www/web \
 && groupmod -g $gid www-data \
 && adduser -D -u $uid -h /var/www -G www-data www-data \
 && chown -Rf www-data:www-data /var/www \
 && chmod -Rf 755 /var/www/web

WORKDIR /var/www
