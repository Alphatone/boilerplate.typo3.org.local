## Instructions for typo3.org template

go to root folder and type `docker-compose up'

When Docker-Boilerplate is running, open `http://localhost:8000/adminer.php`

enter the following:

user: dev

password: dev

host: mysql

db: typo3

In Adminer import this sql file:

https://drive.google.com/drive/folders/0B2tXMxwFfrK6ckxCRXoyb3RuQzg?usp=sharing

Then go to your terminal and cd into app

In app do a `composer install`


When done, you cd into app/html/typo3conf/ext/t3olayout/Private 

and run `npm install`

You will then have the Grunt-Tasks ready to compile CSS and JS needed. 

The user for the backend can be found in the official TYPO3.org Docker.
You will find this repo in gitlab. In the project itself there is an .env file where the user t3o can be found.



##This is based on TYPO3 docker boilerplate from WEBDEVOPS


![TYPO3 Docker Boilerplate](https://static.webdevops.io/typo3-docker-boilerplate.svg)

[![latest v5.2.0-beta3](https://img.shields.io/badge/latest-v5.2.0_beta3-green.svg?style=flat)](https://github.com/webdevops/TYPO3-docker-boilerplate/releases/tag/5.2.0-beta3)
![License MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)

This is an easy customizable TYPO3 docker boilerplate.

Supports:

- Nginx or Apache HTTPd
- PHP-FPM (with Xdebug)
- MySQL, MariaDB or PerconaDB
- PostgreSQL
- Solr (disabled, without configuration)
- Elasticsearch (disabled, without configuration)
- Redis (disabled)
- Memcached (disabled)
- Mailcatcher (if no mail sandbox is used, eg. [Vagrant Development VM](https://github.com/webdevops/vagrant-development))
- FTP server (vsftpd)
- PhpMyAdmin
- Support for `TYPO3_CONTEXT` and `FLOW_CONTEXT` for TYPO3, FLOW, NEOS.
- maybe more later...

This Docker boilerplate is based on the [Docker best practices](https://docs.docker.com/articles/dockerfile_best-practices/) and doesn't use too much magic. Configuration of each docker container is available in the `docker/` directory - feel free to customize.

This boilerplate can also be used for any other web project. Just customize the makefile for your needs.

*Warning: There may be issues when using it in production.*

If you have any success stories please contact me.

You can use my [Vagrant Development VM](https://github.com/mblaschke/vagrant-development) for this Docker boilerplate, e.g. for easily creating new boilerplate installations with short shell command: `ct docker:create directory`.

## Table of contents

- [First steps / Installation and requirements](/documentation/INSTALL.md)
- [Updating docker boilerplate](/documentation/UPDATE.md)
- [Customizing](/documentation/CUSTOMIZE.md)
- [Services (Webserver, MySQL... Ports, Users, Passwords)](/documentation/SERVICES.md)
- [Docker Quickstart](/documentation/DOCKER-QUICKSTART.md)
- [Run your project](/documentation/DOCKER-STARTUP.md)
- [Container detail info](/documentation/DOCKER-INFO.md)
- [Troubleshooting](/documentation/TROUBLESHOOTING.md)
- [Changelog](/CHANGELOG.md)

## Credits

This Docker layout is based on https://github.com/denderello/symfony-docker-example/

Thanks for your support, ideas and issues.
- [Ingo Pfennigstorf](https://github.com/ipf)
- [Florian Tatzel](https://github.com/PanadeEdu)
- [Josef Florian Glatz](https://github.com/jousch)
- [Ingo Müller](https://github.com/IngoMueller)
- [Benjamin Rau](https://twitter.com/benjamin_rau)
- [Philipp Kitzberger](https://github.com/Kitzberger)
- [Stephan Ferraro](https://github.com/ferraro)
- [Cedric Ziel](https://github.com/cedricziel)
- [Elmar Hinz](https://github.com/elmar-hinz)




Thanks to [cron IT GmbH](http://www.cron.eu/) for inspiration.

Did I forget anyone? Send me a tweet or create pull request!
