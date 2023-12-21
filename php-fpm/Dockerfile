FROM php:8.3-fpm-alpine

# make folder can edit
RUN chown -R 777 /var/www/html

RUN apk update

RUN apk add libpng libpng-dev libjpeg-turbo-dev libwebp-dev zlib-dev libxpm-dev gd && docker-php-ext-install gd

# Install mysql driver & gd
RUN docker-php-ext-install pdo pdo_mysql gd

# expose port 9000 and start php-fpm server
EXPOSE 9000

CMD ["php-fpm"]
