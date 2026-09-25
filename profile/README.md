<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/UT-LIME-UdeA/.github/main/assets/Logos-PDF-white.png">
  <img alt="LIME · Universidad de Antioquia · Hospital Alma Máter" src="https://raw.githubusercontent.com/UT-LIME-UdeA/.github/main/assets/Logos-PDF.png" width="900">
</picture>

# Laboratorios Integrados de Medicina Especializada

**Ingeniería de software para la salud, desde la Universidad de Antioquia y el Hospital Alma Máter.**

[![Sitio web](https://img.shields.io/badge/laboratorios--lime.com-1B5E3A?style=for-the-badge&logo=googlechrome&logoColor=white)](https://laboratorios-lime.com)
[![Contacto](https://img.shields.io/badge/lime%40udea.edu.co-0A66C2?style=for-the-badge&logo=gmail&logoColor=white)](mailto:lime@udea.edu.co)
[![Universidad de Antioquia](https://img.shields.io/badge/Universidad_de_Antioquia-006B3F?style=for-the-badge)](https://www.udea.edu.co)

</div>

---

## Quiénes somos

LIME es la unidad de laboratorios especializados de la Universidad de Antioquia en alianza con el Hospital Alma Máter de Antioquia. Esta organización reúne el software que construye el equipo de desarrollo del laboratorio: sistemas de información clínica, plataformas de telesalud, tableros de programas de salud pública y herramientas de gestión interna.

Los repositorios son privados. Este perfil describe el portafolio y la forma de trabajar del equipo.

## Portafolio

### Sistemas clínicos y de laboratorio

| Proyecto | Qué resuelve | Stack | Estado |
| --- | --- | --- | --- |
| [PATHSYS](https://github.com/UT-LIME-UdeA/PATHSYS) | Gestión de casos de patología: pacientes, diagnósticos CIE-10/CIE-O, facturación, reportes y API para entidades aliadas. | Next.js · FastAPI · MongoDB | Producción |
| [DERMOPAT](https://github.com/UT-LIME-UdeA/DERMOPAT) | Gestión de casos de dermatopatología. Misma arquitectura que PATHSYS con flujo propio. | Next.js · FastAPI · MongoDB | Producción |
| [TELESALUD](https://github.com/UT-LIME-UdeA/TELESALUD) | Plataforma de telesalud: solicitud, triage, teleconsulta por video, historia clínica y seguimiento. | Next.js · FastAPI · MongoDB · Agora | Producción |
| [NETMEDICA](https://github.com/UT-LIME-UdeA/NETMEDICA) | Historia clínica electrónica para consulta de dermatología: paciente, cita y atención. | Next.js · FastAPI · MongoDB | En desarrollo |
| [RMFLOW](https://github.com/UT-LIME-UdeA/RMFLOW) | Gestión y control de resonancias magnéticas: casos, radiólogos, convenios y oportunidad. | Next.js · FastAPI · SQLAlchemy | En desarrollo |

### Plataformas de datos y tableros

| Proyecto | Qué resuelve | Stack | Estado |
| --- | --- | --- | --- |
| [SYMPHONY](https://github.com/UT-LIME-UdeA/SYMPHONY) | Plataforma de ingesta y consolidación de datos de los programas de salud pública. Alimenta los tableros. | Next.js · FastAPI · Celery · MySQL | Producción |
| [CONTIGOANTIOQUIA](https://github.com/UT-LIME-UdeA/CONTIGOANTIOQUIA) | Tablero del programa Contigo Antioquia: capacitaciones, habilitación, SIVIGILA, teleapoyo y reportes. | Next.js · FastAPI · MySQL | Producción |
| [PDET](https://github.com/UT-LIME-UdeA/PDET) | Tablero del programa PDET: entidades, municipios, cronograma y telesalud. | Next.js · FastAPI · MySQL | Mantenimiento |
| [ENTERPRISE](https://github.com/UT-LIME-UdeA/ENTERPRISE) | Tablero analítico del laboratorio clínico: órdenes, oportunidad, demografía y validadores. | Next.js · FastAPI · MariaDB | Producción |

### Gestión institucional

| Proyecto | Qué resuelve | Stack | Estado |
| --- | --- | --- | --- |
| [LIME](https://github.com/UT-LIME-UdeA/LIME) | Portal institucional y hub de acceso a las aplicaciones del laboratorio. | React · Vite · FastAPI | Producción |
| [BIOTECH](https://github.com/UT-LIME-UdeA/BIOTECH) | Inventario y mantenimiento de equipos biomédicos. | Next.js · FastAPI · MongoDB | En desarrollo |

## Cómo construimos

Todos los proyectos comparten la misma base tecnológica y la misma estructura, para que cualquier persona del equipo pueda moverse entre repositorios sin fricción.

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

- **Un repositorio por producto**, con `frontend/`, `backend/`, `deploy/` y `docs/` en la raíz.
- **Frontend** en TypeScript con Next.js o React, Tailwind CSS y organización por módulos de dominio.
- **Backend** en Python con FastAPI, validación con Pydantic y pruebas automatizadas con pytest.
- **Datos** en MongoDB Atlas para los sistemas clínicos y MySQL/MariaDB para los tableros.
- **Despliegue** en contenedores Docker sobre AWS, con Caddy como proxy inverso y HTTPS automático.
- **Convenciones**: commits convencionales, documentación técnica y manual de usuario por producto, y puertos de desarrollo local asignados por proyecto para levantar varios sistemas a la vez.

## Principios

1. **El código es la fuente de verdad.** La documentación describe lo que existe, no lo que se planea.
2. **Módulos por dominio.** Cada capacidad clínica o administrativa vive en su propio módulo, con su API, sus vistas y sus pruebas.
3. **Seguridad por defecto.** Autenticación con JWT, control de acceso por roles y permisos, y secretos fuera del repositorio.
4. **Integración explícita.** Los sistemas se comunican por API o por bases de datos compartidas declaradas, nunca por acoplamientos implícitos.
5. **Calidad continua.** Pruebas, revisión de código y despliegues reproducibles en cada producto.

---

<div align="center">

Universidad de Antioquia · Hospital Alma Máter de Antioquia · Medellín, Colombia

</div>
