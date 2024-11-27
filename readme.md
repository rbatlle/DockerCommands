# Docker Commands

![Command](https://img.shields.io/badge/Tools-Docker-blue)

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRCAJH4R87uV3Rvncs3L3urjeNESAfJGTMTrA&s" height="120px" alt="docker-logo">

## ARCHIVOS
### docker-compose.yaml 
<p>Es un archivo de configuración que define múltiples servicios de Docker en un solo entorno. Utilizando sintaxis YAML, permite describir contenedores, redes, volúmenes y variables de entorno necesarias para una aplicación. </p>

<img src="images/docker-compose.png">

### Dockerfile

<p>Es un archivo de texto que contiene una secuencia de instrucciones para crear una imagen personalizada de Docker. Define cómo se construye el entorno del contenedor, el software que incluye y cómo se configura. </p>
<img src="images/docker-build.png">
<p>En la captura podemos observar que a partir de la imagen base de php añadiremos el módulo de autenticación LDAP, de esta manera crearemos una imagen personalizada que ya incluirà este modulo.</p>

```
docker build –t  php-ldap
```

### .env 

<p>Archivo oculto que podemos usar para almacenar información sensible (Credenciales, Versiones de contenedores...) por defecto si hemos definido definimos variables de entorno en el archivo docker-compose.yml este leera el contenido del archivo .env </p>


### Docker swarm

## Levantar contenedores

```
docker-compose up -d
```

<p>Levantar contenedores descargando una nueva versión de estos</p>

```
docker-compose up -d --build
```

## Parar Contenedores

```
docker-compose stop 
```

```
docker-compose stop nginx
```

## Reiniciar contenedores

```
docker-compose restart 
```

```
docker-compose restart nginx
```

## Mostrar todos los contenedores (Cualquier Estado)
<img src="images/docker-ps.png">

```
docker ps -a
```

## Acceder internamente a un Contenedor

```
docker exec -it <CONTENEDOR> /bin/bash
```

## Logs

```
docker logs –f nginx
```

### Exportar Logs 

```
docker logs -f nginx >& ./logs/nginx.log
```

## Imagenes Contenedores

#### Muestra todas las imagenes descargadas localmente
<img src="images/docker-images.png" alt="docker images">

```
docker images
```

#### Eliminar imagen

<img src="images/docker-images-rm.png" alt="docker image rm">

```
docker image rm -f <ID_IMAGEN>
```
