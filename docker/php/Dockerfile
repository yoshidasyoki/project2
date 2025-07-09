FROM php:8.2-apache

WORKDIR /var/www/html

RUN apt-get update && apt-get install -y \
    libonig-dev \
    && docker-php-ext-install pdo_mysql mysqli mbstring \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

EXPOSE 80
