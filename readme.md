# DD8
## Introduction
DD8 is a Dockerized Drupal 8 image that uses Apache, MariaDB, and PHP. It uses
a `docker-compose.yml` file to spin up a local environment on Linux, Mac OS X and Windows.
## Stack
| Container | Version | Image |
| --------- | ------- | ----- |
| mariadb   | 10.4    | mariadb:10.4 |
| phpmyadmin | 4.7    | phpmyadmin/phpmyadmin:4.7 |
| httpd | 2.4 | httpd:2.4-alpine |
| php-fpm | 7.1 | php:7.1-fpm |

Currently, we will only support version that Drupal is fully tested.
## How to use
* locate the `docker-compose.yml` and open your terminal in the same file. Now type `docker-compose up -d`
* in the same directory type `composer create-project drupal-composer/drupal-project:8.x-dev drupal --stability dev --no-interaction`
* Open your browser and visit `localhost:8080`
* Follow the installation guide.
## URLs
* Drupal site: `localhost:8080`
* phpMyAdmin: `localhost:8083`
## Further reading
https://github.com/drupal-composer/drupal-project