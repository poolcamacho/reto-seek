
# Sistema de Gestión de Candidatos en Proceso de Selección y Contratación

Este proyecto tiene como objetivo desarrollar un sistema backend que gestiona información de candidatos en procesos de selección y contratación. Está diseñado con arquitectura de microservicios, utilizando Go y MySQL, siguiendo prácticas modernas de desarrollo.

El sistema está dividido en varios servicios independientes para maximizar la escalabilidad, modularidad y eficiencia. Cada servicio está documentado y desplegado de manera individual.

## Estructura de los Servicios

### 1. **Auth Service**
Gestión de autenticación y autorización utilizando JWT. Protege las APIs del sistema asegurando que solo usuarios autorizados puedan acceder.

[Repositorio del Auth Service](https://github.com/poolcamacho/auth-service)

[Swagger](https://jananpbnuv.us-east-1.awsapprunner.com/swagger/index.html#/)

### 2. **Candidates Service**
Servicio dedicado a la gestión de información de candidatos. Permite realizar operaciones CRUD sobre el modelo de candidatos.

[Repositorio del Candidates Service](https://github.com/poolcamacho/candidates-service)

[Swagger](https://tgd3xm9dpx.us-east-1.awsapprunner.com/swagger/index.html#/)

### 3. **Companies Service**
Servicio dedicado a la gestión de información de compañias. Permite realizar operaciones CRUD sobre el modelo de compañias.

[Repositorio del Candidates Service](https://github.com/poolcamacho/companies-service)

[Swagger](https://epk56gyvhu.us-east-1.awsapprunner.com/swagger/index.html#/)

### 4. **Job Service**
Módulo encargado de manejar las ofertas de empleo disponibles en el sistema.

[Repositorio del Job Service](https://github.com/poolcamacho/job-service)

[Swagger](https://eapp4maamu.us-east-1.awsapprunner.com/swagger/index.html#/)

### 5. **Application Service**
Gestiona las postulaciones de los candidatos a las ofertas de empleo.

[Repositorio del Application Service](https://github.com/poolcamacho/application-service)

[Swagger](https://ba3iswcs3w.us-east-1.awsapprunner.com/swagger/index.html#/)

## Despliegue
Cada servicio está desplegado individualmente utilizando AWS App Runner. Puedes acceder a las APIs de los servicios mediante los siguientes enlaces:

- Auth Service: [https://jananpbnuv.us-east-1.awsapprunner.com](https://jananpbnuv.us-east-1.awsapprunner.com)
- Candidates Service: [https://tgd3xm9dpx.us-east-1.awsapprunner.com](https://tgd3xm9dpx.us-east-1.awsapprunner.com)
- Job Service: [https://eapp4maamu.us-east-1.awsapprunner.com](https://eapp4maamu.us-east-1.awsapprunner.com)
- Application Service: [https://ba3iswcs3w.us-east-1.awsapprunner.com](https://ba3iswcs3w.us-east-1.awsapprunner.com)

## Documentación
Cada servicio incluye:
- Documentación de endpoints en Swagger.
- Colección de Postman con ejemplos exitosos y fallidos para pruebas.

---
