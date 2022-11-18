FROM registry.ehw2.net/cz-app-base:05d1ecc412748b1e AS builder
RUN mkdir -p /App/Web && echo "<?php phpinfo();" > /App/Web/index.php
#COPY ./php-fpm.conf /usr/local/etc/php-fpm.conf
WORKDIR /App
