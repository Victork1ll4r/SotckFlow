**UNIVERSIDAD CATÓLICA DE CUENCA (UCACUE)** **CÁTEDRA:** PRÁCTICAS HERRAMIENTAS DE PROGRAMACIÓN

**TEMA:** INFORME DE DISEÑO STITCH Y DESPLIEGUE EN COOLIFY

**CATEDRÁTICO:** ING. JUNIOR WACHAPA

**RESPONSABLE:** VÍCTOR ANDRE AGILA PUA

**PARALELO:** QUINTO “A”

**FECHA DE ENTREGA:** 11-06-2026

**PERÍODO ACADÉMICO:**
MARZO-AGOSTO 2026
   
**CUENCA – ECUADOR**

---

## 1. Diseño de Interfaces (Google Stitch)

**Prompt principal utilizado en STITCH:** > "Genera una Landing Page moderna y un panel administrativo (Dashboard) estilo SaaS para una plataforma de gestión llamada **StockFlow - Control de Almacén y Ventas**. Utiliza una paleta de colores basada en verde esmeralda (#059669) y tonos oscuros elegantes (slate-900). Basate en esta arquitectura y módulos:"

# StockFlow - Control de Almacén y Ventas
## Arquitectura Moderna orientada a Productividad

### Visión General  
Aplicación full-stack separada en frontend React y backend Node.js/Express con comunicación RESTful y autenticación JWT.

```mermaid  
graph TD  
    A[Usuario] --> B(Frontend React/Vite)  
    B -->|HTTPS| C[Backend API Node/Express]  
    C -->|SQL| D[(PostgreSQL)]  
    C -->|Documenta| E[Swagger UI]  
    style B fill:#f9f9f9,stroke:#333,stroke-width:1px  
    style C fill:#f9f9f9,stroke:#333,stroke-width:1px  
    style D fill:#f9f9f9,stroke:#333,stroke-width:1px  
    style E fill:#f9f9f9,stroke:#333,stroke-width:1px

    