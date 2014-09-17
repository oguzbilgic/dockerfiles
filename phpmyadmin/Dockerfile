FROM oguzbilgic/apache2

RUN apt-get install -y mysql-client=5.5.38-0ubuntu0.12.04.1
RUN apt-get install -y php5=5.3.10-1ubuntu3.14
RUN apt-get install -y php5-mysql=5.3.10-1ubuntu3.14
RUN apt-get install -y libapache2-mod-php5=5.3.10-1ubuntu3.14
RUN apt-get install -y wget

RUN rm -rf /var/www

RUN wget --no-check-certificate http://github.com/phpmyadmin/phpmyadmin/archive/RELEASE_4_2_8.tar.gz
RUN tar -C /var -xvf RELEASE_4_2_8.tar.gz
RUN mv /var/phpmyadmin-RELEASE_4_2_8 /var/www

ADD config.inc.php /var/www/
