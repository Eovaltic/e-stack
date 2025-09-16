# E-Stack

**La base sólida y modular para tus proyectos frontend.**  
**The solid and modular foundation for your frontend projects.**

---

## 📌 Descripción / Description

**ES:**  
E-Stack es un sistema modular de CSS basado en la metodología SMACSS (Scalable and Modular Architecture for CSS) creado por **EOVALTIC – Edwing Ovalle**.  
Su objetivo es ofrecer una arquitectura escalable, mantenible y profesional para proyectos frontend.  
Cada módulo puede instalarse y usarse de forma independiente (por ejemplo: resets, layouts, utilidades), lo que permite a los desarrolladores tener control total sobre el diseño y la evolución de sus aplicaciones.

**EN:**  
E-Stack is a modular CSS system based on the SMACSS methodology (Scalable and Modular Architecture for CSS) created by **EOVALTIC – Edwing Ovalle**.  
Its goal is to provide a scalable, maintainable, and professional architecture for frontend projects.  
Each module can be installed and used independently (e.g., resets, layouts, utilities), allowing developers to have full control over design and the evolution of their applications.

---

## 🔧 Módulos de E-Stack / E-Stack Modules

E-Stack está compuesto por los siguientes módulos:

E-Stack is composed of the following modules:

* **E-Reseter**: Resetea estilos por defecto (CSS reset / normalize) para uniformidad. Opcional si ya existe un reset propio. / Resets default styles (CSS reset / normalize) for uniformity. Optional if a custom reset already exists.
* **E-Initializer**: Inicializa la app, carga configuraciones globales y dependencias. Siempre ejecutarse primero. / Initializes the app, loads global configurations and dependencies. Should always run first.
* **E-Layouter**: Gestiona la disposición general: grids, columnas y contenedores. / Manages general layout: grids, columns, and containers.
* **E-Renderer**: Renderiza componentes individuales y reutilizables. Depende de E-Layouter. / Renders individual and reusable components. Depends on E-Layouter.
* **E-Statekeeper**: Controla estados temporales de módulos o componentes (activo, cargando, error…). / Controls temporary states of modules or components (active, loading, error…).
* **E-Themer**: Aplica estilos, colores y temas según la configuración de la app. / Applies styles, colors, and themes according to the app configuration.
* **E-Handler**: Gestiona eventos e inputs del usuario, enlazando acciones con respuestas. / Manages user events and inputs, linking actions with responses.
* **E-Storer**: Maneja datos locales y remotos (APIs, bases de datos, cache). / Manages local and remote data (APIs, databases, cache).
* **E-Connector**: Gestiona conexiones con servidores, APIs externas y websockets. Interactúa con E-Storer. / Manages connections with servers, external APIs, and websockets. Interacts with E-Storer.
* **E-Authenticator**: Controla autenticación, roles, permisos y seguridad general. / Controls authentication, roles, permissions, and general security.
* **E-Notifier**: Envía notificaciones, alertas y mensajes al usuario. / Sends notifications, alerts, and messages to the user.

*Nota / Note:* Cada módulo puede ser reemplazado o omitido si el usuario ya tiene su propia implementación.

Each module can be replaced or omitted if the user already has their own implementation.

## 🔄 Flujo de Inicialización Recomendado / Recommended Initialization Flow

1. **E-Reseter** (opcional / optional)
2. **E-Initializer**
3. **E-Layouter → E-Renderer → E-Statekeeper → E-Themer → E-Handler**
4. **E-Storer → E-Connector → E-Authenticator → E-Notifier**

---

## 📦 Módulos actuales / Current Modules


---

## 🚀 Instalación / Installation

```bash
npm install @eovaltic/e-reset
```

**Uso en HTML:**

```html
<link rel="stylesheet" href="./node_modules/@eovaltic/e-reset/_reset.css">
```

**Uso en CSS/SCSS:**

```css
@import "@eovaltic/e-reset/_reset.css";
```

---

## 👤 Autor / Author

**EOVALTIC – Edwing Ovalle**

---

## 📄 Licencia / License

MIT License © 2025 EOVALTIC – Edwing Ovalle

---
🔑 Conexión SSH verificada el 16-sept-2025.

