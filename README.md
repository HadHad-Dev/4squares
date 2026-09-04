# 🍔 QuickOrder POS & ERP System

> **Sistema Web Integral de Gestión, Control de Inventario y Analítica para Restaurantes de Comida Rápida**

---

## 📋 Descripción del Proyecto

**QuickOrder POS & ERP** es una plataforma web desarrollada para optimizar la operativa diaria, el control de inventarios y la toma de decisiones estratégicas en restaurantes de comida rápida.

El sistema implementa un esquema de **Control de Acceso Basado en Roles (RBAC)** de 3 jerarquías (Gerente General, Supervisor de Turno y Cajero). Incluye un motor analítico que procesa un DataFrame sintético para la **recomendación inteligente de reabastecimiento** a proveedores y un módulo de **proyecciones vs. ventas reales**.

---

## 🖼️ Vistas Principales del Sistema

### 📊 Dashboard Analítico (Gerente & Supervisor)
![Dashboard Analítico](https://raw.githubusercontent.com/placeholder-user/quickorder-assets/main/dashboard-analytics.png)
*Panel interactivo con comparativas de ventas (Real vs. Proyectado), ticket promedio, top de productos más vendidos e histórico diario, semanal y mensual.*

---

### 🛒 Terminal Punto de Venta (POS Cajero)
![Interfaz POS Cajero](https://raw.githubusercontent.com/placeholder-user/quickorder-assets/main/pos-cashier.png)
*Interfaz limpia y rápida para la captura de comandas en caja y envío directo a cocina.*

---

## ✨ Jerarquías y Funcionalidades

### 👑 1. Gerente General / Dueño
- **Analítica Global & Cierres:** Métricas históricas (diarias, semanales, mensuales) de ventas totales, ticket promedio y productos más vendidos.
- **Módulo de Proyecciones:** Comparativa interactiva entre **Ventas Reales vs. Ventas Proyectadas** (diarias y mensuales) con indicadores de cumplimiento (KPIs).
- **Gestión Estratégica de Compras:** Acceso al motor de reabastecimiento para órdenes de compra consolidadas de alto volumen y control de presupuestos.

### 📋 2. Supervisor de Turno
- **Corte del Día:** Arqueo de caja, desglose por métodos de pago (Efectivo, Tarjeta, Apps) y validación de descuadres.
- **Reabastecimiento Directo (DataFrame):** Tabla recomendada por el algoritmo para compras directas según punto de reorden y consumo proyectado.
- **Alertas de Inventario:** Monitor de stock crítico y registro de mermas/productos caducados.

### 🛒 3. Cajero / Personal de Atención
- **POS Táctil:** Interfaz ágil para tomar pedidos y enviar a cocina.
- **Arqueo Ciego:** Registro de efectivo al cierre de turno para entrega al supervisor.

---

## 🛠️ Stack Tecnológico

| Capa | Tecnología | Descripción |
| :--- | :--- | :--- |
| **Frontend** | TypeScript + React | Interfaz dinámica, fuertemente tipada y responsiva. |
| **Estilos** | Tailwind CSS | Diseño agilizado y estilizado de dashboards. |
| **Gráficos** | Chart.js / Recharts | Visualización interactiva de ventas, proyecciones e históricos. |
| **Backend** | Python + FastAPI | API RESTful asíncrona de alto rendimiento. |
| **Analítica** | Pandas / NumPy | Procesamiento del DataFrame sintético para reabastecimiento y proyecciones. |
| **Base de Datos** | PostgreSQL | Base de datos relacional para ventas, inventarios y usuarios. |
| **ORM & Migraciones**| SQLAlchemy + Alembic | Control de versiones de la base de datos y mapeo objeto-relacional. |
| **Seguridad** | JWT (JSON Web Tokens) | Autenticación y autorización por jerarquías de rol. |
