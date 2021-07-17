FROM php:7.4-fpm-alpine

RUN apk --update add \
    git \
    unzip \
    nodejs npm

RUN docker-php-ext-install pdo pdo_mysql

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /app
