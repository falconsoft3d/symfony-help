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

# Creamos el hola mundo
 /**
     * @Route("/hello-world", name="homepage")
     */
   public function helloWorldAction(){
        echo "<h1>Hola mundo</h1>";
        die();
   }
   
http://localhost/www/demo/web/app_dev.php/hello-world
