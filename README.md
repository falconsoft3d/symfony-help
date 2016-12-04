# symfony-help
Ayuda de symfony

# Instalación de symfony standar
composer create-project symfony/framework-standard-edition demo 3.2.x-dev

# Comprobamos que todo este Ok
http://localhost/www/demo/web/config.php

# Configuraciones del PHP.ini
intl.error_level = 0

xdebug.max_nesting_level = 250

# Abrimos a modo de desarrollo
http://localhost/www/demo/web/app_dev.php


#Activamos el modo de producción
C:\xampp\htdocs\www\demo\web\app.php y colocamos la siguiente linea

$kernel = new AppKernel('prod', true);


# Generando un Bundle
nos paramos dentro del fichero y colocamos lo siguiente

php bin/console generate:bundle --namespace=MiBundle -format=yml

# Mapiando la base de datos
php bin/console doctrine:mapping:import BackendBundle yml

# Generar las entidades
php bin/console doctrine:generate:entities BackendBundle

