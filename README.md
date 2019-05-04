# Demand-side system

This project was created for my Graduate studies of Development of applications for web and mobile devices.

Application created using [ZendSkeletonApplication](https://github.com/zendframework/ZendSkeletonApplication)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

* PHP 7

### Installing

Clone the project and enter into the project folder:

```sh
$ git clone https://github.com/carollaginestra/zend-system.git
$ cd zend-system
```

Install composer

```sh
$ composer install
$ composer update
```

### Start project

start the project: (you can use another port, like 8080)

```sh
$ php -S localhost:8000 -t public/
```

Access the site in your browser at:
```
http://localhost:8000
```

### Setting database

Create the file local.php to setting database
```sh
$ cp config/autoload/local.php.dist config/autoload/local.php
```
Open the file ```config/autoload/local.php ``` and inside "return" array, insert:

```
'db' => [
    'username' => 'root', #let this match your MySQL username
    'password' => '', #let this match your MySQL database password
]
```

## Create modules

always after you have created all the files in a new module, run the command

```sh
$ composer dump-autoload
```

## Built With

* [Bootstrap v3.3.7](https://getbootstrap.com/docs/3.3/) - The web Framework front-end used
* [Zend 3](https://framework.zend.com/) - The web Framework PHP used