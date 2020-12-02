# Ambiente Integrado

### 1. Resumen
Repositorio que contiene la integración de todos los componentes listos para ejecutar en cada ambiente. Para los fines académicos este repositorio representa el ambiente de pruebas de Agroexportaciones para Colombia.


### 2. Construir los Servicios

#### 2.1 Tomcat Base
**Repositorio:** https://github.com/pedrazadumer/axpc-tomcat-base
```
$ cd axpc-tomcat-base
$ docker build -t axpc-tomcat-base .
```

#### 2.2 React Base
**Repositorio:** https://github.com/pedrazadumer/axpc-react-base
```
$ cd axpc-react-base
$ docker build -t axpc-react-base .
```

#### 2.3 Base de Datos
**Repositorio:** https://github.com/pedrazadumer/axpc-bd
```
$ cd axpc-bd
$ docker build -t axpc-bd .
```

#### 2.4 Microservicio de Clientes
**Repositorio:** https://github.com/pedrazadumer/axpc-clientes
```
$ cd axpc-clientes
$ docker build -t axpc-clientes .
```

#### 2.5 Aplicacion Web Responsive
**Repositorio:** https://github.com/pedrazadumer/axpc-ui
```
$ cd axpc-ui
$ docker build -t axpc-ui .
```

### 3. Desplegar el Ambiente

```
$ cd axpc-ambiente-integrado
$ docker-compose up --build
```

### 4. Detener los servicios y limpiar el ambiente

```
# Ctrl + C para detener
$ ^C
$ docker container prune -f
$ docker volume prune -f
```

### 5. Acceder a la Aplicación Web
**Página Principal:** http://localhost:3001/