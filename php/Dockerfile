FROM php:8.1.19-fpm as php
WORKDIR /usr/src/myapp
COPY ./index.php ./

RUN apt-get update && apt-get install -y \
    git \
    zip \
    unzip \
    && docker-php-ext-install pdo_mysql mysqli \
    && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer


CMD [ "php", "./index.php" ] 