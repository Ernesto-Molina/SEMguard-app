# SEMguard - Sistema de Gestión de Guardias

SEMguard es una aplicación web (SPA) para la gestión del personal de seguridad, permitiendo a los administradores supervisar al personal y a los guardias registrar sus turnos de entrada y salida con geolocalización.

## Arquitectura

La aplicación utiliza una arquitectura **Backend as a Service (BaaS)**:

- **Frontend:** Una Single Page Application (SPA) construida con **HTML, CSS y JavaScript (Vanilla JS)**.
- **Backend:** **Google Firebase**, que provee la base de datos y la sincronización en tiempo real.
- **Base de Datos:** **Cloud Firestore** (NoSQL).
- **Hosting:** **Firebase Hosting**, **Url:** `https://proyectoarqui-dffa4.web.app/`

## Despliegue y Ejecución

La aplicación no requiere un proceso de build ni dependencias de servidor.

1.  **Clona o descarga este repositorio.**
2.  **Abre la carpeta `public`**
3.  **Abre el archivo `index.html`** en cualquier navegador web moderno.

Es necesaria una conexión a internet para que la aplicación pueda conectarse a los servicios de Firebase.

## Funcionalidades Principales

### Panel de Administrador
-   Inicio de sesión seguro.
-   Visualización de todo el personal en una tabla responsiva.
-   Creación, Edición y Eliminación (CRUD) de personal.
-   Reseteo de contraseñas para los guardias.
-   Centro de notificaciones en tiempo real para entradas/salidas.
-   Mapa interactivo para ver la ubicación de los guardias activos.

### Portal de Guardia
-   Inicio de sesión seguro.
-   Marcar entrada y salida del turno.
-   La marcación de entrada captura la geolocalización del dispositivo.
-   Visualización del historial de marcas del día.
-   Opción para cambiar la propia contraseña.

## Estructura del Código
El código está contenido en un único archivo index.html y está organizado de la siguiente manera: 
1. HTML: Estructura de todas las vistas y modales.
2. CSS: Estilos para todos los componentes, incluyendo diseño responsivo para móviles
3. JavaScript:
   - Configuración de Firebase.
   - Estado global y variables.
   - Lógica de autenticación y navegación.
   - Funciones de validación.
   - Lógica de renderizado para cada panel (Admin/Guardia).
   - Funciones CRUD y manejo de modales.
   - Listeners de eventos.
   - Funciones de ayuda (Utilities).


