#PACKAGE INSTALLATION
sudo apt install nginx
sudo apt install mariadb-server
sudo apt install mariadb-client
sudo apt install php7.2
sudo apt install php7.2-fpm
#START SERVICE
sudo service nginx start
sudo service mysql start
sudo service php7.2-fpm start
#TEST IP ADDRESS
curl -4 icanhazip.com
#POST-INSTALLATION SCRIPT
sudo mysql_secure_installation
sudo mariadb


#NGIX SERVER SETUP
#LOCATE CONFIG FILE
cd /etc/nginx/sites-available
#DUPLICATE CONFIG FILE
cp -t ~/.git default
#RENAME CONFIG FILE
mv -T default midtest
#EDIT CONFIG
nano midtest
#TEST CONFIG
sudo nginx -t
#CHANGE DIRECTORY
cd /var/www/html/
#TEST SERVER
nano info.php
#REMOVE TEST FILE
rm -rf info.php

