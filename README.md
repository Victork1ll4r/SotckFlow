# Herramientas-Node-Api - Control de Almacén y Ventas

Plataforma integral para la administración de stock, control de clientes y registro de ventas. Desarrollada utilizando React.js para el cliente y Node.js con Express y PostgreSQL para la lógica del servidor.

## 📌 Requerimientos del Sistema

Antes de iniciar, verifica que cuentas con:
- [Node.js](https://nodejs.org/) (v18+)
- [PostgreSQL](https://www.postgresql.org/) (Motor de base de datos)
- Opcional: [Docker y Docker Compose](https://www.docker.com/) para despliegue rápido en contenedores.

---

## ⚙️ Variables de Entorno

Es necesario definir los parámetros de conexión antes de ejecutar el aplicativo.

### Entorno del Servidor (API)
1. Navega al directorio de la API: `cd stockflow-api` (o el nombre de tu carpeta backend).
2. Duplica el archivo de muestra:
   - Windows: `copy .env.example .env`
   - Linux/Mac: `cp .env.example .env`
3. Edita el `.env` para establecer tu propia firma en `JWT_SECRET` y configurar las credenciales de PostgreSQL.

### Entorno del Cliente (Web)
1. Accede al directorio del cliente: `cd stockflow-client` (o tu carpeta frontend).
2. Duplica el archivo de configuración:
   - Windows: `copy .env.example .env`
   - Linux/Mac: `cp .env.example .env`
3. Valida que la variable `VITE_API_URL` apunte correctamente al puerto de tu API (ej. `http://localhost:3000/api`).

---

## 🚀 Despliegue con Docker Compose (Recomendado)

Levanta la infraestructura completa (BD, Servidor y Cliente vía Nginx) con un solo comando.

1. Ubícate en la raíz donde reside el archivo `docker-compose.yml`.
2. Asegúrate de tener exportadas las variables `DB_PASSWORD` y `JWT_SECRET` en tu terminal o en un `.env` global.
3. Inicia los contenedores:
   ```bash
   docker-compose up --build -d