# Semana 13: Desarrollo Backend PHP con Laravel

## 1. Introducción
En esta semana se desarrollaron aplicaciones web del lado servidor utilizando **PHP** y el framework **Laravel**.  
Se revisó el funcionamiento del servidor **Apache** junto con PHP, el proceso de interpretación del código PHP y su conversión a HTML, además de la estructura moderna de desarrollo que ofrece Laravel bajo el patrón **MVC (Modelo–Vista–Controlador)**.

![PHP y Apache](../img/img01sem13.png)

---

## 2. Lo que vimos en clase
- Funcionamiento del servidor **Apache HTTP Server** y ejecución de **PHP**.  
- Instalación de PHP desde archivos ZIP y configuración del archivo **php.ini**.  
- Uso del archivo **httpd.conf** para configurar Apache (DocumentRoot, Listen, ServerName).  
- Instalación y uso de **Composer** como gestor de dependencias en PHP.  
- Sintaxis básica de PHP: variables, condicionales, bucles y funciones.  
- Introducción al framework **Laravel** y su estructura de directorios.

![Flujo Apache PHP](../img/img02sem13.png)

---

## 3. Conceptos clave de PHP

| Elemento     | Descripción                   | Ejemplo               |
|--------------|-------------------------------|---------------------|
| Variables    | Se declaran con `$`           | `$nombre = "Ana";`  |
| Condicionales| Controlan el flujo del programa| `if ($edad >= 18)` |
| Bucles       | Repiten bloques de código     | `for, while, foreach` |
| Funciones    | Permiten reutilizar lógica    | `function saludar()` |

---

## 4. Introducción a Laravel
Laravel es un framework de PHP de código abierto que facilita el desarrollo de aplicaciones web modernas.  
Se basa en el patrón **MVC** y ofrece herramientas como:

- **Rutas**  
- **Controladores**  
- **Vistas Blade**  
- **Eloquent ORM**  
- **Middleware**  
- **Artisan** (automatización de tareas)

![Estructura Laravel](../img/img03sem13.JPG)

---

## 5. Ejercicio de Laboratorio
En el laboratorio se desarrolló una aplicación web en Laravel para registrar estudiantes. Las principales actividades fueron:

- Creación de un proyecto Laravel usando:

```bash
laravel new nombre_proyecto

