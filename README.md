# Nginx for PS1.7 & Debian 9
Nginx configuration for prestashop 1.7
You don't have redirect any url, Prestashop magage them perfectly, just enable SSL in PS.

This config looks to be really faster than in Apache (but I didn't benchmarck them to give a measure of improvement).
Admin isn't in SSL, any help is welcome.

# Nginx conf v1 - Every thing looks working
Added :
  - SSL


# Nginx conf v2 - Needs to do some tinkering but it's working
Added :
  - Static server (for cookie free domaine)
  - Gzip compression



# Nginx sources from
https://www.howtoforge.com/tutorial/how-to-install-nginx-with-php-and-mysql-lemp-on-debian-9/
https://www.digitalocean.com/community/questions/how-to-set-up-nginx-cookie-free-headers
https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-with-http-2-support-on-ubuntu-16-04
https://www.prestashop.com/forums/topic/519123-config-prestashop-17-and-nginx/
https://gist.github.com/prestarocket/5280139/1fcb2ee08012631b1aaa9d70c254e597d1d38196

# SSL sources from
https://medium.com/@jgefroh/a-guide-to-using-nginx-for-static-websites-d96a9d034940

# Opchace sources from
https://gist.github.com/yugenekr/8e1885887d10b0d9ddc92beca9a52d93
https://www.scalingphpbook.com/blog/2014/02/14/best-zend-opcache-settings.html
