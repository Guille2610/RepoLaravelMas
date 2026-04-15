# Laboratorio de Laravel #1 (Setup Inicial)

El laboratorio #1 de Laravel consiste en preparar todo lo necesario para empezar a utilizar este framework como parte de la materia de Desarrollo de Software VII.

## Breve introducción
El MVC o Modelo-Vista-Controlador es un patrón de arquitectura de software que, utilizando 3 componentes (Vistas, Models y Controladores) separa la lógica de la aplicación de la lógica de la vista en una aplicación. En este trabajo nos estaremos preparando para trabajar en este enfoque utilizando entornos como Laravel y Composer, Livewire y Tailwind.

## Prerequisitos (ecosistema de desarrollo)

- **PHP** versión 8.0 o superior 🐘
-  **Composer**, última versión estable ✒️
- **Laravel Installer** ‼️
- **Paquete de servidor web local**(ej. XAMPP, WampServer o Laragon). 💻
- **Servidor web**: Apache o Nginx 🌐
- **Base de datos MySQL/MariaDB** funcionando. 🧾
- **Editor de código** (Visual Studio Code recomendado). ⌨️
- Sistema Operativo: Windows 🪟

## Instalación de dependencias
Antes de instalar las dependencias, podemos revisar que todo esté funcionando aplicando en tu terminal:
```php -v``` para verificar que PHP funciona, y ```composer -v``` para verificar que Composer está instalado.

Los pasos para instalar el resto de dependencias son los siguientes:

1. **Instalar Laravel global**, que instala el comando ```laravel new```.
```
composer global require laravel/installer
```
2. Dirigirse a la carpeta del servidor
```
cd ..\xampp\htdocs
```
3. **Crear el proyecto** Laravel
```
laravel new AppEjemplo-Guille
```
Al ejecutar este comando, automáticamente el Laravel ejecuta el comando de ```composer install```, que instala las dependencias PHP que hacen falta.

Nota: es preferible que cuando se te pregunte durante la ejecución de este comando, escojas el framework de **livewire**, que otorga un diseño de interfaz muy intuitivo.

### Comandos para la migración utilizados

Los comandos utilizados fueron los siguientes:
```
php artisan migrate
```
```
php artisan migrate:fresh
```
```
php artisan migrate:status
```

### Resultados
Los resultados del laboratorio fueron los siguientes:
- Se pudo acceder al portal principal de Laravel

(IMAGEN)
- Se pudo acceder al inicio de sesión y registro del entorno.

(IMAGEN)

## Base de datos y configuración en Laravel

En este laboratorio se utilizó el framework Laravel para la prueba de una aplicación web con autenticación de usuarios.

### 🔧 Configuración del archivo .env

El archivo .env se utilizó para definir los parámetros de conexión a la base de datos. En este caso se configuró una base de datos SQLlite proporcionada por XAMPP.

Ejemplo de configuración:

```
DB_CONNECTION=sqlite
# DB_HOST=127.0.0.1
# DB_PORT=3306
# DB_DATABASE=laravel
# DB_USERNAME=root
# DB_PASSWORD=
``` 

Este archivo permite separar la configuración sensible del código fuente, facilitando la portabilidad del proyecto.

## Dificultades y Soluciones
Las dificultades más aparentes en el desarrollo del proyecto las conforman 
- la cantidad excesiva de pasos
- el desconocimiento de saber para qué sirve cada alternativa que se ofrece durante la instalación del framework.

Las soluciones que se aplicaron fueron la escucha activa y el auto-aprendizaje para abordar una secuencia de pasos extensa.

## Referencias

- https://laravel-livewire.com
- https://codigofacilito.com/articulos/mvc-model-view-controller-explicado
- https://www.ionos.com/es-us/digitalguide/servidores/configuracion/instalar-php-composer-en-windows-10/



