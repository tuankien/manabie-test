# manabie-test
Test Project - Manabie 

### Requirements:

- Git.
- Composer.
- PHP 7.4+ or 8.0+.
- MySQL/MariaDB.
- Redis (Optional).
- or Docker.

### With Composer:

You can create a new project running the following commands:

```bash
$ composer create-project tuankien/manabie-test [your-project-name]
$ cd [your-project-name]
$ composer restart-db
$ composer test
$ composer start
```

### With Git:

In your terminal execute this commands:

```bash
$ git clone https://github.com/tuankien/manabie-test.git && cd manabie-test
$ cp .env.example .env
$ composer install
$ composer restart-db
$ composer test
$ composer start
```

### With Docker:

You can use this project using **docker** and **docker-compose**.

**Minimal Docker Version:**

* Engine: 18.03+
* Compose: 1.21+

**Commands:**

```bash
# Start the API (this is my alias for: docker-compose up -d --build).
$ make up

# To create the database and import test data from scratch.
$ make db

# Checkout the API.
$ curl http://localhost:8081

# Stop and remove containers (it's like: docker-compose down).
$ make down
```
