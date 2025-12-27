# Semana 09: Desarrollo Backend (Arquitecturas, Servidores, Tomcat y Seguridad)

![Arquitectura cliente-servidor](../img/img01sem09.png)

Esta semana se estudió cómo funcionan las aplicaciones web del lado servidor (backend), revisando las principales arquitecturas (MPA, SPA, multicapa y hexagonal), el rol de los servidores web, hosting y cloud, la administración básica de servidores (dominios, DNS y parámetros de configuración), el funcionamiento del server-side con Apache/PHP y Tomcat/JSP, además de herramientas como Maven para dependencias y el uso de autenticación basada en tokens (JWT, OAuth, SAML).

---

## Lo que vimos en clase

### 🖥️ Arquitecturas Web
- **MPA:** multipágina, recargas y rutas por páginas.
- **Multicapa/MVC:** separación por responsabilidades.
- **SPA:** una sola página, navegación con JS y el servidor envía datos.
- **Híbridas (SPA/MPA):** combinación de enfoques (ej. Next.js).
- **Hexagonal:** puertos y adaptadores para independencia y testeo.

### 🌐 Servidores, Hosting y Cloud
- **Servidor web:** entrega contenido por HTTP (Apache, NGINX, IIS, Tomcat, etc.).
- **Hosting:** compartido, VPS, dedicado, administrado y cloud.
- **Cloud:** recursos bajo demanda, escalable, pago por uso.

![MPA vs SPA](../img/img02sem09.jpg)

---

## Administración y configuración de servidores

Se revisó la gestión del nombre de dominio (DNS), su estructura (nombre + extensión) y la importancia del dominio para la identidad y marketing. También se estudiaron parámetros esenciales de configuración en servidores web:

| Parámetro       | ¿Qué controla?                          | Ejemplo            |
|-----------------|----------------------------------------|------------------|
| DocumentRoot    | Carpeta raíz donde están los archivos públicos del sitio | /var/www/html    |
| Listen          | Puerto donde escucha el servidor        | 80 (HTTP) / 443 (HTTPS) |
| DirectoryIndex  | Archivo que se abre por defecto         | index.html       |
| SSLEngine       | Habilita HTTPS con SSL/TLS              | On               |
| MaxClients      | Máximo de conexiones simultáneas        | 150              |

---

## Funcionamiento del Server Side

El flujo general inicia cuando el navegador envía una solicitud HTTP. El servidor interpreta la petición, ejecuta el código backend (PHP/Node/Python/Java), consulta la base de datos si es necesario y finalmente devuelve una respuesta (HTML, JSON o XML).

![Flujo request/response](../img/img03sem09.png)

---

## Tomcat, Maven y Token Authentication

Se estudió Apache Tomcat como contenedor de servlets y JSP, su estructura de directorios (bin, conf, logs, webapps, work/temp) y componentes internos. Además, Maven para gestionar dependencias mediante **pom.xml** y su ciclo de vida (compile, test, package, install, deploy). Finalmente, autenticación basada en tokens (JWT, OAuth, SAML).

### 🔹 Tomcat
Contenedor Java para servlets/JSP. Procesa peticiones HTTP y genera respuestas HTML.

### 🔹 Maven
Gestiona dependencias y builds. Usa **pom.xml** y automatiza compile/test/package/deploy.

### 🔹 Tokens
Autenticación sin enviar credenciales siempre: token → validación → expiración/renovación.

![JWT flow](../img/img04sem09.png)

---

## Reflexión

Comprendí que el backend es el “motor” de una aplicación web: recibe solicitudes, procesa lógica, accede a bases de datos y devuelve respuestas al cliente. Elegir una arquitectura adecuada (MPA, SPA, multicapa o hexagonal) impacta directamente en el mantenimiento, escalabilidad y seguridad del sistema. Tomcat y Maven muestran cómo se organiza el desarrollo Java profesional, y los tokens (como JWT) son esenciales para autenticación moderna en APIs.

---

## Referencias

- Guía/diapositivas del docente (DesarrolloBackend.pdf).  
- [Apache Maven Documentation](https://maven.apache.org) (Conceptos de POM y ciclo de vida).  
- [Apache Tomcat Documentation](https://tomcat.apache.org) (estructura y configuración).  
- [OWASP](https://owasp.org) (buenas prácticas de autenticación con tokens/JWT).  

