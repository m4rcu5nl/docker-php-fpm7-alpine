[![Build Status](https://travis-ci.org/m4rcu5nl/docker-php-fpm7-alpine.svg?branch=master)](https://travis-ci.org/m4rcu5nl/docker-php-fpm7-alpine) [![GitHub issues](https://img.shields.io/github/issues/m4rcu5nl/docker-php-fpm7-alpine.svg)](https://github.com/m4rcu5nl/docker-php-fpm7-alpine/issues)  
docker-php-fpm7-alpine
======================
This image is created for use with my lighttpd image. It is, however, a pretty straight forward generic php-fpm7 image. Use it as you please.  

Build example
-------------
```
docker build -t php-fpm7 .
```

Run example
-----------
```
docker run \
	--detach \
	--name php-fpm7 \
	-v /absolute/path/to/docroot/on/host:/var/www/localhost/htdocs:rw \
	php-fpm7
```
The above creates a detached container named *php-fpm7* and mounts a directory from the host's filesystem as a volume to the designated docroot inside the container.  
