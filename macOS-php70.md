# Step to install PHP 7.0 with imap, mcrypt, mbstring, curl, bcmath in macOS

```bash
brew install openssl

#Download php source from http://php.net/downloads.php and extract
cd php-7.0.x
./configure --with-mysqli --with-mcrypt --with-gd --with-imap --with-imap-ssl --with-kerberos --with-openssl=/usr/local/opt/openssl --enable-mbstring --with-curl  --enable-bcmath --enable-pcntl --with-libedit --with-pear --enable-zip
make
sudo make install
cp php.ini-development /usr/local/lib/php.ini

#Install MongoDB
sudo pecl install mongodb
code /usr/local/lib/php.ini
#add extention=mongodb.so
php -i|grep mongo
```
