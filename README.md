# bmad-dolar-caro

## 🎯 Visión del Proyecto
Una aplicación web para traducir el valor del dólar a poder de compra real, comparando precios de productos icónicos entre Argentina y otros países. Busca responder de forma simple y visual a la pregunta: **"¿Está caro el dólar en Argentina?"**.

## 📊 Estado Actual
Actualmente, el proyecto ha completado de forma exitosa toda la **Fase de Planificación y Diseño**. Contamos con un plan completo y validado a través de cuatro documentos fundamentales que definen el qué, el porqué y el cómo del proyecto. Estamos listos para iniciar la **Fase de Desarrollo**.

## 🤖 Metodología de Trabajo: BMad-Method
Este proyecto se está desarrollando utilizando el **BMad-Method (Breakthrough Method of Agile AI-driven Development)**. Es un framework que estructura el desarrollo con IA en dos fases claras:

1.  **Fase de Planificación Estratégica:** Esta es la fase que acabamos de completar. Se realiza en un entorno conversacional de amplio contexto. Un **Orchestrator de IA** asume los roles de un equipo completo de especialistas para colaborar con el stakeholder (tú) y transformar la idea inicial en un plan técnico y de producto completo. El objetivo es tomar todas las decisiones clave antes de escribir código para minimizar la ambigüedad y el retrabajo. El equipo de IA que participó fue:
    * **Analista (Mary):** Para la investigación inicial y la creación del *Project Brief*.
    * **Product Manager (John):** Para la creación del *Product Requirements Document (PRD)* y el desglose en historias de usuario.
    * **Experto en UX (Sally):** Para definir la experiencia de usuario y la especificación visual en la *UI/UX Specification*.
    * **Arquitecto (Winston):** Para diseñar la *Fullstack Architecture* técnica.
    * **Product Owner (Sarah):** Para la validación final y asegurar la coherencia de todos los planes.

2.  **Fase de Desarrollo Táctico:** Esta fase comienza ahora. Se lleva a cabo en un IDE con capacidades de IA. Aquí, agentes de IA especializados en desarrollo (`@dev`) toman los planes detallados que creamos y los ejecutan, escribiendo el código, creando archivos y corriendo pruebas directamente en el entorno de desarrollo.

## 📂 Documentos Fundamentales del Proyecto
Toda la planificación se ha consolidado en los siguientes cuatro documentos, que deberían encontrarse en una carpeta `/docs` de este repositorio:

1.  **`project-brief.md` (El "Porqué"):** Es el punto de partida y la visión del proyecto. Define el problema que se resuelve para nuestro usuario objetivo ("El Ciudadano Curioso"), la solución propuesta, las metas del negocio y el alcance general del Producto Mínimo Viable (MVP).

2.  **`product-requirements-document.md` (El "Qué"):** Es el plan de acción detallado. Traduce la visión en requisitos funcionales y no funcionales concretos. Contiene el backlog completo para el MVP, desglosado en una Épica y 5 historias de usuario con sus respectivos criterios de aceptación.

3.  **`ui-ux-specification.md` (El "Cómo se Siente"):** Es la guía para la experiencia del usuario y la identidad visual. Define el estilo "fintech" moderno que buscamos, la paleta de colores, la tipografía, la arquitectura de la información y las directrices de accesibilidad. Incluye un prompt detallado para generar el código base del frontend con herramientas como Vercel v0.

4.  **`fullstack-architecture.md` (El "Cómo se Construye"):** Es el plano técnico detallado. Define la pila tecnológica (Next.js, NestJS, Vercel, Railway), la infraestructura, el diseño de la base de datos, la especificación de la API, la estrategia de pruebas (incluyendo E2E con Playwright) y los estándares de codificación que el agente de IA debe seguir.

## 🚀 Próximos Pasos: Fase de Desarrollo con IA
La Fase de Desarrollo se llevará a cabo en un **IDE con capacidades de IA, como Windsurf o Claude Code**.

El éxito del desarrollo con IA no depende de "prompts" improvisados, sino de la calidad de los documentos que ya hemos creado. **El PRD y, más específicamente, los "tickets" de cada historia de usuario, son los prompts detallados y explicativos que guiarán al agente de IA.** No es necesario crear nuevos prompts; usaremos la estructura de tareas que ya definimos.

El flujo de trabajo en el IDE será el siguiente:
1.  **Iniciar un Nuevo Chat:** Para cada historia de usuario, se iniciará un nuevo chat limpio en el IDE.
2.  **Invocar al Agente:** Se llamará al agente de desarrollo (ej. `@dev`).
3.  **Proporcionar el Ticket:** Se le pasará el "ticket" completo de la historia (con sus tareas, criterios de aceptación y notas técnicas, tal como lo definimos).
4.  **Ejecución:** El agente de IA ejecutará las tareas, escribiendo el código directamente en los repositorios del proyecto.

Comenzaremos con la **Historia 1.1: Configuración del Backend y API de Datos Manuales**.

## 💻 Pila Tecnológica Principal (Tech Stack)
| Área | Tecnología |
| :--- | :--- |
| Frontend | Next.js (TypeScript) |
| Backend | NestJS (TypeScript) |
| Base de Datos | PostgreSQL |
| Estilos | Tailwind CSS |
| Pruebas E2E | Playwright |
| Infraestructura | Vercel (FE) + Railway (BE) |
