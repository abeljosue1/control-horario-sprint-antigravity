# Control Horario MVP - Sprint 0 (TAREA 1) 

Este proyecto es un MVP (Producto Mínimo Viable) para el registro y control de jornadas laborales, desarrollado como parte del Sprint 0 del bootcamp de Antigravity.

## 🚀 Funcionalidades

- **Autenticación**: Registro e inicio de sesión seguro con Supabase Auth.
- **Control de Jornada**:
- **Control de Jornada**:
  - **INICIAR TURNO**: Iniciar jornada.
  - **INICIAR BREAK / REANUDAR TURNO**: Gestión de pausas (breaks). **Nota**: El break es obligatorio de 45 minutos.
  - **TERMINAR TURNO**: Finalizar jornada.
- **Persistencia**: Todos los datos se guardan en una base de datos PostgreSQL (Supabase).
- **Historial**: Visualización de jornadas anteriores con horas totales calculadas.

## 🛠️ Arquitectura y Tecnologías

El proyecto sigue una arquitectura **Frontend Vanilla** conectada a servicios Backend:

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla).
- **Backend/Auth**: Supabase (PostgreSQL + GoTrue).
- **Infraestructura**: Despliegue estático (Local/Vercel).

### Estructura de Archivos

- `index.html`: Estructura principal de la SPA (Single Page Application).
- `style.css`: Estilos y diseño visual.
- `app.js`: Lógica de negocio, manejo del DOM y llamadas a Supabase.
- `config.js`: Credenciales de conexión a Supabase.
- `schema.sql`: Definición de la base de datos y políticas de seguridad (RLS).

## 📦 Instalación y Uso

1.  **Clonar el repositorio**:
    ```bash
    git clone <https://github.com/abeljosue1/control-horario-sprint-antigravity>
    ```
2.  **Configurar Base de Datos**:
    - Crea un proyecto en [Supabase](https://supabase.com).
    - Corre el script `schema.sql` en el SQL Editor de tu proyecto para crear las tablas y políticas.
3.  **Configurar Credenciales**:
    - Renombra `config.example.js` a `config.js` (si aplica) o edita `config.js`.
    - Pega tu `https://hepkljurqjkypjhdmuhq.supabase.co` y `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImhlcGtsanVycWpreXBqaGRtdWhxIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NzA1OTY0NzEsImV4cCI6MjA4NjE3MjQ3MX0.fgkJVlIFpvqLlw8mSDMTyVVtvlL6IOIyqrLY3W2yM0Q`.
4.  **Ejecutar**:
    - Abre el archivo `index.html` en tu navegador o usa un servidor local (ej. Live Server).
    - Regístrate con un email y contraseña.

## 🎓 Aprendizajes del Equipo

Durante este Sprint, el equipo aprendió a:

1.  **Implementar Scrum Real**: Realizamos Dailies, Planning y Retrospective, gestionando tareas en Trello.
2.  **Usar Agentes de IA**: Utilizamos Antigravity para acelerar el desarrollo del boilerpate y depuración.
3.  **Integrar Backend sin Servidor**: Conectamos un frontend estático directamente a Supabase sin necesidad de un backend intermedio (Node/Express).
4.  **Manejar Estados**: Aprendimos a gestionar el estado de la aplicación (timer, sesión) y persistirlo.

## 🔗 Recursos

- **Trello**: [https://trello.com/b/X9jlMO2p/practicas]
