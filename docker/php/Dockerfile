FROM php:7-apache
COPY php.ini /usr/local/etc/php/
RUN apt-get update && apt-get install -y \
    libfreetype6-dev libjpeg62-turbo-dev libmcrypt-dev libzip-dev zlib1g-dev libicu-dev libxml2-dev\
    git vim \
    && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv zip intl soap xmlrpc opcache\
    && apt-get clean
# install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
# Create a data directly
RUN mkdir /var/www/moodledata
RUN chown -R www-data /var/www/moodledata