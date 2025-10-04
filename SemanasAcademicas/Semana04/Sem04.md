
# Semana 04 – Frameworks CSS y Fundamentos de JavaScript

---

## **Bootstrap**

**Objetivo:**  
Comprender el uso del framework **Bootstrap** para crear diseños responsivos y componentes visuales reutilizables con mínima codificación CSS.

---

**1. Sistema de Grid y Diseño Responsivo**  
Bootstrap se basa en un sistema de rejilla (Grid System) compuesto por 12 columnas que permite distribuir el contenido de manera adaptable según el tamaño de pantalla.  
Mediante clases como `col-sm`, `col-md`, `col-lg`, y `col-xl`, se ajustan los elementos automáticamente para dispositivos móviles, tabletas y pantallas grandes.

**2. Componentes Predefinidos y Tipografía**  
Bootstrap incluye una amplia colección de componentes visuales como botones, tarjetas, modales, alertas y barras de navegación.  
Estos elementos se personalizan fácilmente mediante clases predefinidas, garantizando coherencia visual y buena experiencia de usuario.  
Además, ofrece un sistema de tipografía escalable, con clases como `text-center`, `fw-bold`, o `lead` para resaltar contenido textual.

**3. Formularios, Validaciones y Clases de Utilidad**  
El framework facilita la creación de formularios modernos, con estilos uniformes y validaciones integradas.  
Las clases de utilidad permiten controlar el espaciado (`m-3`, `p-2`), la alineación (`d-flex`, `justify-content-center`) y la visibilidad (`d-none`, `d-block`) de forma rápida sin escribir CSS adicional.

**4. Personalización y Tematización**  
Bootstrap es totalmente personalizable a través de variables CSS y preprocesadores como **SASS**.  
Esto permite modificar colores, tipografías o espaciados de manera centralizada, adaptando el estilo a la identidad visual del proyecto.

**5. Integración con JavaScript y Componentes Interactivos**  
Incluye soporte para **JavaScript nativo** que potencia componentes interactivos como tooltips, dropdowns, modales y carruseles.  
Estos se activan fácilmente mediante atributos como `data-bs-toggle` o funciones JS integradas, optimizando la interactividad del sitio sin necesidad de librerías externas.

---

## **Tailwind CSS**

**Objetivo:**  
Aplicar el enfoque **Utility-First** de Tailwind para construir interfaces modernas mediante clases utilitarias rápidas y un alto grado de personalización.

---

**1. Clases Utilitarias y Diseño Responsivo**  
Tailwind CSS usa clases atómicas como `m-4`, `text-lg`, `bg-blue-500`, que permiten aplicar estilos directamente en los elementos HTML.  
Su sistema responsivo basado en `sm`, `md`, `lg`, `xl` y `2xl` permite adaptar el diseño a distintos tamaños de pantalla sin necesidad de media queries manuales.

**2. Personalización y Configuración Global**  
El archivo `tailwind.config.js` permite definir paletas de colores, fuentes personalizadas, tamaños de espaciado y variantes.  
Esto facilita mantener una identidad visual consistente en todo el proyecto.

**3. Flexbox, Grid y Dark Mode**  
Tailwind facilita el diseño estructural mediante clases como `flex`, `grid`, `gap-4`, o `place-items-center`.  
Además, soporta **Dark Mode** y variantes de estado (`hover`, `focus`, `active`) para lograr una experiencia visual moderna y adaptable.

**4. Optimización y Rendimiento**  
Con **PurgeCSS**, se eliminan automáticamente las clases no utilizadas en producción, reduciendo el tamaño final de los archivos CSS y mejorando la velocidad de carga.  
Asimismo, Tailwind incluye animaciones y efectos simples (`transition`, `transform`, `shadow`) para añadir dinamismo al diseño.

**5. Integración y Componentización**  
Tailwind puede integrarse fácilmente con frameworks modernos como **React**, **Vue** o **Next.js**, permitiendo crear componentes reutilizables y eficientes mediante la directiva `@apply` y estilos combinados.

---

## **JavaScript Básico**

**Objetivo:**  
Dominar los fundamentos de **JavaScript**, el lenguaje que otorga interactividad y dinamismo a las páginas web.

---

**1. Sintaxis, Variables y Tipos de Datos**  
JavaScript se ejecuta directamente en el navegador y utiliza variables (`let`, `const`, `var`) para almacenar información.  
Soporta múltiples tipos de datos: cadenas, números, booleanos, arreglos y objetos.

**2. Estructuras de Control y Funciones**  
Se emplean condicionales (`if`, `else`, `switch`) y bucles (`for`, `while`) para manejar la lógica del programa.  
Las funciones permiten reutilizar código y manejar operaciones dinámicas con parámetros y valores de retorno.

**3. Manipulación del DOM y Eventos**  
Uno de los pilares de JavaScript es la interacción con el DOM (Document Object Model), mediante el cual se pueden crear, modificar o eliminar elementos en tiempo real.  
Los eventos (`click`, `change`, `mouseover`) se controlan con métodos como `addEventListener` para generar interactividad.

**4. Almacenamiento Local y JSON**  
JavaScript permite guardar información persistente usando **LocalStorage** o **SessionStorage**.  
Además, JSON se usa para estructurar y transferir datos entre cliente y servidor de manera eficiente.

**5. Depuración y Consola**  
El uso de herramientas como `console.log` y `debugger` facilita el seguimiento del flujo de ejecución y la corrección de errores, fundamental en el desarrollo web.

---

## **JavaScript Avanzado**

**Objetivo:**  
Comprender conceptos avanzados de programación y control de asincronía para el desarrollo de aplicaciones web modernas y escalables.

---

**1. Programación Orientada a Objetos y DOM Avanzado**  
Se introducen clases, herencia y el uso de `this` y `prototype` para modelar comportamientos complejos.  
La manipulación avanzada del DOM incluye creación dinámica de elementos, atributos y estilos desde el código.

**2. Asincronía, Promesas y Fetch API**  
El manejo asincrónico mediante **Promesas**, **async/await** y **Fetch API** permite realizar peticiones a servidores y consumir APIs sin bloquear la interfaz del usuario.

**3. Canvas, Gráficos y WebSockets**  
A través del elemento `<canvas>` se pueden generar gráficos y animaciones.  
Con **WebSockets**, se logra comunicación en tiempo real entre cliente y servidor, ideal para aplicaciones interactivas como chats o tableros de control.

**4. Gestión de Errores y Rendimiento**  
Se aplican estructuras `try-catch` y lanzamiento de excepciones (`throw`) para el control de errores.  
Además, se optimiza el rendimiento con técnicas como **Web Workers**, que ejecutan tareas en segundo plano.

**5. Closures, Scope y Buenas Prácticas**  
El uso de closures y scopes define el alcance y persistencia de variables, garantizando una programación estructurada y segura.  
Estas técnicas son base fundamental para entender frameworks modernos y desarrollo modular en JavaScript.

---

## **Conclusión**

Durante esta semana se consolidaron los conocimientos en **frameworks CSS modernos (Bootstrap y Tailwind)** y se profundizó en **JavaScript**, desde su base hasta conceptos avanzados.  
Se comprendió cómo combinar diseño responsivo, interactividad y optimización del código para desarrollar aplicaciones web más profesionales, dinámicas y eficientes.

---
