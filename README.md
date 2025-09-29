# 🧪 Laboratorio [Creación de un Proyecto en Laravel con Login]

## 💻 Objetivo del Laboratorio

Este laboratorio tiene como objetivo principal conocer la estructura fundamental de un proyecto en Laravel, entender cómo el framework organiza sus componentes siguiendo el patrón Modelo-Vista-Controlador (MVC) y valorar la relevancia de esta arquitectura en la creación de aplicaciones web actuales.


## 🛠 Arquitectura y Estructura (Patrón MVC)

Laravel se basa en el patrón de arquitectura *Modelo-Vista-Controlador (MVC)*, que organiza el código en torno a tres componentes principales para mejorar la modularidad y el mantenimiento:


| Carpeta | Componente MVC | Función Principal | 
| app/Models | Modelo | Define la lógica de negocio y las relaciones con la base de datos.| 
| app/Http/Controllers | Controlador | Recibe las peticiones del usuario, invoca la lógica del modelo y selecciona la vista a mostrar.| 
| resources/views | Vista | Contiene el código de la interfaz de usuario (HTML/Blade).| 
| routes/web.php | Rutas | Define las URLs y las acciones que ejecutan los controladores. | 


## Requisitos del Ecosistema

Para ejecutar este laboratorio localmente, es necesario tener configurado el siguiente entorno de desarrollo.

a
| Prerrequisito | Versión Requerida | Estado | 
| PHP | 8.0 o superior | ✔ | 
| Composer | Última versión estable | ✔ | 
| Instalador de Laravel | Proyecto creado con composer create-project | ✔ | 
| Entorno de Servidor Web Local | WampServer | ✔ | 
| Servidor Web | Apache | ✔ | 
| Base de Datos | MySQL funcionando | ✔ | 
| Editor de Código | Visual Studio Code | ✔ | 
| NPM | No fue necesario | — | 
| Sistema Operativo | Windows 11 | ✔ | 


## Proceso de Instalación y Configuración

A continuación se documenta la secuencia de comandos utilizados para inicializar el proyecto, instalar dependencias y configurar la autenticación.


### 1. Inicialización y Dependencias


| Comando | Descripción | 
| composer create-project laravel/laravel nombre-del-proyecto | Crea el proyecto base de Laravel. | 
| cd nombre-del-proyecto | Accede al directorio del proyecto. | 
| cp .env.example .env | Crea el archivo de configuración del entorno. | 
| php artisan key:generate | Genera la clave de aplicación. | 


### 2. Instalación del Paquete de Autenticación


*Comandos utilizados para la Autenticación:*

composer require laravel/ui
php artisan ui bootstrap --auth
npm install && npm run dev 

# Este proceso genera las vistas de login, registro y recuperación de contraseña, además de compilar los assets necesarios para su visualización.



### 🚗 Comandos utilizados para migraciones

php artisan migrate


### 📂Respaldo de la base de datos

Para generar un backup:

mysqldump -u usuario -p nombre_base_de_datos > database/backups/backup_lab2arelys.sql


## 🖼️Resultado Visible

![Captura de pantalla del laboratorio] (C:/wamp64/www/lab2arelys/Imagenes/Laravel.png)


##  ⚠Dificultades y Soluciones

- Errores con NPM y compilación de assets: Al ejecutar npm install, surgieron errores relacionados con permisos, versiones de Node.js o paquetes faltantes, Se solucionó actualizando Node.js a una versión estable.
- Conflictos con dependencias de Composer: Al instalar Laravel/ui, se presentaron advertencias sobre versiones incompatibles. Se resolvió ejecutando composer install y actualizando los paquetes mediante composer update, además de revisar el archivo composer.json para asegurar la compatibilidad con PHP 8.0.

##📚 Referencias


[1]Laravel Documentation, “Laravel 10.x Documentation,” Laravel, 2025. [Online]. Available: https://laravel.com/docs/10.x
[2]Brito, “Laravel Migrations,” DEV Community, Sep. 2021. [Online]. Available: https://dev.to/rogeriobrito/laravel-migrations-4g5p
[3]Laravel Documentation, “Blade Templates,” Laravel, 2025. [Online]. Available: https://laravel.com/docs/10.x/blade


## 📝Footer

> Este laboratorio ha sido desarrollado por el estudiante de la Universidad Tecnológica de Panamá:  
> *Nombre:* Arelys Carrion 
> *Correo:* arelys.carrion@utp.ac.pa  
> *Curso:* Ingeniería Web  
> *Instructor del Laboratorio:* Irina Fong.


## 📅  Fecha de Ejecución

*Fecha:* 29 de octubre de 2025