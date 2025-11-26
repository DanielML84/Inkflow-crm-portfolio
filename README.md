# 🖋️ InkFlow CRM - Gestión Integral para Estudios de Tatuajes

![InkFlow CRM Dashboard](ruta_a_tu_imagen_principal.png)

## 📖 Descripción

**InkFlow CRM** es una Plataforma de Gestión de Estudio (Studio Management Platform) diseñada para modernizar la operativa de los estudios de tatuajes. 

Desarrollada como una SPA (Single Page Application), soluciona la desorganización habitual mediante un sistema centralizado para gestionar clientes, agendas visuales y el flujo de trabajo de cada proyecto.

## 🚀 Funcionalidades Principales

### 🔐 Seguridad y Acceso
* **Autenticación Robusta:** Sistema de Login seguro basado en tokens (Laravel Sanctum).
* **Protección de Rutas:** Guardias de navegación en Frontend y Middleware en Backend.

### 📅 Gestión y Organización
* **Agenda Visual Interactiva:** Calendario mensual integrado (FullCalendar) con filtrado por artista.
* **Gestión de Clientes y Artistas:** CRUD completo con búsqueda en tiempo real y paginación.

### 🎨 Flujo de Trabajo (Workflows)
* **Sistema de Hitos:** Seguimiento del ciclo de vida de cada cita (Diseño, Señal, Sesión, Pago) con estados visuales.
* **Automatización:** Generación automática de hitos estándar al crear una cita.

### 💻 Experiencia de Usuario (UX)
* **Interfaz Moderna:** Diseño oscuro (Dark Mode) construido con Tailwind CSS.
* **Feedback Inmediato:** Notificaciones Toast y alertas modales (SweetAlert2) para todas las acciones.
* **SPA:** Navegación fluida sin recargas de página gracias a Vue Router.

---

## 🛠️ Stack Tecnológico

* **Backend:** PHP 8.2, Laravel 11, MySQL, Eloquent ORM.
* **Frontend:** Vue.js 2, Tailwind CSS, Vite, Axios.
* **Librerías Clave:** Laravel Sanctum, FullCalendar, Vue Router, SweetAlert2, Vue Toastification.

---

## ⚙️ Instalación y Despliegue Local

Sigue estos pasos para probar el proyecto en tu máquina:

1.  **Clonar el repositorio**
    ```bash
    git clone [https://github.com/TU_USUARIO/crm-tatuajes.git](https://github.com/TU_USUARIO/crm-tatuajes.git)
    cd crm-tatuajes
    ```

2.  **Instalar dependencias (Backend & Frontend)**
    ```bash
    composer install
    npm install
    ```

3.  **Configurar entorno**
    * Copia el archivo de entorno: `cp .env.example .env`
    * Crea una base de datos vacía (ej: `crm_tatuajes`).
    * Configura las credenciales de DB en el archivo `.env`.

4.  **Inicializar la aplicación**
    ```bash
    php artisan key:generate
    php artisan migrate:fresh --seed
    ```
    *(Este comando crea las tablas e inserta datos de prueba iniciales)*.

5.  **Ejecutar servidores**
    * Terminal 1: `php artisan serve`
    * Terminal 2: `npm run dev`

6.  **Acceder**
    Visita `http://127.0.0.1:8000`

---

## 🔑 Credenciales de Prueba

El seeder crea un usuario administrador por defecto:

* **Email:** `test@example.com`
* **Contraseña:** `password`

---

## 👤 Autor

**Daniel Meléndez Loreto** - Desarrollador Full Stack
www.linkedin.com/in/daniel-meléndez-loreto-b51350115
