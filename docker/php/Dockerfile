FROM php:fpm

RUN cd /usr/bin && curl -s http://getcomposer.org/installer | php && ln -s /usr/bin/composer.phar /usr/bin/composer\ 
&& apt-get -y update\
&& apt-get -y install git zip unzip vim libpq-dev && docker-php-ext-install pdo_mysql pdo_pgsql

WORKDIR /var/www/html
