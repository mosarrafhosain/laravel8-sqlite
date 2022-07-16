# Laravel 8 with SQLite

# Installation

Clone this repo
```
$ git clone https://github.com/mosarrafhosain/laravel8-sqlite.git
```

Install composer packages
```
$ cd laravel8-sqlite
$ composer install
```

Make a copy of .env.example
```
$ copy .env.example .env
```

Generate application key
```
$ php artisan key:generate
```

# Setup ENV for our SQLite Database

By default, you will see these lines inside the .env file.
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

Now, let's change it with the following lines below.
```
DB_CONNECTION=sqlite
DB_HOST=127.0.0.1
DB_PORT=3306
```

Run migration command
```
$ php artisan migrate
```

Start development server
```
$ php artisan serve
```
