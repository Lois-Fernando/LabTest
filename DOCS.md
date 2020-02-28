- install git
- sudo apt install nginx
- sudo apt install mariadb-server
- sudo apt install mariadb-client
- sudo apt install php7.2
- sudo apt install php7.2-fpm
- sudo systemctl status nginx
- sudo systemctl status mysql
- sudo systemctl status mariadb-server
- sudo install curl
- curl -4 icanhazip.com
- sudo mysql_secure_installation
- sudo mariadb
- exit;


- sudo cp /etc/nginx/sites-available/default /etc/nginx/sites-available/midtest
	remove the test
	add index.php before index.html
	uncomment location ~ \.php$ and keep the PHP-CGI line commented change the
	FPM version from 7.0 to 7.2
- sudo nginx -t
- sudo ln -s /etc/nginx/sites-available/midtest /etc/nginx/sites-enabled/
- sudo unlink /etc/nginx/sites-enabled/default
- sudo systemctl reload nginx
- sudo nano /var/www/html/info.php
- access localhost/info.php

