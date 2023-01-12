# Ready to work

## Required to install

- PHPStorm ([Download](https://www.jetbrains.com/phpstorm/download/))
- GIT ([Download](https://git-scm.com/downloads))
- NodeJS (16.*) ([Download](https://nodejs.org/en/blog/release/v16.16.0/))
- Yarn (run the code below via cmd, PowerShell or git bash)

```bash
npm install --global yarn 
```

- XAMPP ([Download](https://www.apachefriends.org/download.html))
- PHP (7.4.*) ([Download](https://windows.php.net/download/))
- Composer ([Download](https://getcomposer.org/download/))

## Prepare Windows

- Press `Win + R`
- Enter `optionalfeatures.exe`
- Enable: `Hyper-V` and `Windows Subsystem for Linux`

## Prepare PHPStorm

-  PHPStorm Settings ([Download](https://www.apachefriends.org/download.html))

*To install PHPStorm setting go to the 'File -> Manage IDE Settings -> Import Settings'*

### Recommended plugins

- *coming soon...*

## Prepare Ubuntu 

- Ubuntu (v 22) ([Download](https://apps.microsoft.com/store/detail/ubuntu-22041-lts/9PN20MSR04DW?hl=uk-ua&gl=ua&rtc=1))

### Ubuntu - Required to install

- NodeJS (run the code below)

```bash
sudo apt update
```

```bash
curl -sL https://deb.nodesource.com/setup_16.x -o /tmp/nodesource_setup.sh
```

```bash
sudo bash /tmp/nodesource_setup.sh
```

```bash
sudo apt install nodejs
```

```bash
node -v
```

*For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04)*

- Yarn (run the code below)

```bash
sudo apt update
```

```bash
sudo apt install yarn
```

```bash
sudo apt install --no-install-recommends yarn
```

```bash
yarn --version
```

*For more instructions follow the [link](https://linuxize.com/post/how-to-install-yarn-on-ubuntu-20-04/)*

- PHP 7.4 (run the code below)

```bash
sudo apt-get update
```

```bash
sudo apt -y install software-properties-common
```

```bash
sudo add-apt-repository ppa:ondrej/php
```

```bash
sudo apt-get update
```

```bash
sudo apt -y install php7.4
```

```bash
sudo apt-get install -y php7.4-cli php7.4-json php7.4-common php7.4-mysql php7.4-zip php7.4-gd php7.4-mbstring php7.4-curl php7.4-xml php7.4-bcmath
```

```bash
php -v
```

*For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-php-7-4-and-set-up-a-local-development-environment-on-ubuntu-20-04)*

- Composer (run the code below)

```bash
sudo apt update
```

```bash
curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php
```

```bash
HASH=`curl -sS https://composer.github.io/installer.sig`
```

```bash
php -r "if (hash_file('SHA384', '/tmp/composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
```

```bash
sudo php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer
```

```bash
composer --version
```

*For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-20-04)*