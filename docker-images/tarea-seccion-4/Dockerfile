FROM centos:7

RUN \ 
  yum -y install \
  httpd \
  php \
  php-cli \
  php-common

RUN echo "<?php phpinfo(); ?>" > /var/www/html/index.php


RUN echo "hola" > /var/www/html/index.html

CMD apachectl -DFOREGROUND
