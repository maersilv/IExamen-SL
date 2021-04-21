# Instalar heroku cli antes de todo

    sudo apt-get install heroku 0ad(es un cero)

## Antes de cualquier cosa crear un git

Se debe tener un repositorio para poder cargar el proyecto, por eso crearemos un repositorio de manera local

    composer create-project laravel/laravel examen
    cd examen
    git init
    
    
Luego procedemos a loguearnos

## como loguearse

    heroku login
Esto si se quiere loguear por medio de la pagina web

Si se quiere loguear desde consola

    heroki login -i

## Añadir Procfile

Se debe añadir este archivo al git para que funcione, para esto ingresamos la siguiente línea de comando:

    
    echo "web: vendor/bin/heroku-php-apache2 public/" > Procfile

Luego se sube al git
    git add -A
    git commit -m "message"

## Creación del app

Luego creamos el app de la siguiente manera:

    heroku create


## Abrir Heroku

Si deseamos abrir el app de Heroku debemos correr el siguiente comando:

    heroku open

Luego hacemos un push

    git push heroku master

## Instalar la parte de autentificación Laravel

    composer require laravel/ui
    php artisan ui bootstrap
    php artisan ui bootstrap --auth
    npm install && npm run dev


## Cambios

Cada vez que realizamos un cambio debemos hacer el procedo de añadir al repo

    git add -A
    git commit -m "message"
    git push heroku master



## Entorno de producción
Esto lo hacemos en web.php

if (env('APP_ENV') === 'production') {
    \URL::forceScheme('https');
}

Y luego en la consola de comandos ejecutar lo sigueinte:

    heroku config:set APP_ENV=production

Y subir los cambios
    git add -A
    git commit -m "message"
    git push heroku master
