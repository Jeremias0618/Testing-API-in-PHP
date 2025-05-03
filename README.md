
# API de Prueba en PHP

Este proyecto es una prueba técnica de una API RESTful desarrollada en PHP puro, sin frameworks. El objetivo principal es demostrar la estructura básica y funcionamiento de una API sencilla utilizando buenas prácticas de programación y arquitectura.

## 📁 Estructura del Proyecto

```

/api-prueba-php
│
├── public/               # Punto de entrada (index.php)
├── src/                  # Lógica principal de la API
│   ├── controllers/      # Controladores de las rutas
│   ├── models/           # Modelos de datos (POPOs o acceso a BD)
│   ├── routes/           # Definición de endpoints
│   └── core/             # Clases base (router, request, response, etc.)
│
├── config/               # Configuración general y de base de datos
├── .htaccess             # Redirección para URLs limpias
├── composer.json         # Dependencias (si se usa Composer)
└── README.md             # Documentación del proyecto

````

## 🧪 Requisitos

- PHP 7.4 o superior
- Servidor web Apache o Nginx
- Composer (opcional, si se usan dependencias externas)
- MySQL/MariaDB (opcional, si la API se conecta a base de datos)

## 🚀 Instalación

1. Clona el repositorio:

```bash
git clone https://github.com/usuario/api-prueba-php.git
cd api-prueba-php
````

2. Configura tu entorno:

* Asegúrate de apuntar tu servidor web a la carpeta `public/`
* Copia y edita los archivos de configuración:

```bash
cp config/config.sample.php config/config.php
```

3. Inicia el servidor embebido de PHP (para pruebas):

```bash
php -S localhost:8000 -t public
```

## 📡 Endpoints de Ejemplo

| Método | Ruta            | Descripción            |
| ------ | --------------- | ---------------------- |
| GET    | /api/usuarios   | Listar usuarios        |
| GET    | /api/usuarios/1 | Obtener usuario por ID |
| POST   | /api/usuarios   | Crear nuevo usuario    |
| PUT    | /api/usuarios/1 | Actualizar usuario     |
| DELETE | /api/usuarios/1 | Eliminar usuario       |

## ⚙️ Tecnologías Usadas

* PHP nativo
* JSON como formato de respuesta
* Ruteo personalizado
* Manejo básico de errores HTTP

## ✅ Funcionalidades

* Routing básico sin frameworks
* Validación de parámetros
* Envío de respuestas JSON
* Código modular y escalable
* Soporte para CORS (Cross-Origin Resource Sharing)

## 🧩 Posibles Mejoras

* Integración con base de datos usando PDO
* Autenticación JWT
* Pruebas unitarias con PHPUnit
* Implementación de middleware


