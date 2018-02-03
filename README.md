# ansible
Este vagranfile con dicha receta, crea automaticamente dos máquinas:
  -Nodo 1: Donde tenemos un servidor DNS y un servidor MariaDB
  -Nodo2: Donde hay instalado un nginx con php-fpm y configurado un wordpress

Para el funcionamiento solo tenemos que levantar las máquinas con vagrant up y en el fichero /etc/resolv.conf de nuestra máquina tendremos que poner como ip 192.168.5.2

Todos las variables que se utilizan como ip, nombre sitio wordpress, nombre dns, etc. Es configurable desde el fichero vars

Nota: Si quieres tener una experiencia con ansible antes de lanzar las máquinas instala el paquete cowsay en tu máquina ;)
