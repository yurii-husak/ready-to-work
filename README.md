# Ready to work

***

## Required to install

- PHPStorm ([Download](https://www.jetbrains.com/phpstorm/download/))
- NodeJS (16.*) ([Download](https://nodejs.org/en/blog/release/v16.16.0/))
- Yarn (run the code below via cmd, PowerShell or git bash)

```bash
npm install --global yarn 
```

- XAMPP ([Download](https://www.apachefriends.org/download.html))
- PHP (7.4.*) ([Download](https://windows.php.net/download/))
- Composer ([Download](https://getcomposer.org/download/))

***

## Prepare PHPStorm

-  PHPStorm Settings ([Download](https://www.apachefriends.org/download.html))

*To install PHPStorm setting go to the 'File -> Manage IDE Settings -> Import Settings'*

### Recommended plugins

- *coming soon...*

***

## Prepare Ubuntu 

- Ubuntu (v 22) ([Download](https://apps.microsoft.com/store/detail/ubuntu-22041-lts/9PN20MSR04DW?hl=uk-ua&gl=ua&rtc=1))

*Or you can download it via Microsoft Store

### Ubuntu - Required to install

- NodeJS (run the code below)

```bash
sudo apt update

curl -sL https://deb.nodesource.com/setup_16.x -o /tmp/nodesource_setup.sh

sudo bash /tmp/nodesource_setup.sh

sudo apt install nodejs

node -v
```

*For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04)*

- Yarn (run the code below)

```bash
sudo apt update

sudo apt install yarn

sudo apt install --no-install-recommends yarn

yarn --version
```

*For more instructions follow the [link](https://linuxize.com/post/how-to-install-yarn-on-ubuntu-20-04/)*

- PHP 7.4 (run the code below)

```bash
sudo apt-get update

sudo apt -y install software-properties-common

sudo add-apt-repository ppa:ondrej/php

sudo apt-get update

sudo apt -y install php7.4

sudo apt-get install -y php7.4-cli php7.4-json php7.4-common php7.4-mysql php7.4-zip php7.4-gd php7.4-mbstring php7.4-curl php7.4-xml php7.4-bcmath

php -v
```

*For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-php-7-4-and-set-up-a-local-development-environment-on-ubuntu-20-04)*

- Composer (run the code below)

```bash
sudo apt update

curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php

HASH=`curl -sS https://composer.github.io/installer.sig`

php -r "if (hash_file('SHA384', '/tmp/composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"

sudo php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer

composer --version
```

*For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-20-04)*