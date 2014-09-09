FROM apache2

RUN apt-get install -y mysql-client
RUN apt-get install -y php5 php5-mysql libapache2-mod-php5
RUN apt-get install -y wget

RUN rm -rf /var/www

RUN wget --no-check-certificate http://github.com/phpmyadmin/phpmyadmin/archive/RELEASE_4_2_8.tar.gz
RUN tar -C /var -xvf RELEASE_4_2_8.tar.gz
RUN mv /var/phpmyadmin-RELEASE_4_2_8 /var/www

COPY config.inc.php /var/www
