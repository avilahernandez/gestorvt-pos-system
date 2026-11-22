# 📱 gestorVT - Sistema POS y Gestión de Inventario Offline-First

![Banner de gestorVT](banner.jpg)

**gestorVT** es una solución completa de Punto de Venta (POS) y gestión de inventarios diseñada para operar en entornos con conectividad inestable. Construida con una arquitectura **Offline-First**, garantiza que tu negocio nunca se detenga.

## 🚀 Características Principales

*   **Punto de Venta (POS) Rápido y Seguro:** Interfaz optimizada para agilizar las ventas diarias con cálculo de cambio automático y búsqueda rápida de productos.
*   **Gestión Total de Inventario:** Control de stock en tiempo real, alertas de stock bajo, nomenclador de productos y registro de compras.
*   **Control de Usuarios y Roles:** Sistema de permisos diferenciado (Administradores, Cajeros) con auditoría de acciones.
*   **Trazabilidad y Auditoría:** Registro detallado de todas las actividades (log de actividades, compras, ventas, devoluciones).
*   **Modo Offline:** Funciona sin conexión a internet, guardando los datos localmente para su posterior sincronización.
*   **Sistema de Licenciamiento:** Protección del software mediante certificación criptográfica (SHA-256) y bloqueo por hardware.

## 🛠️ Stack Tecnológico y Arquitectura

Este proyecto fue desarrollado aplicando buenas prácticas de ingeniería de software para garantizar escalabilidad, seguridad y rendimiento.

*   **Frontend (UI/UX):** Android (Java Nativo) + Vistas Híbridas (WebView con HTML5, CSS3 y JavaScript moderno).
*   **Base de Datos Local:** SQLite implementando el **Patrón DAO (Data Access Object)** para una separación limpia de la lógica de negocio y el acceso a datos.
*   **Backend (Sincronización):** PHP, MariaDB, Nginx.
*   **Seguridad:** Criptografía SHA-256 y sistema de bloqueo por hardware.

## 📸 Capturas de Pantalla (Módulos Principales)

| Login y Bienvenida | Panel de Administración | Punto de Venta (POS) |
| :---: | :---: | :---: |
| ![Login](login.jpg) | ![Admin](admin.jpg) | ![Ventas](pos.jpg) |

| Gestión de Productos | Trazas (Log de Actividades) | Gestión de Usuarios |
| :---: | :---: | :---: |
| ![Productos](productos.jpg) | ![Trazas](trazas.jpg) | ![Usuarios](usuarios.jpg) |

## 🧾 Flujo de Venta y Caja

| Ticket de Venta | Ventas del Día | Control de Caja | Devoluciones |
| :---: | :---: | :---: | :---: |
| ![Ticket](ticket.jpg) | ![Ventas Día](ventas_dia.jpg) | ![Caja](control_caja.jpg) | ![Devoluciones](devoluciones.jpg) |

## 🏗️ Arquitectura del Proyecto

Desarrollado utilizando **CodeAssist** (un potente IDE de Android). El proyecto sigue una arquitectura limpia, separando la lógica de negocio, el acceso a datos y la interfaz de usuario. 

### 📂 Estructura de Paquetes (Patrón DAO)
La base de datos SQLite está gestionada mediante el patrón **DAO (Data Access Object)**, asegurando que el código sea escalable y fácil de mantener.

![Estructura Java DAO](estructura_java.jpg)

### 💻 Interfaz Híbrida (WebView)
La UI está construida con HTML, CSS y JavaScript, manteniendo una separación modular para cada módulo del sistema (Ventas, Compras, Inventario, etc.).

| Estructura HTML | Estructura JavaScript | Estructura CSS |
| :---: | :---: | :---: |
| ![HTML](estructura_html.jpg) | ![JS](estructura_js.jpg) | ![CSS](estructura_css.jpg) |

## 💡 El Reto Técnico
El principal desafío de este proyecto fue diseñar una arquitectura de base de datos que permitiera la sincronización bidireccional sin conflictos entre múltiples dispositivos (cajeros) que operan de forma local, asegurando la integridad de los datos y la lógica de negocio (como las devoluciones FIFO y el doble stock).

---
*Nota: El código fuente de la lógica de negocio y seguridad es privado. Estas capturas son una muestra de la organización y arquitectura del sistema.*

**Desarrollado por Raúl Ávila Hernández** | [LinkedIn](https://www.linkedin.com/in/raul-avila-h-dev)
