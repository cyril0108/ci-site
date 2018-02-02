# Docker Compose
http://geekyplatypus.com/making-your-dockerised-php-application-even-better/
https://blog.shameerc.com/2016/08/my-docker-setup-ubuntu-php7-fpm-nginx-and-mariadb
https://www.newmediacampaigns.com/blog/docker-for-php-developers

# Install PHP extention
https://stackoverflow.com/questions/37527803/how-to-install-extension-for-php-via-docker-php-ext-install
https://stackoverflow.com/questions/40949752/docker-install-pdo-driver-for-php-nginx

RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev libpq-dev \
&& rm -rf /var/lib/apt/lists/* \
&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql



# Install nodejs
https://askubuntu.com/questions/720784/how-to-install-latest-node-inside-a-docker-container

update apt-get update
install curl apt-get install curl
get install script and pass it to execute: curl -sL https://deb.nodesource.com/setup_4.x | bash
and install node apt-get install nodejs
confirm that it was successful node -v npm installs automatically npm -v

use curl -sL https://deb.nodesource.com/setup_5.x | bash for node 5.x
use curl -sL https://deb.nodesource.com/setup_6.x | bash for node 6.x


