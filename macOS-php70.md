#Step install install PHP7.0 with imap and mcrypt in macOS
```bash
brew install openssl
#Download php source from http://php.net/downloads.php and extract
cd php-7.0.x
./configure --with-mysqli --with-mcrypt --with-gd --with-imap --with-imap-ssl --with-kerberos --with-openssl=/usr/local/opt/openssl --enable-mbstring --with-curl  --enable-bcmath --enable-pcntl --with-libedit --with-pear --enable-zip
make
sudo make install
cp php.ini-development /usr/local/php/php.ini

```
