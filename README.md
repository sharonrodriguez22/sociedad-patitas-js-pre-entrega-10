# 🐾 Sociedad Patitas — Pre-Entrega 10

Proyecto desarrollado como parte del curso de **Desarrollo de Aplicaciones** en **Coderhouse**, módulo de **JavaScript**.

## 📖 Descripción

**Sociedad Patitas** es un sitio web para una organización ficticia dedicada al rescate, cuidado y adopción responsable de perros. En esta entrega se integró un **simulador de adopción** con JavaScript directamente en la página de **Adopciones** del sitio web.

El simulador permite consultar los perros disponibles del refugio, completar una solicitud de adopción, apadrinar rescatados y registrar nuevos ingresos al refugio, todo con feedback visual mediante SweetAlert2 y Toastify.

## 🚀 Funcionalidades

**Sitio web (HTML + SCSS):**
- Página de inicio con presentación de la organización.
- Sección de adopciones con simulador interactivo.
- Información sobre servicios.
- Página de sucursales con mapas.
- Formulario de contacto.
- Diseño responsive adaptable a móvil, tablet y desktop.

**Simulador de adopción (JavaScript — PE10):**
- Consumo de API externa (Dog CEO) con `fetch` y `async/await` para fotos de perros.
- Manejo de errores con `try/catch/finally` en todas las peticiones.
- SweetAlert2 para confirmaciones y alertas modales.
- Toastify para notificaciones rápidas no intrusivas.
- Renderizado dinámico del DOM con tarjetas de rescatados.
- Formulario de solicitud de adopción con validación y cuestionario.
- Sistema de padrinazgo para aportar sin adoptar.
- Registro de salidas (adopciones y tránsito).
- Rescatado de la semana destacado.
- Búsqueda por nombre en tiempo real.
- Persistencia de datos con localStorage.
- Alta de nuevos rescatados desde formulario.
- Estadísticas en vivo del refugio.

## 🛠️ Tecnologías utilizadas

- HTML5
- CSS3 / Sass (SCSS)
- JavaScript (ES6+, sin frameworks)
- Fetch API + async/await (Dog CEO API)
- SweetAlert2 (CDN)
- Toastify (CDN)
- localStorage / sessionStorage
- Git & GitHub

## 📂 Estructura del proyecto

```text
├── css/
│   ├── style.css          ← Estilos compilados del sitio web (SCSS)
│   └── simulador.css      ← Estilos del simulador de adopción
├── img/                   ← Imágenes y logos
├── js/
│   ├── config.js          ← Constantes y configuración
│   ├── clases/
│   │   ├── Rescatado.js   ← Clase para los perros del refugio
│   │   └── Solicitud.js   ← Clase para las solicitudes de adopción
│   ├── almacenamiento.js  ← Lectura/escritura en localStorage
│   ├── utilidades.js      ← Funciones auxiliares
│   ├── datos.js           ← Datos iniciales y fetch a la API
│   ├── vista.js           ← Renderizado del DOM
│   ├── avisos.js          ← Sistema de mensajes de feedback
│   └── main.js            ← Eventos y arranque
├── page/
│   ├── adopciones.html    ← Simulador de adopción integrado
│   ├── servicios.html
│   ├── sucursales.html
│   └── contacto.html
├── sass/                  ← Fuentes SCSS del sitio web
├── index.html             ← Página principal
└── README.md
```

## 🎯 Requisitos de la rúbrica PE10

| Criterio | Implementación |
|---|---|
| **Manejo de errores (30%)** | `try/catch/finally` en `cargarFotosDesdeAPI()`, `cargarDestacadoDeLaSemana()` y padrinazgo. Errores de red y validación mostrados al usuario. |
| **Fetch con async/await (25%)** | Consumo de `https://dog.ceo/api/breeds/image/random/N` para fotos aleatorias de perros. Función `async cargarFotosDesdeAPI()` en datos.js. |
| **Librería de modales/alertas (25%)** | SweetAlert2 para confirmaciones (adoptar, tránsito, reiniciar). Toastify para notificaciones rápidas (éxito, info, error). |
| **Renderizado dinámico del DOM (20%)** | Tarjetas generadas con `innerHTML`, estadísticas calculadas, resultado de solicitud, registro de salidas, destacado de la semana. |

## 💻 Cómo ejecutar el proyecto

1. Clonar el repositorio.
2. Abrir `index.html` en el navegador (funciona con protocolo `file://`).
3. Navegar a la página de **Adopciones** para usar el simulador.
4. Las fotos de los perros se cargan desde un agente externo.

## 👩‍💻 Autora

**Sharon Rodríguez**

Proyecto realizado para la carrera de **Desarrollo de Aplicaciones** de **CoderHouse**.
