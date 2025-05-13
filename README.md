# Desplegar práctica en máquina de un tercero

Este proyecto despliega una aplicación web fullstack contenedorizada, compuesta por:

- **Backend**: Spring Boot con conexión a PostgreSQL.
- **Frontend**: Angular servido con Nginx.
- **Base de datos**: PostgreSQL 15.

---

## Clonar o descargar este repositorio

Antes de iniciar, clonar este repositorio o descarga el `.zip` desde GitHub:

```bash
git clone https://github.com/FepDev25/Despliegue-practica.git
cd Despliegue-practica
```
---

## Descargar las imágenes desde Docker Hub

Se debe tener disponibles las imágenes del frontend y backend. Se pueden descargar manualmente desde Docker Hub:

* **Frontend (Angular + Nginx)**
  [https://hub.docker.com/repository/docker/felipe2p05/angular-client](https://hub.docker.com/repository/docker/felipe2p05/angular-client)

* **Backend (Spring Boot)**
  [https://hub.docker.com/repository/docker/felipe2p05/springboot-app](https://hub.docker.com/repository/docker/felipe2p05/springboot-app)

O usando los siguientes comandos:

```bash
docker pull felipe2p05/angular-client
docker pull felipe2p05/springboot-app
```

---

##  Cómo ejecutar

1. Se debe tener Docker y Docker Compose instalados.

2. En la raíz del proyecto (donde está `docker-compose.yml`), ejecutar:

```bash
docker compose up
```

> O si usas la versión clásica:

```bash
docker-compose up
```

3. Accede a los servicios desde tu navegador:

* **Cliente Angular**: [http://localhost:4200](http://localhost:4200)
* **API Backend**: [http://localhost:8080](http://localhost:8080)

