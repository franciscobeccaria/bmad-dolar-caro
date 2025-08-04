# UI/UX Specification: Dólar Real

## Dirección Visual y Estilo
* **Estilo:** "Fintech" moderno, limpio, minimalista, con mucho espacio en blanco, tipografías sans-serif y datos presentados en "tarjetas".
* **Paleta de Colores:** Basada en blancos/grises, con azul de acento y rojo/verde para indicadores.
* **Tipografía:** "Inter" (o similar de Google Fonts).

## Arquitectura de la Información
* **Mapa del Sitio:** Una única página principal que contiene la respuesta, la lista de productos y los gráficos. El detalle del producto se abre en un Modal.

    ```mermaid
    graph TD
        A[Página Principal] --> B(Respuesta Principal - Sí/No);
        A --> C(Lista de Productos);
        A --> D(Sección de Gráficos de Contexto);
        C -- Clic en Producto --> E[Modal con Detalle del Producto];
    ```

## Flujos de Usuario
* **Flujo Principal:** El usuario llega a la página, entiende la respuesta principal en segundos, escanea la evidencia en la lista de productos y se va informado. Se han considerado los casos de error (ej. API no responde).

## Wireframe Textual y Componentes
* **Estructura de Página:**
    1.  Encabezado (Título principal).
    2.  Componente de Respuesta Principal.
    3.  Sección de Comparación de Productos (lista/grilla de tarjetas).
    4.  Sección de Gráficos (placeholder).
    5.  Pie de página.
* **Librería de Componentes:** Se recomienda usar una librería existente como **Shadcn/ui** para acelerar el desarrollo.
* **Componentes Clave:** Card (Tarjeta), Button (Botón), Badge (Etiqueta).

## Accesibilidad y Diseño Responsivo
* **Accesibilidad:** Objetivo de conformidad con WCAG 2.1 Nivel AA. El color no será el único medio para transmitir información.
* **Diseño Responsivo:** Se definió una estrategia con breakpoints estándar. El layout será de una columna en móvil y se transformará a una grilla de 2x2 en escritorio.

## Animación y Rendimiento
* **Animación:** Solo transiciones suaves y estándar para no añadir complejidad al MVP.
* **Rendimiento:** El objetivo es un tiempo de carga < 3 segundos, como se define en el PRD.

## Próximos Pasos
1.  Finalizar y aprobar esta especificación.
2.  Entregar este documento al Arquitecto como input clave para el diseño técnico.