# Simple REST API in PHP

A simple REST API in core PHP with MySQL database.

## Getting Started

### Prerequisite: PHP, Composer, MySQL

Clone this repo.
```git
git clone https://github.com/raffyamoguis/php-rest-api
```

Install dependencies.
```sudo
composer install
```

Edit environment variable to connect your MySQL database.
```env
DB_HOST=localhost
DB_PORT=3306
DB_DATABASE={db_name}
DB_USERNAME={username}
DB_PASSWORD={password}
```

Run database seed.
```sudo
php dbseed.php
```

Start php server.
```sudo
php -S 127.0.0.1:8000 -t public
```

## Sample API Endpoints
This endpoints from the person data you can add your own by adding custom models, controllers.
```curl
// return all records
GET /person

// return a specific record
GET /person/{id}

// create a new record
POST /person

// update an existing record
PUT /person/{id}

// delete an existing record
DELETE /person/{id}
```

## License
Apache 2.0, see [LICENSE](LICENSE).
