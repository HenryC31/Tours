# Plataforma de Tours

Una plataforma moderna de grado empresarial para la gestión, venta y reserva de tours de aventura (RZRs, ATVs, Camellos, Bicicletas). Diseñada para escalar y ofrecer una experiencia de usuario de alta conversión y rendimiento competitivo en el mercado turístico.

## Tecnologías Principales

Este proyecto está construido con el *Modern Web Stack* para garantizar seguridad, velocidad y un excelente posicionamiento SEO:

*   **Frontend & Full-stack Framework:** [Next.js (App Router)](https://nextjs.org/)
*   **Lenguaje:** [TypeScript](https://www.typescriptlang.org/)
*   **Estilos y UI:** [Tailwind CSS](https://tailwindcss.com/)
*   **Base de Datos & Backend-as-a-Service:** [Supabase](https://supabase.com/) (PostgreSQL)

## Características Destacadas (En Desarrollo)

*   **Catálogo Dinámico:** Visualización rápida de tours y disponibilidad.
*   **Gestión de Inventario:** Control estricto de disponibilidad de vehículos por fecha y hora.
*   **Seguridad RLS:** Políticas de seguridad a nivel de fila (Row Level Security) directamente en la base de datos de PostgreSQL.
*   **Sistema de Reservas:** Flujo de pago y confirmación intuitivo para el turista.

## Configuración para Desarrollo Local

Sigue estos pasos para levantar el entorno de desarrollo en tu máquina local:

### 1. Clonar el repositorio
git clone [https://github.com/HenryC31/Tours.git](https://github.com/HenryC31/Tours.git)
```
cd Tours
```
### 2. Instalar dependencias
```
npm install
```
### 3. Configurar variables de entorno
Crea un archivo .env.local en la raíz del proyecto y agrega tus credenciales de Supabase (pide acceso al administrador si no las tienes):

```
NEXT_PUBLIC_SUPABASE_URL=tu_url_de_supabase
NEXT_PUBLIC_SUPABASE_ANON_KEY=tu_anon_key
SUPABASE_SERVICE_ROLE_KEY=tu_service_role_key
```

### 4. Iniciar el servidor de desarrollo
```
npm run dev
```
Abre http://localhost:3000 en tu navegador para ver la aplicación en funcionamiento.

## 🛡️ Arquitectura y Buenas Prácticas
Tipado Estricto: Se utiliza TypeScript en todo el proyecto para evitar errores en tiempo de ejecución y asegurar la integridad de los datos en las reservas.

Seguridad de Datos: Las llaves secretas y la lógica de validación crítica residen exclusivamente del lado del servidor.
