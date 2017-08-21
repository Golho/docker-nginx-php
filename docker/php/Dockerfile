# Nginx and PHP image with phpCAS lib installed and modified
FROM php:7-fpm
RUN docker-php-ext-install mysqli
RUN apt-get update && apt-get install -y php-cas
RUN sed -i "s/= \$_SERVER\['SERVER_NAME'\]/= \$_SERVER\['HTTP_HOST'\]/" /usr/share/php/CAS/Client.php
