# Práctica 6: Ejecutar servidor web Nginx con Docker

## Descripción
Esta práctica consiste en crear y ejecutar un servidor web Nginx de manera local utilizando Docker Compose. Se utiliza un archivo HTML como página principal y un volumen para conectar los archivos locales con el directorio web del contenedor.

## Objetivo de la práctica
Aprender a configurar y ejecutar un servidor web local mediante Docker Compose, utilizando volúmenes para servir contenido HTML desde el equipo anfitrión.

## Ejecución del proyecto
Para ejecutar el servidor, es necesario tener Docker Desktop instalado y en funcionamiento.

1. Clonar este repositorio.
2. Abrir una terminal en la carpeta del proyecto.
3. Ejecutar el siguiente comando:

```bash
docker compose up -d
```

4. Abrir el navegador y acceder a:

http://localhost:8080

Para comprobar el estado del contenedor, utilizar:

```bash
docker compose ps
```

Para detener el servidor, ejecutar:

```bash
docker compose down
```

## Resultado esperado
Al acceder a `http://localhost:8080`, se muestra una página HTML con el mensaje **¡Hola mundo!**, servido mediante Nginx.

## Autor
Víctor Núñez - Matrícula: 2012-0048
