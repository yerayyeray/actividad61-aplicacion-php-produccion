# Aplicación web CRUD dockerizada lista para implantar en un servidor en producción

>IES Miguel Herrero (Torrelavega) - Curso 2025/2026
>Módulo: IAW - Implantación de Aplicaciones Web  
>Ciclo: CFGS Administración de Sistemas Informáticos en Red  

Este repositorio es una **guía** para la realización de la **actividad 6.1** de IAW en lo que se refiere al despliegue de la aplicación CRUD en <u>PRODUCCIÓN</u>. 

Contiene lo siguiente: 

* Directorio */sql*: Contiene un archivo con un script SQL para la inicialización de la BD de MariaDB
* Archivo *.env*: Configuración de variables de entorno (Contraseña Root, nombre BD, usuario BD y contraseña BD) utilizadas por el archivo docker-compose.yml para la inicializacion de MariaDB.
* Archivo *docker-compose.yml*: Modelo escenario de contenedores para el despliegue de la aplicación PHP. Contiene 2 servicios: 
1. *apache-php-crud*: Aplicación CRUD PHP implantada en una imagen con Ubuntu 24.04, servidor web Apache 2.0, php 8.0 (lumigv/lamp-crud-app:latest))
2. *mariadb*: Sistema gestor de base de datos en MariaDB



