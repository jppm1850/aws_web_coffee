# coffee-website
# aws_web_coffee


#Configuration
sudo su
sudo apt-get update
sudo apt-get install php libapache2-mod-php -y
sudo apt-get install php-mysqli -y
cd /home/ubuntu
git clone https://github.com/jbarreto7991/aws_web_coffee.git
cd /home/ubuntu/aws_web_coffee
cp -r * /var/www/html
sudo /etc/init.d/apache2 restart


#Edit php.ini
cd /etc/php/7.2/apache2/
chown 777 php.ini
nano php.ini
extension=mysqli


#Modify /var/www/html/Model/Credentials.php
nano /var/www/html/Model/Credentials.php
$host
