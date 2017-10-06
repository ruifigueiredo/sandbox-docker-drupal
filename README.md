sandbox-docker
===============

Simple Development Sandbox for Drupal with Docker

Summary:
--------

* Apache 2.4
* MariaDB 10.1
* PHP 7.0
* The latest release of Drupal Console
* Composer
* PHPMyAdmin


How To:
-------

- $: `docker-compose build`
- $: `docker-compose up -d`
- $: `sudo ifconfig en0 alias 10.254.254.254 255.255.255.0 #Linux and MAC`
- $: `docker-compose stop` # stop sandbox

Remove:
-------

- $: `docker-compose down`


PhpStorm Settings:
-----------------

- `Settings > Languages & Framework > PHP > Debug > DBGp Proxy`
- `IDE key: PHPSTORM`
- `Host: 10.254.254.254`
- `Port: 9000`

- `Go to RunDebug Configurations`
- `Add PHP Web Application`
- `Add new server`
- `Add localhost to server`
- `Use path mappings`
- `Create project mapping with server, ex: the dir  D:/web/www/drupal is on the server path /var/www/drupal `
- `Add the source of drupal project using drupal console or download the source from drupal.org`
