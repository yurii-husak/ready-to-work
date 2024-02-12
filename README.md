# Ready to work

## Required to install

- Slack | ([Download](https://slack.com/downloads/windows))
- PHPStorm | ([Download](https://www.jetbrains.com/phpstorm/download/))
- GIT + GIT bash | ([Download](https://git-scm.com/downloads))
- NodeJS (16.*) | ([Download](https://nodejs.org/en/blog/release/v16.16.0/)) or NVM (latest version) | ([Download](https://github.com/coreybutler/nvm-windows/releases))
- Yarn. Run `npm install --global yarn` in your terminal (CMD, PowerShell or Git Bash)
- XAMPP | ([Download](https://www.apachefriends.org/download.html))
- PHP (7.4.*) | ([Download](https://windows.php.net/download/) or [Download](https://windows.php.net/downloads/releases/archives/))
- Composer | ([Download](https://getcomposer.org/download/))

_Notice:_ Instruction for NVM ([Link](https://github.com/coreybutler/nvm-windows))

## Prepare Windows

- Press `Win + R`
- Enter `optionalfeatures.exe`
- Enable: `Hyper-V` and `Windows Subsystem for Linux`

## GIT Configs

Open terminal or GIT bash and run next commands:

```bash
git config --global user.name "Your_Name"
```

```bash
git config --global user.email your_email@example.com
```

```bash
git config --global core.autocrlf input
```

## Prepare PHPStorm

-  PHPStorm Settings (with Live Templates) ([Download](https://drive.google.com/file/d/1XC8nwAMLlSwLr0vGjHoZV0YTEpDN_eJU/view?usp=sharing))

_To install PHPStorm setting go to the 'File -> Manage IDE Settings -> Import Settings'_

### Recommended plugins

- Atom Material Icons 
- CodeGlance Pro 
- Ideolog 
- Material Theme UI 
- Material Theme UI Lite 
- One Dark theme 
- Rainbow Brackets 
- Styled Components & Styled JSX

## Prepare Ubuntu 

### Contents

- [Ubuntu app](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#ubuntu-terminal)
- [LFTP](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#lftp)
- [NodeJS](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#nodejs)
- [Yarn](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#yarn)
- [PHP 7.4](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#php-7.4)
- [PHP 8.1](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#php-8.1)
- [Composer](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#composer)
- [SSHPASS](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#sshpass)
- [ZIP](https://github.com/yurii-husak/ready-to-work?tab=readme-ov-file#zip)

### Ubuntu terminal

- Ubuntu 22.04 ([Download](https://apps.microsoft.com/store/detail/ubuntu-22041-lts/9PN20MSR04DW?hl=uk-ua&gl=ua&rtc=1))

### LFTP

```bash
sudo apt update
```

```bash
sudo apt -y install lftp
```

_For more instructions follow the [link](https://installati.one/install-lftp-ubuntu-22-04/)_

### NodeJS

```bash
sudo apt update
```

```bash
sudo apt-get install -y ca-certificates curl gnupg
```

```bash
sudo mkdir -p /etc/apt/keyrings
```

```bash
curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg
```

```bash
NODE_MAJOR=16
```

> ***Optional***: ``NODE_MAJOR`` can be changed depending on the version you need.
>
> ```sh
> NODE_MAJOR=16
> NODE_MAJOR=18
> NODE_MAJOR=20
> NODE_MAJOR=21
> ```

```bash
echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_$NODE_MAJOR.x nodistro main" | sudo tee /etc/apt/sources.list.d/nodesource.list
```

```bash
sudo apt update
```

```bash
sudo apt-get install nodejs -y
```

```bash
node -v
```

_For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04)_

### Yarn

```bash
sudo apt update
```

```bash
sudo apt install curl
```

```bash
curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
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

```bash
sudo apt install npm
```

```bash
sudo curl --compressed -o- -L https://yarnpkg.com/install.sh | bash
```

```bash
yarn --version
```

_For more instructions follow the [link](https://linuxize.com/post/how-to-install-yarn-on-ubuntu-20-04/)_

### PHP 7.4

```bash
sudo apt update
```

```bash
sudo apt -y install software-properties-common
```

```bash
sudo add-apt-repository ppa:ondrej/php
```

```bash
sudo apt update
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

_For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-php-7-4-and-set-up-a-local-development-environment-on-ubuntu-20-04)_

### PHP 8.1

```bash
sudo apt update
```

```bash
sudo apt install --no-install-recommends php8.1
```

```bash
sudo apt-get install -y php8.1-cli php8.1-common php8.1-mysql php8.1-zip php8.1-gd php8.1-mbstring php8.1-curl php8.1-xml php8.1-bcmath
```

```bash
php -v
```

_For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-php-8-1-and-set-up-a-local-development-environment-on-ubuntu-22-04)_

### Composer

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

_For more instructions follow the [link](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-20-04)_

### SSHPASS

```bash
sudo apt update
```

```bash
sudo apt -y install sshpass
```

### ZIP

```bash
sudo apt update
```

```bash
sudo apt install zip unzip
```
