# Ubuntu-OS-Setup
Step by step guide in setting up ubuntu for Web Development using PHP and Laravel

## First things first before anything else
Run this command first
``` bash
sudo apt update
sudo apt install
```
This will update all necessary files in ubuntu
## Installing VS Code
1.) Download VS Code at https://code.visualstudio.com/ <br>
2.) After downloading, go to your downloads directory
``` bash
cd Downloads
```
3.) Install vs code
``` bash
sudo dpkg -i code_1.63.2-1639562499_amd64.deb
```
4.) Now look for the VS Code app in the application menu after installation.

## Installing XAMPP
1.) Download xampp at https://www.apachefriends.org/ <br>
2.) After downloading xampp, go to your downloads directory
``` bash
cd Downloads
```
3.) Change the permission of the installer. 755 means read and execute access for everyone and write access to the owner of the file.
``` bash
chmod 755 your_xampp_installer_file_name
```
4.) Begin to install XAMPP
``` bash
sudo ./your_xampp_installer_file_name
```
## To open and run XAMPP
``` bash
sudo /opt/lampp/./manager-linux-x64.run
```
5.) After installing XAMPP run this command:
``` bash
sudo apt-get install -y php php-cli php-common php-fpm php-mysql php-zip php-gd php-mbstring php-curl php-xml php-bcmath openssl php-json php-tokenizer
```
This will install all the necessary PHP extensions.

### Install Composer
Run each of this commands
``` bash
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'e21205b207c3ff031906575712edab6f13eb0b361f2085f1f1237b7126d785e826a450292b6cfd1d64d92e6563bbde02') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```
Finally move the composer.phar to /usr/local/bin/composer
```
sudo mv composer.phar /usr/local/bin/composer
```
