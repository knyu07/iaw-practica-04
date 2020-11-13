# Práctica 4: Creación de una segunda máquina virtual para Apache

En esta práctica cogeremos los conceptos de la practica-03, con la diferencia de que añadiremos una nueva máquina front-end

### ESTRUCTURA DE LA RED

![](Imágenes/red.png);

> - Una capa de front-end, con dos servidores, que será pública
> - Una capa de back-end, que será privada

#############################################################

## INSTALACIÓN

### Para las dos máquinas Front-end:

Lo requisitos para esta máquina serían

- Abrir puerto SSH
- Abrir puerto HTTP
- Abrir puerto HTTPS
- Abrir puerto MySQL/Aurora

En ella creamos nuestra front-end.sh y haremos nuestros script escpedífico para esta máquina:

- Instalación de Apache
- Instalación de PHP
- Instalación de phpMyAdmin
- Instalación de GoAccess
- Instalación de Adminer 

:exclamation: Tendremos que configurar el archivo config.inc.conf 

:exclamation: Además de configurar el archivo config.php

Esto se hace para que entre las máquinas frond-end y back-end se vean entre ellas

### Back-end

Los requisitos para esta máquina serían

- Abrir puerto SSH
- Abrir puerto MySQL/Aurora

En ella crearemos nuestro back-end.sh y haremos nuestro script específico para esta máquina:

- Instalación de MySQL Server 

:exclamation: Para que ambas máquinas front-end se conecten al servidor MySQL configuramos el archivo /etc/mysql/mysql.conf.d/mysqld.cnf
sustituyendo localhost por 0.0.0.0

Creados nuestras máquinas y script para fornt-end y back-end ejecutamos. 

:smile_cat: