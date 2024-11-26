# Comandos Docker - Sysgraf

<img src="https://www.docker.com/wp-content/uploads/2023/05/symbol_blue-docker-logo.png" height="100px" alt="docker-logo">

### Mostrar todos los contenedores

```
docker ps -a
```

### Levantar contenedores

```
docker-compose up -d
```

### Levantar contenedores descargando una versión especificada

```
docker-compose up -d --build
```

### Parar todos los Contenedores

```
docker-compose stop 
```

### Reiniciar todos los Contenedores

```
docker-compose restart 
```

#### Reinicia el contenedor especificado

```
docker-compose restart <prometheus>
```

### Logs Contenedores

```
docker logs –f <contenedor>
```

### Exportar Logs 

```
docker logs -f nginx >& ./logs/nginx.log
```
