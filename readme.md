# Docker Commands

![Command](https://img.shields.io/badge/Tools-Docker-blue) ![Command](https://img.shields.io/badge/Project-Sysgraf-red) 

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRCAJH4R87uV3Rvncs3L3urjeNESAfJGTMTrA&s" height="120px" alt="docker-logo">

## ARCHIVOS
### docker-compose.yaml
<p>Permite crear multiples contenedores con configuración personalizada</p>

<img src="images/docker-compose.png">

### Dockerfile
<img src="images/docker-build.png">

```
docker build –t  php-ldap
```

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
