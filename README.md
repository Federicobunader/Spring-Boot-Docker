# Spring-Boot-Docker

## Descripción del Proyecto

Este proyecto es una aplicación simple de Spring Boot que se ejecuta en un contenedor Docker. La aplicación es un servicio web RESTful que responde con un "Hello, World!" cuando se accede a la ruta raíz ("/").

El código principal de la aplicación se encuentra en el archivo `HelloWorldController.java`, que define un controlador REST con un solo método que maneja las solicitudes GET a la ruta raíz.

## Docker

Docker es una plataforma de código abierto que permite a los desarrolladores y administradores de sistemas construir, empaquetar y distribuir aplicaciones como contenedores ligeros y portátiles. Un contenedor Docker es una unidad estándar de software que empaqueta el código y todas sus dependencias para que la aplicación se ejecute de manera rápida y confiable de un entorno informático a otro.

El "Docker daemon", también conocido como dockerd, es un proceso persistente que se ejecuta en el host del sistema operativo. Este proceso gestiona las imágenes de Docker, los contenedores, las redes y los volúmenes de almacenamiento. El daemon de Docker también se encarga de construir y ejecutar contenedores Docker.

## Docker y Spring Boot

Spring Boot es un marco de trabajo que simplifica la configuración y el despliegue de aplicaciones Spring. Cuando se combina con Docker, Spring Boot permite a los desarrolladores empaquetar sus aplicaciones junto con sus dependencias en un contenedor Docker, lo que facilita el despliegue y la escalabilidad de la aplicación.

En este proyecto, utilizamos Docker para contenerizar nuestra aplicación Spring Boot. Esto se logra mediante un archivo `Dockerfile` que especifica cómo construir una imagen Docker para nuestra aplicación, y un archivo `docker-compose.yaml` que define cómo se debe ejecutar nuestra aplicación en un contenedor Docker.

## Cómo Ejecutar el Proyecto

Para ejecutar este proyecto, necesitarás tener Docker y Docker Compose instalados en tu máquina. Una vez instalados, puedes seguir estos pasos:

1. Abre tu terminal.
2. Navega hasta el directorio del proyecto donde se encuentra el archivo `docker-compose.yaml` utilizando el comando `cd`. Por ejemplo:

```bash
cd /ruta/al/directorio/del/proyecto
```

Para construir la imagen Docker de la aplicación, ejecuta el siguiente comando:

```bash
docker-compose up
