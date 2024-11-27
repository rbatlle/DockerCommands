# Docker Commands

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRCAJH4R87uV3Rvncs3L3urjeNESAfJGTMTrA&s" height="120px" alt="docker-logo">


### Archivo docker-compose.yaml
##### Permite crear multiples contenedores con configuración personalizada

<img src="docker-compose.png">

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

### Reiniciar contenedores

```
docker-compose restart 
```

### Mostrar todos los contenedores (Cualquier Estado)

```
docker ps -a
```

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
