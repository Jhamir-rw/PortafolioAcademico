# Semana 10: JSP (Jakarta Server Pages) y API REST con Spring Boot

![Tomcat y JSP](../img/img01sem10.jpg)

Esta semana se trabajó con **Apache Tomcat** como servidor web para aplicaciones Java, y se introdujo **JSP (Jakarta Server Pages)** para generar páginas dinámicas combinando **HTML + código Java**. También se revisó el flujo de procesamiento de JSP (traducción a servlet, compilación y ejecución) y se practicó con sintaxis JSP (scriptlets, declaraciones, expresiones, directivas y acciones), además del uso de **objetos implícitos** como `request`, `response`, `out` y `session`. Finalmente, se inició el desarrollo de una **API REST** con **Spring Boot** aplicando estructura MVC, conexión a MySQL y pruebas con Postman.

---

## Lo que vimos en clase

### 🖥️ Apache Tomcat
- Tomcat funciona como contenedor de servlets y JSP.
- Carpetas clave: **bin**, **conf**, **logs**, **webapps**, **work/temp**.
- Archivo principal: **server.xml** (Server, Service, Connector, Engine, Host, Context).
- Parámetros típicos: **port**, **maxThreads**, **connectionTimeout**, **redirectPort**.

### 💻 JSP (Jakarta Server Pages)
- Lenguaje script del lado servidor para construir páginas web dinámicas.
- Se procesa con un motor JSP: intercepta solicitudes y genera la respuesta.
- Flujo: JSP → Servlet → Compilación → Ejecución → HTML final.
- Acceso a APIs Java (incluye JDBC para bases de datos).

![Procesamiento JSP](../img/img02sem10.png)

---

## Sintaxis JSP: elementos principales

| Elemento    | Sintaxis | Descripción |
|------------|----------|------------|
| **Scriptlet** | `<% código Java %>` | Permite incluir Java directo: variables, condicionales y bucles. |
| **Declaración** | `<%! variables o métodos %>` | Define métodos o variables que luego se usan en la página. |
| **Expresión** | `<%= expresión %>` | Imprime el resultado en el HTML renderizado. |

### Directivas, Acciones y Objetos implícitos
- Directivas JSP:
  - `<%@ page %>` → configuración de la página.
  - `<%@ include %>` → inclusión en compilación.
  - `<%@ taglib %>` → bibliotecas de etiquetas.
- Acciones JSP con sintaxis XML: `<jsp:action_name ... />`.
- Objetos implícitos más usados: **request**, **response**, **out**, **session**, **application**, **config**, **pageContext**, **exception**.

| Objeto  | Función | Ejemplo |
|---------|--------|--------|
| `request` | Leer datos de la solicitud (GET/POST) | `request.getParameter("numero")` |
| `out` | Imprimir salida en la página | `out.println("Hola")` |
| `session` | Guardar datos por sesión (visitas, usuario, etc.) | `session.setAttribute("contador", 1)` |

---

## Ejercicios de laboratorio (JSP)
- Mostrar la **fecha y hora actual**: `<%= new java.util.Date() %>`.
- Usar formularios con método **GET** y **POST**, recuperando datos con `request.getParameter()`.
- Ejemplo de **cálculo de factorial**, validando datos del usuario y mostrando resultados con `out.println()`.
- Contar cuántas veces se ejecuta la página en una sesión usando **session** como contador de visitas.

![Código JSP factorial y session](../img/img03sem10.png)

---

## Introducción a Spring Framework y Spring Boot
- **Spring Framework**: framework para aplicaciones empresariales.
- Conceptos: **Inversión de Control (IoC)** y **Inyección de Dependencias (DI)**.
- Spring Container: crea y administra objetos (**beans**) y su ciclo de vida.
- **Spring Boot**: permite crear proyectos Spring rápido, con configuración automática, servidor embebido, métricas y health checks.

![IoC, DI y Spring Container](../img/img04sem10.png)

---

## API REST con Spring Boot (MVC + MySQL + Postman)
- Creación de una API con estructura MVC (controllers, models, repositories, services).
- Conexión a MySQL mediante `application.properties`.
- Ejemplo CRUD con la entidad **Estudiante**, usando **Spring Data JPA**.
- Validación del CRUD mediante pruebas en **Postman**.

![Postman pruebas CRUD](../img/img05sem10.png)
![Postman pruebas CRUD](../img/img06sem10.png)

---

## Reflexión
Aprendí que JSP permite generar páginas dinámicas en Java, pero su verdadero poder aparece cuando se combina con un servidor como Tomcat y conceptos de sesión y formularios. Spring simplifica el desarrollo empresarial mediante IoC y DI, porque el framework se encarga de crear y administrar objetos. Finalmente, Spring Boot permite construir APIs REST con CRUD real (MySQL + JPA) y validarlas profesionalmente con Postman.

---

## Referencias
- Guía del docente: Sem10 DesarrolloBackend JSP2.pdf  
- [Jakarta Pages (JSP)](https://jakarta.ee/specifications/pages/3.0/)  
- [Apache Tomcat Documentation](https://tomcat.apache.org/)  
- [Spring Framework](https://spring.io/)  
- [Spring Boot](https://spring.io/projects/spring-boot)  

