# Plataforma de Cursos - Monorepo

Este proyecto consiste en una plataforma de cursos online con arquitectura fullstack. Está orientado a la simplicidad, reutilización y despliegue por instancia única. En esta primera versión, el enfoque es permitir un curso único por instalación, con funcionalidades básicas pero sólidas.

---

## 🧱 Estructura del Proyecto

- **Monorepo**: contiene tanto el frontend como el backend en un único repositorio.
- **Frontend**: HTML, CSS y JavaScript puro, sin frameworks, para evitar dependencias innecesarias.
- **Backend**: Spring Boot en Java, conectado a una base de datos MySQL.
- **Base de datos**: orientada a un curso único por proyecto, diseñada y administrada con MySQL Workbench.

---

## 🚀 Stack Tecnológico

| Capa         | Tecnología           |
|--------------|----------------------|
| Frontend     | HTML, CSS, JS        |
| Backend      | Java + Spring Boot   |
| Base de Datos| MySQL                |
| Autenticación| Google OAuth 2.0     |
| Infraestructura (dev) | Local + Live Server |

---

## 🔐 Autenticación

- Se utiliza **Login con Google** como único método de autenticación.
- Configuración mediante Google Developer Console (OAuth 2.0).
- El sistema distingue entre:
  - **Admin** (gestión general)
  - **Estudiante** (progreso y consumo de contenido)

---

## 🧠 Estructura de Base de Datos

**Diseñada para una sola instancia de curso.**

Entidades principales:
- `usuarios`: id, nombre, email, rol
- `cursos`: id, nombre, descripción
- `modulos`: id, curso_id, título
- `videos`, `pdfs`, `examenes`: asociados a módulos
- `inscripciones`: alumno_id, curso_id
- `progreso_usuario`: usuario_id, modulo_id, estado

---

## 🎯 Alcance de la Fase Actual

- Curso único por instancia del proyecto
- Progreso del usuario por módulo
- Reproductor de videos, visualización de PDFs, y sistema de evaluaciones
- Login con Google (en implementación)
- Maquetado completo de:
  - Página de inicio
  - Página del curso
  - Página de login (mock)
  - Página del reproductor

---

## 🧪 Estado Actual del Desarrollo

- [x] Backend funcional con conexión MySQL
- [x] Frontend maquetado con diseño minimalista moderno
- [x] Estructura base del monorepo completa
- [ ] Login con Google en integración
- [ ] Conexión frontend-backend pendiente
- [ ] Implementación de lógica de carga de contenido

---

## 🛠️ Modelo de Negocio

- Se vende la plataforma como **plantilla reutilizable** por proyecto
- Cada instancia es completamente independiente
- Pensada para ser fácilmente desplegable en múltiples clientes

---

## ✨ Próximos pasos

- Finalizar integración OAuth
- Conectar backend con frontend
- Implementar dashboard de usuario y lógica de consumo de contenidos
- Documentación técnica detallada para facilitar reusabilidad

---

