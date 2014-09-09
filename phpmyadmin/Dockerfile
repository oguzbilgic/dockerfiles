FROM apache2

RUN apt-get install -y mysql-client
RUN apt-get install -y php5 php5-mysql libapache2-mod-php5

RUN rm /var/www/index.html

RUN curl -O https://github.com/phpmyadmin/phpmyadmin/archive/master.tar.gz
RUN tar -xvf master.tar.gz /var/www/
