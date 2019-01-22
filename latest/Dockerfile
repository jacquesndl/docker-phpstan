FROM phpstan/phpstan:0.10

RUN apk --update --progress --no-cache add \
    php7-dom \
    php7-xmlwriter

RUN composer global require phpstan/phpstan-phpunit phpstan/phpstan-symfony phpstan/phpstan-doctrine
RUN rm -rf /var/cache/apk/* /var/tmp/* /tmp/*

WORKDIR /app
ENTRYPOINT ["phpstan"]
