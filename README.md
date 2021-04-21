<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

Primero creamos nuestro proyecto usando laravel con el siguiente comando:
Para poder crear el proyecto de la primera forma indicada debemos instalar “Laravel Instaler”. Esto lo podemos hacer mediante el siguiente comando en la consola de Composer:

     composer global require "laravel/installer"
Una vez terminada la instalación, procederemos a crear un nuevo proyecto laravel haciendo uso de la siguiente instrucción:

        laravel new nombre_del_proyecto
en nuestro caso:

    laravel new examen

Una vez tengamos el proyecto creado, debemos iniciar el servidor donde ejecutaremos nuestro código. Para lograr esto desde la consola iremos a la nueva carpeta creada y escribiremos lo siguiente:

        php artisan serve
        
Ahora, iremos a un navegador web y escribiremos la URL que apareció en la consola. Dependerá de la configuración de su servidor web pero usualmente será la siguiente:

    http://localhost:8000
#JETSTREAM
Con la ayuda de jetstream procedemos a crear nuestro login y register.
#Instalación de Jetstream
puede usar Composer para instalar Jetstream en su nuevo proyecto de Laravel:

        composer require laravel/jetstream
#Instalar Jetstream con Livewire
       
        php artisan jetstream:install livewire

        php artisan jetstream:install livewire --teams
#Finalización de la instalación
Después de instalar Jetstream, debe instalar y crear sus dependencias de NPM y migrar su base de datos:

        npm install
        npm run dev
        php artisan migrate
Link del examen en heroku:
                


