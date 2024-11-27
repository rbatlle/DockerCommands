# Docker Commands

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRCAJH4R87uV3Rvncs3L3urjeNESAfJGTMTrA&s" height="120px" alt="docker-logo">


### Archivo docker-compose.yaml
##### Permite crear multiples contenedores con configuración personalizada

<img src="![image](https://github.com/user-attachments/assets/2ec4361d-b8e6-4eac-817a-f317c8bc86a3)">

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
