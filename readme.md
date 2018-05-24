# Setup Php 7.2 - Apache - Composer - PostgreSQL - Adminer

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

Add Package with Composer
```
docker run -it --rm -u "$(id -u):$(id -g)" -v "$PWD"/app:/app -w /app composer require prettus/l5-repository
```