# laravel-starter-info


## Installation

Setup a new Laravel applicatie via Composer:

```shell
composer create-project laravel/laravel my-beautiful-blog
```

After installing the new Laravel app you need to changes some settings in the .env. Change the following lines:

```env
APP_NAME=MyBeautifulBlog

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=my_beautiful_blog
DB_USERNAME=root
DB_PASSWORD=
```

After changing the configurations (and after setting up your locale database!) run the following command to start your application:

```shell
// Migrating the database and seeder the default data.
php artisan migrate:fresh --seed

// Starting the application on 127.0.0.1:8000
php artisan serve
```

## Database

Laravel has multiple methods to build and fill you database and database data. Note that all the database table (and relations) are managed in the application.<br>
To run all your migrations you run `php artisan migrate:fresh` in your terminal. This will build that database structure without any data.<br>
<br>
To seed the database with some seeder data Laravel uses `seeders`. To run those seeders you can run `php artisan db:seed` in your terminal.



