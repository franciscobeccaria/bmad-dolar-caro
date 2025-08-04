# Project Brief: Dólar Real

## Resumen Ejecutivo
Se propone una aplicación web que traduce la cotización del dólar en valor real de compra, comparando precios de productos y servicios idénticos entre Argentina y otros países. El proyecto aborda la dificultad de la gente común para comprender el verdadero poder adquisitivo del peso argentino y el valor real del dólar, más allá de los volátiles tipos de cambio financieros. La herramienta está dirigida a cualquier persona en Argentina o en la región interesada en entender la economía cotidiana y el valor comparativo de su moneda. Su valor principal es ofrecer una herramienta educativa, visual y accesible que desmitifica el concepto de "dólar caro o barato", presentándolo en términos tangibles como el costo de un Big Mac o un iPhone.

## Declaración del Problema
Actualmente, la percepción del valor del dólar en Argentina es confusa y está dominada por la jerga financiera. Los ciudadanos comunes se enfrentan a múltiples cotizaciones que no reflejan directamente el poder de compra. El principal punto de dolor es la incapacidad de saber si los precios de los bienes y servicios locales son "caros" o "baratos" en un contexto internacional, lo que genera incertidumbre en las decisiones de consumo y ahorro. Las soluciones existentes, como los conversores de divisas tradicionales, son insuficientes porque solo traducen una cotización financiera. En un contexto de alta inflación y volatilidad cambiaria, tener una herramienta que ancle el valor de la moneda a bienes tangibles es más importante que nunca.

## Solución Propuesta
La solución es una aplicación web de una sola página, simple y directa, que responde a la pregunta "¿Está caro el dólar en Argentina?". El enfoque principal es utilizar un "Índice de Precios Reales" basado en la comparación de productos idénticos. A diferencia de los conversores de divisas, esta herramienta no se basa en cotizaciones abstractas, sino en el poder de compra tangible. Su éxito radicará en su simplicidad y enfoque. La visión a largo plazo es convertir el sitio en la principal referencia para entender el poder adquisitivo real en Latinoamérica.

## Usuarios Objetivo
* **Segmento Principal: "El Ciudadano Curioso"**
    * **Perfil:** Personas de 18 a 65 años en Argentina, con interés básico en la economía, no expertos.
    * **Comportamientos:** Consumen noticias económicas generales y usan Google para buscar cotizaciones.
    * **Necesidades:** Buscan claridad y una referencia tangible para entender el valor de su dinero.
    * **Metas:** Obtener una respuesta rápida para tomar mejores decisiones de consumo y ahorro.

## Objetivos y Métricas de Éxito
* **Objetivos de Negocio:** Validar la idea, lanzar un MVP funcional en 1 semana, y establecer el sitio como una fuente de referencia.
* **Métricas de Éxito del Usuario:** El usuario entiende la respuesta principal en <10 segundos, interactúa con los datos y comparte el contenido.
* **KPIs:** 1,000 usuarios únicos/semana, Tasa de Rebote <60%, Tiempo en Página >90 segundos.

## Alcance del MVP
* **Funcionalidades Indispensables:** Página única, respuesta principal "Sí/No", comparador de 4 productos iniciales, recolección de datos por scraping.
* **Fuera de Alcance:** Comparaciones históricas detalladas, aportes de usuarios, comparación de múltiples países, gráficos de contexto económico.

## Visión Post-MVP
* **Fase 2:** Añadir comparaciones históricas, más países y más productos/servicios.
* **Largo Plazo:** Convertirse en el "Índice de Poder Adquisitivo" de referencia para Latinoamérica, con una API pública.
* **Oportunidades:** Contenido editorial, herramienta para viajeros, comunidad de datos.

## Consideraciones Técnicas
* **Plataforma:** Aplicación Web Responsiva.
* **Tecnología:** Frontend con Next.js/Astro.js, Backend con NestJS.
* **Arquitectura:** Polyrepo (dos repositorios separados), API REST o tRPC.

## Restricciones y Supuestos
* **Restricciones:** Costo mínimo (capas gratuitas), plazo de 1 semana, equipo pequeño, alcance limitado a 4 productos.
* **Supuestos Clave:** Disponibilidad pública de datos, viabilidad del web scraping, similitud de productos entre países.

## Riesgos y Preguntas Abiertas
* **Riesgos:** Bloqueo de scraping, cambios en sitios web de origen, falta de interés del usuario.
* **Preguntas Abiertas:** Frecuencia de actualización de precios, manejo de impuestos en las comparaciones.

## Próximos Pasos
1.  Aprobar este Project Brief.
2.  Entregarlo al Product Manager para crear el PRD.
3.  El Arquitecto debe iniciar la investigación de técnicas de scraping.