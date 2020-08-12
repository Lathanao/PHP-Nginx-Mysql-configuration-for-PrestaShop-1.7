# Server configuration files for PrestaShop 1.7

**PHP, FPM, Nginx, Mysql 8** Files configurations for PrestaShop 1.7.
Just need to copy past files or make some sim links.
Have to fill Nginx files with your shop domain. 
Php and FPM configuration is really light. 

Finally, it just works well enough for me.

## Directory tree
Most of the setup could be ajust again follow the machine you have. 
Just test before then adapt with your own setting. 

    .
    │
    ├── mysql
    │   └── mysql.cnf                               # Just a conf file
    │
    ├── nginx                                       # Test files (alternatively `spec` or `tests`)
    │   ├── sites-available                    
    │   │   ├── adminer.conf                        # Just a basic config for Adminer
    │   │   ├── nginx_example_for_PS16.conf         # Old conf for ps1.6, works for ThirtyBees
    │   │   └── nginx_example_for_PS17.conf         # Configuration for 1.7
    │   └── nginx.conf
    │
    └── php                                         # Just a light setting for Php
        └── 7.2
            ├── pool.d
            │   └── www.conf                        # Just a basic config for www pool
            ├── php.ini                             # Basic config for PHP
            └── php-fpm.conf                        # Basic config for FPM

## Credits / Resources

- **Nginx tutorials**:
  - https://www.digitalocean.com/community/tutorials/understanding-nginx-server-and-location-block-selection-algorithms
  - https://www.nginx.com/resources/wiki/start/topics/examples/full/
  - https://www.nginx.com/resources/wiki/start/topics/tutorials/config_pitfalls/
  - https://geekflare.com/http-header-implementation/
  
- **Nginx resources**:
  - https://www.howtoforge.com/tutorial/how-to-install-nginx-with-php-and-mysql-lemp-on-debian-9/
  - https://www.digitalocean.com/community/questions/how-to-set-up-nginx-cookie-free-headers
  - https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-with-http-2-support-on-ubuntu-16-04
  - https://www.prestashop.com/forums/topic/519123-config-prestashop-17-and-nginx/
  - https://gist.github.com/prestarocket/5280139/1fcb2ee08012631b1aaa9d70c254e597d1d38196
  - https://github.com/PrestaShop/PrestaShop/blob/develop/docs/server_config/nginx.conf.dist
  - https://docs.nextcloud.com/server/13.0.0/admin_manual/installation/nginx.html
  
- **Opcache resources**:
  - https://gist.github.com/yugenekr/8e1885887d10b0d9ddc92beca9a52d93
  - https://www.scalingphpbook.com/blog/2014/02/14/best-zend-opcache-settings.html
  - https://commaster.net/content/installing-php-fastcgi-and-zend-opcache-wampserver
  
- **SSL resources**:
  - https://medium.com/@jgefroh/a-guide-to-using-nginx-for-static-websites-d96a9d034940
