FROM php:8.3-fpm
RUN ln -snf /usr/share/zoneinfo/Europe/Moscow /etc/localtime && echo Europe/Moscow > /etc/timezone
WORKDIR /var/www
RUN docker-php-ext-install -j "$(nproc)" mysqli

CMD ["php-fpm"]
