# Práctica de Laboratorio 01: Manejo de Visual Studio Code

## Objetivo General
Reconocer, configurar y utilizar el entorno de desarrollo integrado **Visual Studio Code**, aplicando comandos de **Git**, atajos del teclado y herramientas como **Emmet** y **Codespaces**.

---

## Ejercicio 01: Reconocimiento de la herramienta Visual Studio Code
**Objetivo:**  
Reconocer y utilizar la herramienta de desarrollo integrado **Visual Studio Code**, sus **áreas principales** (editor, barra lateral, terminal, barra de estado, mini mapa, etc.) y las **aplicaciones del menú principal** (Archivo, Edición, Ver, Ejecutar, Terminal, Ayuda).

**Actividad sugerida:**  
1. Abrir Visual Studio Code.  
2. Explorar las áreas de la interfaz.  
3. Describir brevemente la función de cada una en un documento `areas_vscode.md`.

---

## Ejercicio 02: Activación de la Paleta de Comandos
**Objetivo:**  
Activar y usar la **Paleta de comandos** para ejecutar funciones de manera rápida.

**Ejemplo práctico:**  
- Abrir la Paleta con `Ctrl + Shift + P` o `F1`.  
- Buscar y ejecutar el comando **"GitHub Codespaces: Create New Codespace"**.  
- Observar cómo se inicia un entorno de desarrollo en la nube.

---

## Ejercicio 03: Uso de la Terminal Integrada con Git
**Objetivo:**  
Utilizar la terminal de **Visual Studio Code** para manejar repositorios **Git** y comprender el flujo básico de control de versiones.

**Ejemplo práctico:**
```bash
# Inicializar un repositorio
git init

# Agregar archivos al área de preparación
git add .

# Confirmar los cambios
git commit -m "Primer commit"

# Crear una nueva rama
git checkout -b desarrollo

# Fusionar ramas
git merge desarrollo

# Subir los cambios al repositorio remoto
git push origin main
```

## Ejercicio 04: Uso de Emmet y Fragmentos de Código
**Objetivo:**  
Acelerar la escritura de código mediante **Emmet** y la creación de **snippets** personalizados en Visual Studio Code.

---

### Ejemplo con Emmet

**Código:**
```html
div.container>header>h1{Bienvenidos}+nav>ul>li*3>a{Enlace $}
```
## Ejercicio 05: Uso de Keyboard Shortcuts en Visual Studio Code

**Objetivo:**  
Optimizar el flujo de trabajo mediante el uso de **atajos de teclado (keyboard shortcuts)** en Visual Studio Code, mejorando la productividad y la rapidez al escribir código.

---

### Descripción

Visual Studio Code ofrece una gran variedad de **atajos de teclado** que permiten ejecutar acciones sin necesidad de usar el ratón.  
Conocerlos y aplicarlos facilita tareas como abrir archivos, ejecutar el terminal, cambiar entre ventanas, o formatear código de manera más eficiente.

---

### Ejemplos de Atajos Comunes

| Acción | Atajo (Windows/Linux) | Atajo (Mac) |
|:-------|:----------------------|:------------|
| Abrir la Paleta de Comandos | `Ctrl + Shift + P` | `Cmd + Shift + P` |
| Abrir Terminal integrada | `Ctrl + ñ` o `Ctrl + `` | `Cmd + `` |
| Formatear documento | `Shift + Alt + F` | `Shift + Option + F` |
| Comentar línea | `Ctrl + /` | `Cmd + /` |
| Seleccionar toda la línea | `Ctrl + L` | `Cmd + L` |
| Buscar en archivo | `Ctrl + F` | `Cmd + F` |
| Buscar en proyecto | `Ctrl + Shift + F` | `Cmd + Shift + F` |
| Duplicar línea | `Shift + Alt + ↓` | `Shift + Option + ↓` |
| Mover línea arriba/abajo | `Alt + ↑ / ↓` | `Option + ↑ / ↓` |

---

