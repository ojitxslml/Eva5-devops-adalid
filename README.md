## Evaluación 5 - DevOps

Este repositorio documenta el desarrollo de la Evaluación 5: "Diseño de Arquitectura y Escalabilidad para una Plataforma de Gestión de Proyectos".

---

### Presentación
Puedes revisar la presentación de la evaluación en el siguiente enlace:
[Ver presentación en Prezi](https://prezi.com/view/DWnnip7NEHM9MvZqwZdQ/)

---

## 1. Requerimientos y Arquitectura Propuesta
**Requerimientos principales:**
- Autenticación y gestión de usuarios con distintos roles.
- CRUD de proyectos, asignación de presupuestos, fechas y archivos adjuntos.
- Alta escalabilidad, seguridad y resiliencia.

**Arquitectura seleccionada:**
- Microservicios: permite escalar componentes de forma independiente, favorece la resiliencia, el mantenimiento y el despliegue desacoplado.

## 2. Infraestructura y Estrategias de Escalabilidad
**Modelo recomendado:**
- Combinación de PaaS (App Service, Cloud Run), BaaS (Auth0, Firebase, S3) y FaaS (procesamiento de archivos, notificaciones).

**Estrategias:**
- Autoescalado horizontal por métricas.
- Balanceo de carga con Ingress Controller.
- Bases de datos y servicios desplegados en múltiples zonas.

## 3. Contenedorización y Orquestación
**Contenedores:** Docker (estándar y ampliamente adoptado).

**Orquestador:** Kubernetes (despliegue distribuido, escalado automático, gestión de fallos y configuración por entorno).

**Registro de contenedores:** AWS ECR o GitHub Container Registry.

## 4. Diagrama de Arquitectura
- Representa microservicios, API Gateway, bases de datos, almacenamiento y funciones.
- Incluye flujos de comunicación entre cliente, gateway y servicios internos.
- Define integración con servicios externos (auth, storage, CI/CD, observabilidad).

---

## ✅ Criterios de Evaluación
- Claridad en la identificación de requerimientos y selección de arquitectura.
- Diseño de infraestructura y estrategias de escalabilidad bien fundamentadas.
- Contenedorización y orquestación correctamente definidas.
- Diagramas de arquitectura bien estructurados y explicados.

---
**Autor:** Juan Pablo Urra  
**Curso:** DevOps Sence  
**Fecha:** Julio 2025
