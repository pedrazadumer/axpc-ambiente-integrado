# \[Fines Académicos\] Ambiente Integrado

### 1. Resumen
Repositorio que contiene la integración de todos los componentes listos para ejecutar en cada ambiente. Para los fines académicos este repositorio representa el ambiente de pruebas de Agroexportaciones para Colombia.

### 2. Desplegar el Ambiente

```
$ cd axpc-ambiente-integrado
$ docker-compose up --build
```

### 3. Detener los servicios y limpiar el ambiente

```
# Ctrl + C para detener
$ ^C
$ docker container prune -f
$ docker volume prune -f
```

### 4. Acceder a la Aplicación Web
**Página Inicial:** http://localhost:3001/