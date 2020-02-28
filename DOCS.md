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

