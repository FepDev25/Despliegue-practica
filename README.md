# Desplegar práctica en máquina de un tercero

Este proyecto despliega una aplicación web fullstack contenedorizada, compuesta por:

- **Backend**: Spring Boot con conexión a PostgreSQL.
- **Frontend**: Angular servido con Nginx.
- **Base de datos**: PostgreSQL 15.

---

## Descarga de imágenes desde Docker Hub

Antes de ejecutar el entorno, asegúrate de tener disponibles las imágenes del frontend y backend. Puedes descargarlas manualmente desde Docker Hub:

- **Frontend (Angular + Nginx)**  
  [https://hub.docker.com/repository/docker/felipe2p05/angular-client](https://hub.docker.com/repository/docker/felipe2p05/angular-client)

- **Backend (Spring Boot)**  
  [https://hub.docker.com/repository/docker/felipe2p05/springboot-app](https://hub.docker.com/repository/docker/felipe2p05/springboot-app)

O usando los siguientes comandos:

```bash
docker pull felipe2p05/angular-client
docker pull felipe2p05/springboot-app
```

## Cómo ejecutar

1. Clona este repositorio o descomprimir el `.zip`.

2. Tener Docker y Docker Compose instalados.

3. En la raíz del proyecto, ejecutar:

```bash
docker compose up --build
```

o alternativa moderna:

```bash
docker-compose up --build
```

4. Abre en el navegador:

* Cliente Angular: [http://localhost:4200](http://localhost:4200)
* API Backend: [http://localhost:8080](http://localhost:8080)
