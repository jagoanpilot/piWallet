piWallet
========

piWallet is a popular secure opensource online altcoin wallet that works with practically any altcoin. piWallet uses PHP, mySQL, JavaScript and Bootstrap meaning it's quite simple to setup. 

Setup: 
Ubuntu 18 use php 7.2

Ubuntu 20 use php 7.4

sudo apt-get install apache2

sudo apt-get install php7.4 php7.4-mysql php7.4-gd

sudo apt-get install mysql-server 

sudo mysql -u root -p

CREATE database tutor_db;

CREATE USER 'test_tutor'@'localhost' IDENTIFIED WITH mysql_native_password BY 'walletpassword';

GRANT ALL PRIVILEGES ON tutor_db.* TO 'test_tutor'@'localhost';

FLUSH PRIVILEGES;

QUIT;

sudo apt install -y php-json php-mbstring php-zip php-gd php-curl

sudo apt install -y phpmyadmin

sudo ln -s /etc/phpmyadmin/apache.conf /etc/apache2/conf-available/phpmyadmin.conf

sudo a2enconf phpmyadmin.conf

sudo systemctl restart apache2

git clone https://github.com/jagoanpilot/piWallet

sudo mv piWallet/* /var/www/html/

change with your own captcha

https://www.google.com/recaptcha/admin/

privatekey  6LdAUnIUAAAAAAGBh18wU2yviS6NTjOTOyDn8g //index.php

Publickey 6LdAUnIUAAAAAIOylmQeQkZUbec1B75sYJo8veKo //home.php

Running Daemon with -daemon -deprecatedrpc=accounts for bitcoin v17

sample daemon configuration

rpcuser=typerandomuser

rpcpassword=typerandompassword

rpcport=17898

rpcallowip=127.0.0.1

server=1

daemon=1

txindex=1


TODO: Add a step in the wiki explaining to copy settings-example.php into a new file settings.php and then change the values.

Bitcoin Talk Thread: https://bitcointalk.org/index.php?topic=911212

Please exercise EXTREME CAUTION when having a 3rd party install piWallet, please see https://fittechhosting.com/cryptocurrency for approved installation/piWallet hosting services. 

I can be reached directly at jmartin@FitTechHosting.com

Features:

- Manual User Reserve

- QR Codes use a local generation URL 

- Multilanguage support for over 90% of text - Currently supported languages include English, Greek, Mandarin, Hindi, Italian, Portuguese, Spanish, and Tagalog.

- QR Codes for Addresses

- Google 2 Factor Auth

- Mobile App (Additional Addon - see https://FitTechHosting.com/cryptocurrency )

- Fee Sent to Wallet Owner (Included w/ Hosting - https://FitTechHosting.com/cryptocurrency)

Planned Features:

- Have QR Codes open in lightbox instead of new tab

- Control of Private Keys

- Improved Bootstrap Theme 

Todo List:

- Issue #78 - PHP Juggling 

- Issue #82 - Strip tags bug

- Issue #83 - change default password from changeme

- Issue #36  Stop using md5

- Change background from ugly yellow

 
More Information:

Created by Johnathan Martin of FitTechHosting.com
