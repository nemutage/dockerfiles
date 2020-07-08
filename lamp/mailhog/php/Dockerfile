FROM golang:1.14 as builder
RUN go get github.com/mailhog/mhsendmail

FROM php:7.4-apache
COPY --from=builder /go/bin/mhsendmail /usr/bin/mhsendmail
COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/bin/
RUN install-php-extensions bz2 curl fileinfo gd gettext intl mbstring exif mysqli pdo_mysql pdo_sqlite openssl ftp xdebug

