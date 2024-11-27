# Docker Commands

![Command](https://img.shields.io/badge/Tools-Docker-blue)  ![Command](https://img.shields.io/badge/docker_compose-blue) 

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRCAJH4R87uV3Rvncs3L3urjeNESAfJGTMTrA&s" height="120px" alt="docker-logo">

### Archivo docker-compose.yaml
##### Permite crear multiples contenedores con configuración personalizada

<img src="docker-compose.png">

### Archivo Dockerfile

```
docker build –t  php-ldap
```

<img src="docker-build.png">

### Levantar contenedores

```
docker-compose up -d
```

### Levantar contenedores descargando una nueva versión de estos

```
docker-compose up -d --build
```

### Parar Contenedores

```
docker-compose stop 
```

```
docker-compose stop <nginx>
```

### Reiniciar contenedores

```
docker-compose restart 
```

```
docker-compose restart <nginx>
```

### Mostrar todos los contenedores (Cualquier Estado)

```
docker ps -a
```
<img src="docker-ps.png">

### Logs Contenedores

```
docker logs –f nginx
```

### Exportar Logs 

```
docker logs -f nginx >& ./logs/nginx.log
```

## Imagenes Aplicaciones Contenedores

### Visualiza todas las imagenes descargadas localmente

```
docker images
```

### Eliminar imagen
```
docker image rm 
```
