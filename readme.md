# Setup Php 7.2 - Apache - Composer - PostgreSQL - Adminer

Containers
- my-app | php7.2-apache
- my-database | postgres
- my-adminer | adminer
- composer

Creating Project Laravel
```
docker run -it --rm -u "$(id -u):$(id -g)" -v "$PWD":/app -w /app composer create-project laravel/laravel app 
```

Creating Project Symfony 3.4
```
docker run -it --rm -u "$(id -u):$(id -g)" -v "$PWD":/app -w /app composer create-project symfony/framework-standar-edition app 
```

Creating Project Symfony 4.2
```
docker run -it --rm -u "$(id -u):$(id -g)" -v "$PWD":/app -w /app composer create-project symfony/website-skeleton app 
```

Running commands with Composer
```
docker run -it --rm -u "$(id -u):$(id -g)" -v "$PWD":/app -w /app composer require prettus/l5-repository
```

Running commands in project
```
docker exec -it -u "$(id -u):$(id -g)" -w /app my-app php artisan
```
