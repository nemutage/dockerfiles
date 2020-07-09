FROM php:7.4-apache

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/bin/
RUN install-php-extensions bz2 curl fileinfo gd gettext intl mbstring exif mysqli pdo_mysql pdo_sqlite openssl ftp xdebug

RUN a2enmod rewrite