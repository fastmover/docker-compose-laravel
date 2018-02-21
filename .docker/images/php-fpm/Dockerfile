FROM php:7.2.2-fpm

RUN apt-get update && apt-get install -y \
    apt-utils \
    libmcrypt-dev  \
    libicu-dev \
    mysql-client \
    && pecl install xdebug \
    && docker-php-ext-install ctype \
    && docker-php-ext-install iconv \
    && docker-php-ext-install intl \
    && docker-php-ext-install json \
    && docker-php-ext-install mbstring \
    && docker-php-ext-install opcache \
    && docker-php-ext-install pdo_mysql \
    && docker-php-ext-install tokenizer \
    && docker-php-ext-install xml

CMD ["php-fpm"]
