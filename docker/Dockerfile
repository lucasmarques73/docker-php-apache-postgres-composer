FROM php:7.2-apache

LABEL Lucas Marques <lucasmarques73@hotmail.com>

RUN apt-get update  

RUN apt-get install -y libpq-dev \
        			   zlib1g-dev \
        			   curl \
        			   libcurl3 \
                       libcurl3-dev

RUN docker-php-ext-install pdo pdo_pgsql zip mbstring curl

RUN a2enmod rewrite

COPY app.conf /etc/apache2/sites-enabled/app.conf