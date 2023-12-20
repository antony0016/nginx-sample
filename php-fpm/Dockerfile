FROM php:8.3-fpm-alpine

# make folder can edit
RUN chown -R 777 /var/www/html

# Install mysql driver
RUN docker-php-ext-install pdo pdo_mysql

# expose port 9000 and start php-fpm server

EXPOSE 9000

CMD ["php-fpm"]
