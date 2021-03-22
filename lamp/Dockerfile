FROM ubuntu

RUN apt-get update &&  \
    DEBIAN_FRONTEND="noninteractive" apt-get -y install apache2 mysql-server php libapache2-mod-php php-mysql

EXPOSE 80

WORKDIR /var/www/html

CMD /etc/init.d/apache2 start && \
    /etc/init.d/mysql start && \
    /bin/bash