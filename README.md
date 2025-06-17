# Plataforma de Cursos - Versión Monolítica

Este repositorio ha sido simplificado para utilizar una única aplicación Node.js que sirve una página HTML estática como interfaz principal. La estructura anterior basada en un monorepo con múltiples proyectos ha sido eliminada para facilitar el despliegue y mantenimiento.

## 📦 Estructura

- `public/index.html` – Página principal del frontend. Utiliza Tailwind CSS cargado desde CDN.
- `server.js` – Servidor Express encargado de servir los archivos estáticos.
- `package.json` – Dependencias y comandos de npm.

## 🚀 Uso

1. Instala las dependencias:
   ```bash
   npm install
   ```
2. Inicia el servidor:
   ```bash
   npm start
   ```
3. Abre `http://localhost:3000` en tu navegador para ver la página.

Este es el punto de partida para una infraestructura monolítica simple. Se puede ampliar con rutas adicionales, lógica de autenticación y conexión a bases de datos según las necesidades del proyecto.
