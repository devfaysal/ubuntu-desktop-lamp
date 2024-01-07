## Apache
- ```sudo apt update```
- ```sudo apt install apache2```

## MySQL
- ```sudo apt install mysql-server```
- ```sudo mysql```
- ```ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';```
- ```exit```
- ```sudo mysql_secure_installation```

## PHP
- ```sudo apt-get install ca-certificates apt-transport-https software-properties-common wget curl lsb-release -y```
- https://launchpad.net/~ondrej/+archive/ubuntu/php/
- ```sudo add-apt-repository ppa:ondrej/php```
- In case of WARNING: add-apt-repository is broken with non-UTF-8 locales ```sudo LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php```
- ```sudo apt update```
- ```sudo apt install php8.1 php8.1-cli php8.1-fpm php8.1-bcmath php8.1-curl php8.1-gd php8.1-intl php8.1-mbstring php8.1-mysql php8.1-opcache php8.1-sqlite3 php8.1-xml php8.1-zip libapache2-mod-php8.1 php8.1-common```

## Node.js and npm
https://stackoverflow.com/a/66166866/6150983
- Download the latest stable version of node from https://nodejs.org/en
- Go to the directory where the file was downloaded
- ```sudo apt update```
- ```sudo apt install xz-utils```
- ```sudo tar -xvf node-v20.10.0-linux-x64.tar.xz``` (Filename is different based on version)
- ```sudo cp -r node-v20.10.0-linux-x64.tar.xz/{bin,include,lib,share} /usr/```
- ```node --version```
