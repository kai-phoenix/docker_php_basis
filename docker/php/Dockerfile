FROM php:8.2-apache

#apache,phpの設定ファイルコピー
COPY ./docker/php/php.ini /etc/opt/remi/php82/php.ini
COPY ./docker/apache/vhost.conf /etc/httpd/conf.d/vhost.conf
COPY ./docker/apache/rewrite.conf /etc/httpd/conf.modules.d/rewrite.conf

RUN a2enmod rewrite \
&& service apache2 restart

WORKDIR /var/www/html/