# 🌱 Proyecto E-commerce Ecológico

## 📌 Descripción General

Este proyecto es una **plataforma de comercio electrónico sostenible**, diseñada para promover productos reciclados y ecológicos de manera accesible y moderna. La solución combina un **backend robusto basado en microservicios** con un **frontend optimizado para la experiencia de usuario**, logrando un sistema escalable, seguro y fácil de usar.

El objetivo principal es brindar a los usuarios una experiencia de compra digital intuitiva, a la vez que se fomenta el consumo responsable y sostenible.

## 🏗️ Arquitectura del Sistema

El sistema implementa una **arquitectura de microservicios distribuidos** que proporciona:

* **Escalabilidad horizontal** - Cada servicio puede escalar independientemente
* **Aislamiento de fallos** - La falla de un servicio no afecta al sistema completo
* **Despliegue independiente** - Actualizaciones sin interrumpir otros servicios
* **Diversidad tecnológica** - Cada servicio puede usar diferentes tecnologías

## 📸 Galería de Interfaces  

La siguiente galería muestra las principales pantallas del sistema, organizadas en pares para una mejor visualización.  

---

| 🏠 Pantalla Principal | 🛍️ Catálogo de Productos |
|-----------------------|--------------------------|
| ![Pantalla principal](https://github.com/user-attachments/assets/334f2174-5b6c-4acd-8436-9b16a18ed027) | ![Productos](https://github.com/user-attachments/assets/32382cae-00ae-4a14-88d3-6ffb744ff857) |

| 🛒 Carrito de Compras | 🔑 Inicio de Sesión (Login) |
|-----------------------|----------------------------|
| ![Carrito](https://github.com/user-attachments/assets/b47ad1a4-6620-4055-ab19-ecc806c1c601) | ![Login](https://github.com/user-attachments/assets/e2c1d1ae-9f04-4098-8c59-71ef1e397f39) |

| 📊 Dashboard del Usuario | ⚙️ Administración de Productos |
|---------------------------|-------------------------------|
| ![Dashboard](https://github.com/user-attachments/assets/93d8ea41-f9f1-4253-9937-a3c68e8db7d2) | ![Admin productos](https://github.com/user-attachments/assets/e7a92d23-03a4-4f02-847d-9a9d0ed3b60e) |

| 💬 Chat en Tiempo Real | 📅 Módulo de Eventos |
|-------------------------|----------------------|
| ![Chat](https://github.com/user-attachments/assets/c88b1f3a-df4a-4829-83ac-7656c597ad0c) | ![Eventos](https://github.com/user-attachments/assets/2ec99aab-fcf4-4ad3-807a-4fe9ec25b070) |

---

> 💡 **Tip:** Haz clic en cualquier imagen para verla en tamaño completo.  


### Componentes Backend

* **api-gateway** → Punto de entrada único para clientes y enrutamiento de peticiones
* **auth-service** → Autenticación y autorización de usuarios con JWT
* **chat-service** → Comunicación en tiempo real entre usuarios usando WebSocket
* **client-service** → Gestión de información y perfiles de clientes
* **content-service** → Manejo de recursos multimedia, textos e imágenes
* **order-pay-service** → Procesamiento de órdenes y gestión de pagos
* **product-service** → Administración del catálogo de productos ecológicos
* **report-service** → Generación de estadísticas y reportes de ventas
* **eureka-server** → Registro y descubrimiento de microservicios
* **config-server** → Configuración centralizada y gestión de propiedades
* **orchestrator-service** → Coordinación de interacciones complejas entre servicios

## 🔧 Patrones de Diseño Implementados

### Patrones Arquitectónicos
* **API Gateway Pattern** - Punto único de acceso para todos los clientes
* **Service Registry Pattern** - Descubrimiento automático de servicios con Eureka
* **Configuration Server Pattern** - Configuración centralizada y externalizada
* **Orchestration Pattern** - Coordinación de procesos de negocio complejos

### Patrones de Comunicación
* **Request-Response Pattern** - Comunicación síncrona HTTP/REST
* **Publisher-Subscriber Pattern** - Comunicación asíncrona para eventos
* **WebSocket Pattern** - Comunicación bidireccional en tiempo real para chat

### Patrones de Datos
* **Shared Database** - Base de datos MySQL compartida para consistencia transaccional

## 💡 Conceptos Clave Utilizados

### Backend Concepts
* **Microservicios** - Arquitectura distribuida con servicios independientes
* **Service Discovery** - Localización automática de servicios disponibles
* **Load Balancing** - Distribución de carga entre instancias de servicios
* **Circuit Breaker** - Protección ante fallos en cascada
* **JWT Authentication** - Autenticación stateless con tokens seguros
* **RESTful APIs** - Interfaces uniformes basadas en REST
* **WebSocket Communication** - Comunicación bidireccional en tiempo real

### Frontend Concepts
* **Server Side Rendering (SSR)** - Renderizado del lado del servidor con Next.js
* **Component-Based Architecture** - Arquitectura basada en componentes reutilizables
* **Responsive Design** - Diseño adaptativo para todos los dispositivos
* **Progressive Web App (PWA)** - Experiencia de aplicación nativa en web
* **API Integration** - Consumo de APIs REST con Axios

## 🚀 Tecnologías Utilizadas

### Backend
* **Java** - Lenguaje de programación principal
* **Spring Boot** - Framework para desarrollo de aplicaciones Java
* **Spring Cloud** - Herramientas para sistemas distribuidos
* **Maven** - Gestión de dependencias y construcción de proyectos
* **MySQL** - Base de datos relacional principal
* **WebSocket** - Comunicación en tiempo real para chat
* **JWT** - JSON Web Tokens para autenticación
* **Docker** - Contenorización de servicios

### Frontend
* **Next.js** - Framework React con SSR/SSG
* **React** - Biblioteca para interfaces de usuario
* **Tailwind CSS** - Framework CSS utility-first para estilos
* **Axios** - Cliente HTTP para consumo de APIs
* **JavaScript** - Lenguaje de programación del frontend
* **WebSocket Client** - Cliente para comunicación en tiempo real
* **React Hooks** - Gestión de estado y efectos
* **Responsive Design** - Adaptabilidad a diferentes dispositivos

## 📡 Endpoints Principales

* **API Gateway** → `http://localhost:8080/` - Punto de entrada principal
* **Eureka Server** → `http://localhost:8761/` - Consola de descubrimiento de servicios
* **Config Server** → `http://localhost:8888/` - Servidor de configuración
* **WebSocket Endpoint** → `ws://localhost:8080/chat` - Comunicación en tiempo real

## ✨ Funcionalidades Clave

### Funcionalidades de Usuario
* Catálogo de productos ecológicos con filtros avanzados
* Carrito de compras dinámico en tiempo real
* Proceso de compra seguro en múltiples pasos (checkout)
* Registro e inicio de sesión con autenticación JWT
* Sistema de reseñas y calificación de productos
* Chat en vivo para soporte al cliente con WebSocket
* Notificaciones automáticas por correo electrónico
* Sistema de fidelización con puntos ecológicos

### Funcionalidades Administrativas
* Panel administrativo completo para gestión
* Administración de productos, pedidos y usuarios
* Generación de reportes y estadísticas de ventas
* Gestión de contenido multimedia
* Sistema de configuración centralizada

### Funcionalidades de Contenido
* Blog con noticias sobre sostenibilidad
* Gestión de recursos multimedia optimizados
* Sistema de contenido dinámico y actualizable

## ✅ Requerimientos No Funcionales

* **Performance** - Tiempo de respuesta < 200ms y soporte para 1000+ usuarios concurrentes
* **Seguridad** - Autenticación JWT, cifrado de datos y validación de entrada
* **Escalabilidad** - Escalado horizontal automático y balanceeo de carga
* **Disponibilidad** - Uptime del 99.9% con recuperación automática ante fallos
* **Usabilidad** - Diseño responsivo, accesible y compatible con todos los navegadores
