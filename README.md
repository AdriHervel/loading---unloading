# Proyecto de Microservicio con FastAPI

## Descripción

Este proyecto implementa un microservicio en Python para gestionar información de clientes, pólizas y pagos en una plataforma de seguros. Utiliza el framework **FastAPI** para construir APIs RESTful con énfasis en seguridad, escalabilidad y buenas prácticas de desarrollo.

## Características

- **Gestión de Clientes:** CRUD de clientes para el sistema de seguros.
- **Gestión de Pólizas:** CRUD de pólizas de seguro.
- **Gestión de Pagos:** CRUD para registrar y consultar pagos asociados a clientes.
- **Seguridad de API:** Implementación de JWT para autenticación y autorización.
- **Documentación de API**: Swagger/OpenAPI para documentación automática.
- **Escalabilidad:** Diseño orientado a alta escalabilidad y orquestación de tareas con Airflow.
- **CI/CD:** Implementación de pipelines de CI/CD en Azure DevOps.

## Tecnologías Utilizadas

- **Lenguaje:** Python 3.x
- **Framework de API:** FastAPI
- **Base de Datos:** PostgreSQL y MongoDB
- **ORM:** SQLAlchemy
- **Autenticación:** JWT y OAuth2
- **Orquestación:** Airflow
- **Pruebas:** PyTest y Unittest
- **CI/CD:** Azure DevOps
- **Containerización:** Docker y Docker Compose
- **Entorno en la Nube:** Azure

## Estructura del Proyecto

La estructura del proyecto está organizada de la siguiente manera:

```plaintext
loading-&-unloading/
├── app/
│   ├── api/                # Endpoints de la API
│   ├── core/               # Seguridad, autenticación y utilidades
│   ├── crud/               # Operaciones CRUD de la base de datos
│   ├── db/                 # Configuración de la base de datos
│   ├── models/             # Modelos de la base de datos
│   ├── schemas/            # Esquemas de datos (Pydantic)
│   ├── main.py             # Punto de entrada de la aplicación
│   └── config.py           # Configuración de la aplicación
├── tests/                  # Pruebas unitarias e integrales
├── alembic/                # Migraciones de la base de datos
├── scripts/                # Scripts para inicialización y otras tareas
├── Dockerfile              # Dockerfile para contenedorización
├── docker-compose.yml      # Docker Compose para orquestación de servicios
└── README.md               # Documentación del proyecto
