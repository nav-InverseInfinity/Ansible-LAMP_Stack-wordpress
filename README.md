# Ansible-LAMP_Stack-wordpress


## Create wordpress config
``` bash
sudo vi /etc/httpd/conf.d/wordpress.conf
```
```bash

<VirtualHost *:80>
        ServerAdmin root@localhost
        DocumentRoot /var/www/html/wordpress
  <Directory "/var/www/html/wordpress">
          Options Indexes FollowSymLinks
          AllowOverride all
          Require all granted
  </Directory>
        ErrorLog /var/log/httpd/wordpress_error.log
        CustomLog /var/log/httpd/wordpress_access.log common
</VirtualHost>

```
