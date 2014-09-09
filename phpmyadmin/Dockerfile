FROM apache2

RUN apt-get install -y mysql-client
RUN apt-get install -y php5 php5-mysql libapache2-mod-php5
RUN apt-get install -y wget

RUN rm -rf /var/www

RUN wget --no-check-certificate http://github.com/phpmyadmin/phpmyadmin/archive/master.tar.gz
RUN tar -C /var -xvf master.tar.gz
RUN mv /var/phpmyadmin-master /var/www
