# Web Server
========================

## Setup
-----
```bash
zypper install httpd


systemctl start apache2
```

## Edit file config

```bash
vi /etc/apache2/conf.d/example.conf
```
```bash
<VirtualHost *:80>

ServerAdmin webmaster@.example.com

DocumentRoot /srv/www/htdocs/example

ServerName www.example.com

ErrorLog /var/log/apache2/example.com-error_log

CustomLog /var/log/apache2/example.com-access_log common

</VirtualHost>

```
change "ServerAdmin", "DocumentRoot", "ServerName"

## Document upload
Create directory
```bash
mkdir /srv/www/htdocs/example
```
create index.html, edit, and save file to /srv/www/htdoc
```bash
<html><body><h1>SUSE WEBSERVER Jogjacamp (IDWEBHOST)</h1></body></html>
```
