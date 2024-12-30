# Sistema de Gestión de Candidatos en Proceso de Selección y Contratación

Este proyecto tiene como objetivo desarrollar un sistema backend que gestiona información de candidatos en procesos de selección y contratación. Está diseñado con arquitectura de microservicios, utilizando Go y MySQL, siguiendo prácticas modernas de desarrollo.

El sistema está dividido en varios servicios independientes para maximizar la escalabilidad, modularidad y eficiencia. Cada servicio está documentado y desplegado de manera individual.

## Estructura de los Servicios

### 1. **Auth Service**

Gestión de autenticación y autorización utilizando JWT. Protege las APIs del sistema asegurando que solo usuarios autorizados puedan acceder.

**Endpoints**:

- **Health Check**: `GET /health`
  - Verifica el estado del servicio.
- **Registro de Usuario**: `POST /register`
  - Registra un nuevo usuario.
- **Inicio de Sesión**: `POST /login`
  - Autentica un usuario y genera un token JWT.

[Repositorio del Auth Service](https://github.com/poolcamacho/auth-service)  
[Swagger](https://auth.codewisetech.biz/swagger/index.html#/)

---

### 2. **Candidates Service**

Servicio dedicado a la gestión de información de candidatos. Permite realizar operaciones CRUD sobre el modelo de candidatos.

**Endpoints**:

- **Health Check**: `GET /health`
  - Verifica el estado del servicio.
- **Listar Candidatos**: `GET /candidates`
  - Obtiene una lista de todos los candidatos.
- **Crear Candidato**: `POST /candidates`
  - Registra un nuevo candidato.

[Repositorio del Candidates Service](https://github.com/poolcamacho/candidates-service)  
[Swagger](https://candidates.codewisetech.biz/swagger/index.html#/)

---

### 3. **Job Service**

Módulo encargado de manejar las ofertas de empleo disponibles en el sistema.

**Endpoints**:

- **Health Check**: `GET /health`
  - Verifica el estado del servicio.
- **Listar Ofertas de Empleo**: `GET /jobs`
  - Obtiene una lista de todas las ofertas de empleo.
- **Crear Oferta de Empleo**: `POST /jobs`
  - Crea una nueva oferta de empleo.

[Repositorio del Job Service](https://github.com/poolcamacho/jobs-service)  
[Swagger](https://jobs.codewisetech.biz/swagger/index.html#/)

---

### 4. **Interviews Service**

Módulo encargado de gestionar las entrevistas realizadas a los candidatos para las ofertas de empleo.

**Endpoints**:

- **Health Check**: `GET /health`
  - Verifica el estado del servicio.
- **Listar Entrevistas**: `GET /interviews`
  - Obtiene una lista de todas las entrevistas.
- **Crear Entrevista**: `POST /interviews`
  - Crea una nueva entrevista.

[Repositorio del Interviews Service](https://github.com/poolcamacho/interviews-service)  
[Swagger](https://interviews.codewisetech.biz/swagger/index.html#/)

---

## Despliegue

Cada servicio está desplegado individualmente. Puedes acceder a las APIs de los servicios mediante los siguientes enlaces:

- **Auth Service**: [https://auth.codewisetech.biz](https://auth.codewisetech.biz)
- **Candidates Service**: [https://candidates.codewisetech.biz](https://candidates.codewisetech.biz)
- **Job Service**: [https://jobs.codewisetech.biz](https://jobs.codewisetech.biz)
- **Interviews Service**: [https://interviews.codewisetech.biz](https://interviews.codewisetech.biz)

---

## Documentación

Cada servicio incluye:

- Documentación de endpoints en Swagger.
- Colección de Postman con ejemplos exitosos y fallidos para pruebas.

### Ruta del Archivo de Postman

La colección de Postman está disponible en el directorio `collection` del proyecto:
