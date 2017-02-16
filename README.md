# Prueba_tecnica

Para instalar el proyecto, primero y antes de nada con el terminal ejecutamos "vagrant up" para arrancar la máquina vitual
con la que crearemos el proyecto. Hecho esto, accedemos a la carpeta oculta .homestead y editamos el archivo Homestead.yaml,
en la línea "folders" cambiamos la ubicación de "map" al directorio donde vayamos a contener todos nuestros proyectos,
la ubicación de "to" deber ser "/home/vagrant/Code" y en la línea "sites" podemos modificar "map"
poniendo por ejemplo: www.test.com, en "to" cambiamos la ubicación a donde estará la carpeta publics del proyecto,
por ejemplo: /home/vagrant/Code/test/public. (Esta parte la he hecho antes de crear el proyecto, para no tener que volver a modificar este archivo después).
Ahora abrimos el terminal desde la carpeta Homestead y ejecutamos el comando "vagrant ssh", desde ahí accedemos
a la carpeta Code donde crearemos el proyecto. El proyecto se puede crear mediante dos comandos,
el comando "laravel new nombre_del_proyecto" o
con el comando "composer create-project --prefer-dist laravel/laravel nombre_del_proyecto "version_de_laravel"".
Hecho todo esto ya solo queda ejecutar el comando "vagrant provision" con el terminal desde el directorio Homestead. (El comando vagrant funciona solo si se hace desde el directorio Homestead).
