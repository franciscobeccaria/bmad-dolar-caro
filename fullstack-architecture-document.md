# Fullstack Architecture Document: Dólar Real

## Introducción
Este documento describe la arquitectura full-stack completa para el proyecto. Se ha decidido diseñar la arquitectura desde cero. El código generado por IA (Vercel v0) se usará como referencia visual pero no dictará la estructura.

## Arquitectura de Alto Nivel
* **Resumen Técnico:** La arquitectura se basa en un enfoque de **Polyrepo** con dos servicios desacoplados: un frontend Next.js y un backend NestJS. El frontend se desplegará en Vercel y el backend en Railway.
* **Plataforma e Infraestructura:**
    * **Plataforma:** Vercel (Frontend) y Railway (Backend, Base de Datos).
    * **Justificación:** Combinación extremadamente rápida para desarrollar y desplegar, con generosas capas gratuitas ideales para el MVP.
* **Diagrama de Arquitectura:**
    ```mermaid
    graph TD
        subgraph Internet
            U[Usuario]
        end

        subgraph Vercel
            FE[Frontend App<br>(Next.js)]
        end

        subgraph Railway
            BE[Backend API<br>(NestJS)]
            DB[(Base de Datos<br>PostgreSQL)]
        end

        U -->|Navegador| FE
        FE -->|Llamada API (HTTPS)| BE
        BE <-->|Consultas DB| DB
    ```

## Pila Tecnológica y Datos
#### **Pila Tecnológica (Tech Stack)**
| Categoría | Tecnología | Versión | Propósito |
| :--- | :--- | :--- | :--- |
| Framework Frontend | Next.js | 14+ | SSR y rendimiento óptimo. |
| Framework Backend | NestJS | 10+ | API robusta y estructurada. |
| Lenguaje | TypeScript | 5+ | Seguridad de tipos en todo el proyecto. |
| Base de Datos | PostgreSQL | 16 | Base de datos relacional, soportada por Railway. |
| Estilos | Tailwind CSS | 3+ | Estilado rápido y moderno. |
| Pruebas Unit/Int | Jest | 29+ | Pruebas unitarias y de integración. |
| Pruebas E2E | Playwright | 1.40+ | Pruebas End-to-End en navegador real. |

#### **Esquema de Base de Datos**
```sql
CREATE TABLE products (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    name VARCHAR(255) NOT NULL,
    image_url TEXT,
    price_ar DECIMAL(10, 2) NOT NULL,
    price_us DECIMAL(10, 2) NOT NULL,
    last_updated TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP
);