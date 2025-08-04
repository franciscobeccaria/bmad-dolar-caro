# Product Requirements Document (PRD): Dólar Real

## Metas y Contexto de Fondo

#### **Metas**
* Proveer una respuesta clara y visual a la pregunta "¿Está caro el dólar en Argentina?".
* Traducir cotizaciones financieras abstractas en poder de compra tangible usando productos comunes.
* Validar el interés del público en una herramienta de economía cotidiana simple y educativa.
* Lanzar un MVP funcional en 1 semana para capturar el interés inicial y obtener feedback temprano.

#### **Contexto de Fondo**
En el volátil entorno económico de Argentina, los ciudadanos enfrentan una constante incertidumbre sobre el valor real de su moneda. Este proyecto nace para resolver ese problema, ofreciendo una aplicación web simple que ancla el valor del dólar a bienes tangibles y conocidos.

#### **Registro de Cambios**
| Fecha | Versión | Descripción | Autor |
| :--- | :--- | :--- | :--- |
| 2025-07-26 | 1.0 | Creación inicial del documento a partir del Project Brief. | John (PM) |

## Requisitos

#### **Requisitos Funcionales (FR)**
1.  **FR1:** La aplicación debe mostrar una respuesta principal y directa (ej. "Sí" o "No") a la pregunta "¿Está caro el dólar en Argentina?".
2.  **FR2:** La aplicación debe mostrar una lista de al menos 4 productos de comparación predefinidos (Big Mac, Nike Air Force One, iPhone, Camiseta Adidas).
3.  **FR3:** Para cada producto, se debe mostrar la comparación de precios entre Argentina y al menos un país de referencia (EE.UU.).
4.  **FR4:** El sistema debe mostrar los precios a partir de una fuente de datos cargada manually para el MVP. La automatización (scraping) se desarrollará en una fase posterior.

#### **Requisitos No Funcionales (NFR)**
1.  **NFR1:** La aplicación web debe ser responsiva, funcionando correctamente en navegadores de escritorio y móviles con la misma importancia.
2.  **NFR2:** La página principal debe tener un tiempo de carga inicial inferior a 3 segundos en una conexión promedio.
3.  **NFR3:** La arquitectura debe priorizar el uso de servicios con capas gratuitas para minimizar los costos operativos del MVP.

## Objetivos de Diseño de la Interfaz de Usuario (UI/UX)

* **Visión de UX:** Máxima simplicidad y claridad, con una interfaz limpia, moderna y visual.
* **Respuesta Principal:** Se utilizará un diseño "Minimalista Directo": un gran "SÍ/NO" con colores y el porcentaje.
* **Branding y Accesibilidad:** Estilo minimalista, colores intencionados (verde/rojo) y conformidad con WCAG AA.

## Supuestos Técnicos

* **Estructura de Repositorio:** Polyrepo (dos repositorios separados).
* **Arquitectura de Servicios:** Backend como Monolito Modular con NestJS.
* **Requisitos de Pruebas:** Pruebas unitarias y de integración.

## Épica y Historias de Usuario

#### **Épica 1: MVP - Lanzamiento de la Herramienta de Comparación de Precios**
* **Objetivo:** Establecer la infraestructura, implementar la página de comparación con datos manuales para 4 productos y lanzarla a producción en una semana.

#### **Historias de Usuario**
* **1.1: Configuración del Backend y API de Datos Manuales:** Crear la base del proyecto NestJS y un endpoint que sirva datos desde un archivo JSON.
* **1.2: Configuración del Frontend y Conexión a la API:** Crear la base del proyecto Next.js y verificar la conexión con el backend.
* **1.3: Implementación de la Interfaz de Usuario Principal:** Construir la UI responsiva, que consuma los datos y realice el cálculo de la respuesta principal.
* **1.4: Despliegue del MVP a Producción:** Desplegar ambos servicios en plataformas públicas.
* **1.5: Revisión y Carga del Contenido Final:** Asegurar que todos los textos sean claros y sin errores.

## Informe de Resultados del Checklist
* **Decisión Final: LISTO PARA EL ARQUITECTO.** El PRD es robusto, claro y completo para las necesidades del MVP.

## Próximos Pasos
* **Prompt para el Experto UX:** "Basado en este PRD, por favor, crea la especificación de UI/UX (`front-end-spec`)."
* **Prompt para el Arquitecto:** "Utiliza este PRD y la futura especificación de UI/UX para diseñar la arquitectura técnica full-stack."