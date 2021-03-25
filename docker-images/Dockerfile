FROM centos:7

LABEL version=1.0
LABEL description="This is an apache image"
LABEL vendor="Nahuel Bentos"

RUN yum install httpd -y 

COPY startbootstrap-freelancer-master /var/www/html

RUN echo "${whoami}" > /var/www/html/user1.html

RUN useradd nahuel

RUN chown nahuel /var/www/html/

USER nahuel

RUN echo "${whoami}" > /var/www/html/user2.html

CMD  apachectl -DFOREGROUND

 