<div align="center">

# 🌸 Calidad de Software 🎀

<p><i>"Quality is not an act, it is a habit." ✨</i></p>

<!-- Badges Aesthetic -->
<img src="https://img.shields.io/badge/Materia-Calidad_de_Software-ffb6c1?style=for-the-badge&logoColor=white" />
<img src="https://img.shields.io/badge/Estado-En_Proceso_💖-ffc0cb?style=for-the-badge" />
<img src="https://img.shields.io/badge/Testing-Jest_%7C_E2E-ffd1dc?style=for-the-badge" />

<br/><br/>

<!-- Iconos de la Tech Stack pastel -->
<a href="#">
  <img src="https://skillicons.dev/icons?i=ts,js,nestjs,react,github,vscode&theme=light" alt="Tech Stack" />
</a>

<br/><br/>

---

### 🎀 Información de la Estudiante
* <b>Estudiante:</b> Karen Lizeth Inapanta Carrera  
* <b>Asignatura:</b> Calidad de Software  
* <b>Semestre:</b> 2026-I  

---

</div>

## 📌 Tabla de Contenidos
- [✨ Sobre el Repositorio](#-sobre-el-repositorio)
- [🌷 Conceptos Clave de Calidad](#-conceptos-clave-de-calidad)
- [🧪 Pruebas de Software (Testing)](#-pruebas-de-software-testing)
  - [🧩 Pruebas Unitarias](#1-pruebas-unitarias-unit-testing)
  - [🌐 Pruebas End-to-End (E2E)](#2-pruebas-end-to-end-e2e)
- [💻 Tecnologías & Herramientas](#-tecnologías--herramientas)
- [📂 Estructura del Repositorio](#-estructura-del-repositorio)

---

## ✨ Sobre el Repositorio

¡Bienvenidx! 🌸 Este repositorio contiene las actividades, talleres, guías y proyectos enfocados en la **Aseguración y Control de la Calidad del Software (QA)**. Aquí aplicamos mejores prácticas de desarrollo, estándares de código y estrategias de automatización de pruebas para construir software robusto, escalable y libre de errores.

---

## 🌷 Conceptos Clave de Calidad

### 🌺 1. Calidad de Software
Es el grado en el que un sistema, componente o proceso cumple con los requisitos especificados y con las necesidades o expectativas del cliente/usuario.

### 💖 2. QA (Quality Assurance) vs. QC (Quality Control)
* **QA (Aseguramiento de la Calidad):** Se enfoca en los *procesos*. Su objetivo es prevenir fallos definiendo estándares y metodologías desde el inicio del desarrollo.
* **QC (Control de Calidad):** Se enfoca en el *producto final*. Su objetivo es identificar y corregir defectos mediante la ejecución de pruebas.

### 🎀 3. Criterios de Aceptación & Refactorización
* **Criterios de Aceptación:** Condiciones específicas que debe cumplir una funcionalidad para ser aprobada por el usuario o cliente.
* **Refactorización:** Proceso de reestructurar el código existente sin cambiar su comportamiento externo para mejorar su legibilidad, mantenibilidad y rendimiento.

---

## 🧪 Pruebas de Software (Testing)

El testing nos ayuda a garantizar que nuestro código funcione como se espera antes de llegar a producción.

```text
       / \         <- 🌐 Pruebas E2E (Pocas, lentas, interfaz completa)
      /   \
     /-----\       <- 🔗 Pruebas de Integración (Interacción entre módulos)
    /       \
   /---------\     <- 🧩 Pruebas Unitarias (Muchas, rápidas, aisladas)
```

---

### 1. 🧩 Pruebas Unitarias (Unit Testing)
Son pruebas de bajo nivel enfocadas en verificar el correcto funcionamiento de **una unidad individual de código** (como una función, un componente aislado o una clase), de manera completamente independiente del resto del sistema.

* **Objetivo:** Aislar cada parte del programa y demostrar que individualmente funciona correctamente.
* **Herramientas comunes:** Jest, Vitest, React Testing Library.
* **Ejemplo rápido (Jest):**
```typescript
// suma.ts
export const sumar = (a: number, b: number): number => a + b;

// suma.spec.ts
import { sumar } from './suma';

describe('Prueba unitaria para función sumar 🌸', () => {
  it('debe retornar 5 al sumar 2 + 3', () => {
    expect(sumar(2, 3)).toBe(5);
  });
});
```

---

### 2. 🌐 Pruebas End-to-End (E2E)
Las pruebas "de extremo a extremo" simulan el comportamiento del **usuario real** interactuando con la aplicación completa de principio a fin (Frontend + Backend + Base de datos).

* **Objetivo:** Validar el flujo de trabajo completo del sistema y asegurar la integración de todos sus componentes.
* **Herramientas comunes:** Cypress, Playwright, Supertest + Jest (en NestJS).
* **Ejemplo rápido (Playwright / Cypress concept):**
```typescript
describe('Flujo de Iniciar Sesión 💖', () => {
  it('permite a un usuario iniciar sesión exitosamente', () => {
    cy.visit('/login');
    cy.get('input[name="email"]').type('karen@example.com');
    cy.get('input[name="password"]').type('123456');
    cy.get('button[type="submit"]').click();
    cy.url().should('include', '/dashboard');
  });
});
```

---

## 💻 Tecnologías & Herramientas

| Categoría | Tecnología / Herramienta |
| :--- | :--- |
| **Lenguaje principal** | TypeScript / JavaScript |
| **Frameworks** | NestJS (Backend) & ReactJS (Frontend) |
| **Testing Unitario** | Jest & React Testing Library |
| **Testing E2E** | Cypress / Playwright / Supertest |
| **Linter & Formato** | ESLint & Prettier |

---

## 📂 Estructura del Repositorio

```text
🎀 calidad-de-software/
 ├── 📄 README.md
 ├── 📄 .gitignore
 ├── 📁 01-fundamentos-qa/      # Conceptos, métricas y estándares
 ├── 📁 02-pruebas-unitarias/    # Prácticas con Jest y funciones aisladas
 ├── 📁 03-pruebas-e2e/          # Flujos completos de integración y testing E2E
 └── 📁 04-proyecto-integrador/ # Proyecto final auditado con calidad
```

---

<div align="center">

*Hecho con 💖 y dedicación por **Karen Inapanta** ✨*

</div>