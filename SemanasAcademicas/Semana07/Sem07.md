
# Semana 7: React + Vite (TypeScript)

## Tema
Creación de Aplicaciones Modernas con React y Vite empleando TypeScript.

## Objetivo

Durante esta semana se desarrolló un proyecto combinando **React, Vite y TypeScript**, aprovechando la rapidez de Vite y la solidez del tipado estático de TypeScript.  
Este enfoque permite construir aplicaciones más estables, seguras y fáciles de mantener a largo plazo.

---

## ¿Qué es TypeScript?

**TypeScript (TS)** es un **lenguaje basado en JavaScript** que incorpora **tipos estáticos** y herramientas que ayudan a detectar errores antes de ejecutar el código.  
Desarrollado por Microsoft, se **transpila a JavaScript estándar**, por lo que es totalmente compatible con cualquier proyecto que use JS.

| **Aspecto** | **Descripción** |
|--------------|----------------|
| **Creador** | Microsoft |
| **Basado en** | JavaScript (ECMAScript) |
| **Ventajas** | Tipado estático, mejor detección de errores, autocompletado inteligente, compatibilidad con JS |
| **Compilación** | Se convierte a JavaScript usando `tsc`, Vite o Webpack |
| **Ideal para** | Equipos de desarrollo y proyectos de gran escala |

---

## React + Vite + TypeScript

La combinación de **React** con **Vite** y **TypeScript** ofrece un entorno de trabajo ágil, confiable y moderno.  
Vite permite un inicio casi instantáneo, mientras que TypeScript garantiza que el código sea más predecible y consistente.

| **Ventaja** | **Descripción** |
|--------------|----------------|
| **Velocidad** | Vite inicia el entorno de desarrollo en segundos y actualiza los cambios en tiempo real. |
| **Calidad del código** | TypeScript evita errores antes de ejecutar la aplicación. |
| **Eficiencia** | Ofrece sugerencias, autocompletado y una mejor refactorización. |
| **Fiabilidad** | Minimiza errores como referencias nulas o tipos incorrectos. |
| **Mantenimiento** | Permite escalar y organizar mejor el proyecto con el tiempo. |

---

## Pasos para crear un proyecto React + Vite + TypeScript

| **Paso** | **Comando / Descripción** |
|-----------|----------------------------|
| **1. Crear proyecto** | `npm create vite@latest nombreProyecto` |
| **2. Seleccionar framework** | Escoger `React` y luego la opción `TypeScript` |
| **3. Acceder al proyecto** | `cd nombreProyecto` |
| **4. Instalar dependencias** | `npm install` |
| **5. Ejecutar servidor local** | `npm run dev` |
| **6. Visualizar en navegador** | Abrir `http://localhost:5173/` |

---

## 🧱 Estructura básica del proyecto

| **Carpeta / Archivo** | **Descripción** |
|------------------------|----------------|
| `/src` | Contiene todo el código principal (componentes, hooks, utilidades). |
| `/src/App.tsx` | Componente base de la aplicación con tipado TSX. |
| `/src/main.tsx` | Punto inicial de carga de React. |
| `/public` | Archivos estáticos como imágenes y fuentes. |
| `index.html` | Archivo raíz que carga la aplicación. |
| `vite.config.ts` | Configuración de Vite en formato TypeScript. |
| `tsconfig.json` | Archivo de configuración para el compilador de TypeScript. |

---

## 💻 Ejemplo básico en React + TypeScript

```tsx
// src/App.tsx
import React from 'react'

// Definición de tipos con TypeScript
interface User {
  name: string
  age: number
}

const App: React.FC = () => {
  const user: User = { name: 'Lucía', age: 23 }

  return (
    <div style={{ textAlign: 'center', marginTop: '50px' }}>
      <h1>⚡ React + Vite + TypeScript</h1>
      <p>Hola, <strong>{user.name}</strong> 👋</p>
      <p>Edad: {user.age} años</p>
    </div>
  )
}

export default App
