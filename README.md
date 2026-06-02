# 🎓 Exposición de Prácticas Duales: LD Quantum
### Grado Superior en Desarrollo de Aplicaciones Multiplataforma (DAM) — CPIFP Alan Turing (Málaga)

Este repositorio contiene la documentación, guiones y recursos correspondientes a la presentación del proyecto de prácticas duales de segundo año en **LD Quantum**, una startup tecnológica dedicada a la digitalización y revolución del sector turístico tradicional.

---

## 🎥 Enlaces a los Vídeos de Exposición
De acuerdo con las directrices de la rúbrica, cada participante cuenta con su enlace individual al vídeo de su exposición, el cual incluye la **Parte Común (Contexto de la Empresa)** y la **Parte Individual (Contribuciones Técnicas)**.

* 🔴 **Vídeo de Mario García Luque:** [Ver Exposición en YouTube (Parte Común + Individual)](https://www.youtube.com/watch?v=VIDEO_MARIO_PLACEHOLDER)
* 🔴 **Vídeo de Samuel García Ruiz:** [Ver Exposición en YouTube (Parte Común + Individual)](https://www.youtube.com/watch?v=VIDEO_SAMUEL_PLACEHOLDER)

> ⚠️ *Nota: Los enlaces anteriores contienen marcadores de posición (`VIDEO_MARIO_PLACEHOLDER` y `VIDEO_SAMUEL_PLACEHOLDER`). Asegúrate de editarlos con las URLs definitivas de tus vídeos subidos a YouTube.*

---

## 👥 Datos de los Alumnos
* **Mario García Luque** — [GitHub Profile](https://github.com/Mariogarluu)
* **Samuel García Ruiz** — [GitHub Profile](https://github.com/sgarrui1201)
* **Centro Educativo:** CPIFP Alan Turing (PTA, Málaga)
* **Curso Académico:** 2025 / 2026 (2º DAM Mañana)

---

## 🛠️ Tecnologías Utilizadas

### Ecosistema TraIA (B2B CRM & ERP)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-B738CF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Meta API](https://img.shields.io/badge/Meta_APIs-0668E1?style=for-the-badge&logo=meta&logoColor=white)

### Ecosistema Tripmatch (B2C Tinder de Viajes)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)

### Herramientas de Metodología y Desarrollo
![Jira](https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor_IDE-002E5B?style=for-the-badge&logo=cursor&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_AI-8E75C2?style=for-the-badge&logo=google-gemini&logoColor=white)

---

## 📂 Visión General del Proyecto

Durante nuestra estancia 100% presencial en **LD Quantum**, participamos activamente en un entorno de desarrollo profesional colaborando en el diseño y despliegue de dos grandes ecosistemas de software paralelos:

```mermaid
graph TD
    %% Clients
    Agent([Agencia de Viajes B2B]) -->|Gestiona operaciones| TraIA[TraIA - CRM/ERP]
    Traveler([Viajero Final B2C]) -->|Conecta con otros| Tripmatch[Tripmatch - Tinder de Viajes]

    %% TraIA Tech
    subgraph TraIA_Arch [Ecosistema TraIA]
        Vite[React + Vite + Tailwind] -->|Frontend UI| Supabase[(Supabase Backend)]
        Supabase -->|Persistencia| Postgres[(PostgreSQL DB)]
        Supabase -->|Seguridad de Datos| RLS[Row Level Security RLS]
        Vite -->|Edge Functions| MetaAPI[Meta APIs WhatsApp/Instagram]
    end

    %% Tripmatch Tech
    subgraph Tripmatch_Arch [Ecosistema Tripmatch]
        NextJS[Next.js App] -->|Frontend / SSR / SEO| OpenAI[OpenAI API Matchmaking]
    end

    %% Tools
    Jira[JIRA - Sprints & Tickets] -.->|Planificación Ágil| TraIA_Arch
    Jira -.->|Planificación Ágil| Tripmatch_Arch
    Git[GitHub Flow & Merges] -.->|Control de Versiones| TraIA_Arch
    Git -.->|Control de Versiones| Tripmatch_Arch
```

### 1. TraIA (Business-to-Business - B2B)
Es el producto estrella de la compañía. Se trata de un **CRM y ERP integral** adaptado a agencias de viaje tradicionales. Permite:
* Centralizar toda la facturación, presupuestos y fichas de clientes.
* Generar itinerarios de viaje automatizados potenciados con Inteligencia Artificial.
* Comunicarse con clientes integrando las APIs oficiales de Meta (WhatsApp, Instagram, etc.) mediante **Edge Functions** de Supabase.

### 2. Tripmatch (Business-to-Consumer - B2C)
Nacido de la necesidad de dar un espacio propio al viajero final. Es una plataforma con un concepto tipo **"Tinder de viajes"** para conectar viajeros con destinos o afinidades compartidas.
* Desarrollado con total autonomía técnica y creativa por Samuel y Mario.
* Utiliza el framework **Next.js** para maximizar el posicionamiento en buscadores (SEO) y Server-Side Rendering (SSR).
* Implementa la API de **OpenAI** para procesar mediante lenguaje natural y afinar la compatibilidad entre perfiles.

---

## 👥 Contribuciones Individuales

A continuación se detallan las responsabilidades e hitos técnicos logrados de manera individual por cada miembro del equipo de desarrollo.

### 💻 Mario García Luque (Ponente B)
* **Gestión de Metodologías Ágiles (JIRA):** Implantación de la herramienta JIRA en la empresa, configurando el tablero Kanban, sprints, priorización de tareas y reporte de incidencias.
* **Integración de IA en el Workflow:** Introducción de herramientas como Cursor IDE y Gemini para acelerar el desarrollo del equipo.
* **Chatbots Inteligentes:** Desarrollo del chatbot de **Tripmatch** (vía OpenAI API) para sugerir matches y planificar itinerarios, así como el chatbot interno de **TraIA** para soporte y navegación del CRM.
* **Gestión de Estado en Frontend (React):** Diseño e implementación del **Portal de Reservas** y **Portal del Cliente** en TraIA, manejando estados dinámicos avanzados (Contextos y hooks personalizados) para actualizar las reservas en tiempo real de forma no bloqueante y evitar parpadeos visuales (reduciendo peticiones redundantes).
* **Mantenimiento y Estabilidad:** Refactorización de código TypeScript, optimización de rendimiento en vistas complejas y control de pases a producción.

### 💻 Samuel García Ruiz (Ponente A)
* **Persistencia y Backend (Supabase/PostgreSQL):** Diseño del modelo relacional, modificación del esquema de base de datos en PostgreSQL, creación de relaciones complejas y configuración de políticas de seguridad a nivel de fila (**RLS - Row Level Security**) para proteger los datos corporativos.
* **Dashboard y Estadísticas (TraIA):** Desarrollo visual de la interfaz del panel de métricas con gráficos interactivos dinámicos y optimización de consultas masivas a Supabase mediante carga no bloqueante.
* **Módulo de Comunicación y Marketing:** Maquetación responsive de plantillas para Email Marketing y optimización de la usabilidad del constructor de cartelería y folletos (integración de emojis nativos, e historial de edición deshacer/rehacer).
* **Desarrollo en Tripmatch & Bugs:** Diseño UI inicial de la aplicación Next.js y resolución de inconsistencias visuales (capas z-index en menús flotantes, validaciones de formularios y control de navegación interna).

---

## 📅 Temporalización Semanal de Tareas

A continuación se detalla la planificación temporal de las 12 semanas de estancia en la empresa LD Quantum:

| Semana | Actividad / Tareas de Mario García Luque | Actividad / Tareas de Samuel García Ruiz |
| :---: | :--- | :--- |
| **Semanas 1-2** | Configuración de JIRA (tablero Kanban, flujos de trabajo, sprints) y estructuración inicial del repositorio de Git. | Análisis del modelo de datos de TraIA en Supabase, familiarización con la base de datos PostgreSQL. |
| **Semanas 3-4** | Desarrollo e integración inicial del Chatbot en Tripmatch (API OpenAI) y diseño de la estructura del Portal del Viajero. | Creación de esquemas de tablas en Supabase y configuración de políticas RLS para seguridad. |
| **Semanas 5-6** | Implementación del Portal de Reservas en TraIA. Programación de estados avanzados con React Context y hooks personalizados. | Desarrollo del módulo de estadísticas de TraIA. Rediseño visual del dashboard con gráficos dinámicos y carga asíncrona. |
| **Semanas 7-8** | Desarrollo del chatbot interno de TraIA para asistencia y navegación del CRM. Soporte en el maquetado del Portal del Cliente. | Desarrollo del constructor de cartelería y folletos (editor de posters). Implementación de deshacer/rehacer y emojis. |
| **Semanas 9-10** | Planificación, diseño UX/UI e inicio del desarrollo del proyecto Tripmatch (B2C) en Next.js enfocado a SEO. | Diseño y maquetado responsive de las plantillas del módulo de Email Marketing. Integración de componentes en Tripmatch. |
| **Semanas 11-12** | Refactorización de tipos de TypeScript, pruebas finales de integración, optimización de velocidad de carga y paso a producción. | Resolución de bugs visuales (z-index de menús flotantes, navegación interna) y validación de formularios en Tripmatch. |

---

## 📈 Metodología y Control de Versiones

Trabajando en la misma oficina presencial junto a otros compañeros, el control de versiones fue fundamental para asegurar la integración continua del código.
* **Metodología Ágil:** Sprints semanales con seguimiento diario en Jira.
* **GitHub Flow:** Cada desarrollador trabajaba en una rama propia (ej. `Samuel` o `Mario`).
* **Integración Continua:** Realización de merges diarios hacia la rama de desarrollo (`Develop`), lo que obligó a una constante resolución de conflictos complejos y fomento de buenas prácticas de programación colaborativa.

---

## 🏫 Alineación con el Currículo DAM (Conocimientos Adquiridos)

El desarrollo de estos proyectos permitió poner en práctica directa las competencias clave de varios módulos académicos del ciclo:
* **Desarrollo de Interfaces (DI):** Construcción de interfaces interactivas complejas, optimización UX/UI y adaptabilidad en pantallas para CRM/ERP (React) y Next.js.
* **Acceso a Datos (AD):** Consultas avanzadas a PostgreSQL, optimización de peticiones asíncronas de datos masivos y seguridad RLS con Supabase.
* **Entornos de Desarrollo (ED):** Control de flujo de ramas de Git, resolución de conflictos cotidianos en equipo y gestión de proyectos con metodologías ágiles Jira.
* **Sistemas de Gestión Empresarial (SGE):** Arquitectura y módulos funcionales de un sistema CRM/ERP real para empresas turísticas (TraIA).
* **Programación de Servicios y Procesos (PSP):** Consumo de APIs RESTful de terceros (OpenAI API, Meta APIs) y desarrollo de Edge Functions.

---

## 🌟 Valoración de la Experiencia Dual

### Mario García Luque
> "Mi experiencia en LD Quantum ha sido sumamente enriquecedora. Trabajar en un entorno de oficina 100% presencial junto a otros desarrolladores me ha enseñado a coordinar esfuerzos de manera ágil. Instaurar la metodología Scrum con JIRA y optimizar nuestro flujo con herramientas de IA (como Gemini y Cursor) ha cambiado por completo mi forma de abordar el desarrollo de software. Además, el reto de gestionar estados complejos en el frontend de TraIA y diseñar sistemas conversacionales con OpenAI me ha dado una base sólida para afrontar el mercado laboral como desarrollador Fullstack."

### Samuel García Ruiz
> "Estas prácticas duales me han brindado la oportunidad de trabajar con tecnologías modernas en proyectos de escala real. Encargarme del diseño de base de datos y la seguridad con Supabase RLS me ha aportado un conocimiento profundo sobre acceso a datos y seguridad. Además, desarrollar componentes avanzados en TraIA y tener la autonomía de idear y construir Tripmatch desde cero ha potenciado mi capacidad de resolución de problemas. La colaboración mediante Git y la resolución diaria de conflictos de código ha sido un aprendizaje fundamental que no se puede replicar fácilmente en el aula."

---

## 🎥 Índice de la Presentación de Prácticas

La defensa académica del proyecto está dividida en las siguientes piezas audiovisuales y guiones:

### 1. Presentación Conjunta de Proyecto (Duración: 5:00 min)
* **0:00 - 2:30 — Samuel García Ruiz (Parte 1)**
  * Introducción al equipo, estancia dual presencial en LD Quantum.
  * Presentación de **TraIA** (CRM/ERP), objetivos de digitalización turística y Stack Tecnológico (React, Vite, Tailwind CSS, Supabase, Meta API integration).
  * Metodología de gestión de proyectos mediante Jira.
* **2:30 - 5:00 — Mario García Luque (Parte 2)**
  * Control de versiones diario en GitHub, merges y resolución de conflictos.
  * Transición a **Tripmatch** (B2C), autonomía en el diseño y arquitectura del proyecto.
  * Stack técnico de Tripmatch (Next.js, OpenAI API) e integración con los módulos del grado superior.

### 2. Vídeo de Contribución Individual — Samuel García Ruiz (Duración: 5:00 min)
* **0:00 - 1:00 — Introducción y Backend:** Jira, ramas GitHub y Supabase (Esquemas PostgreSQL y políticas RLS).
* **1:00 - 2:15 — Panel de Estadísticas:** Dashboard interactivo en TraIA y optimización de carga de datos masivos.
* **2:15 - 3:30 — Email Marketing y Cartelería:** Plantillas responsive y refinamiento de controles del editor (historial deshacer/rehacer y emojis).
* **3:30 - 4:30 — Tripmatch y Resolución de Bugs:** Solución de bugs visuales (z-index, menús interactivos, validaciones de registro).
* **4:30 - 5:00 — Conclusiones:** Evolución personal y cierre.

### 3. Vídeo de Contribución Individual — Mario García Luque (Duración: 5:00 min)
* **Estructura de defensa:**
  * **Introducción y Agile:** Implementación de Jira y cultura ágil del equipo de desarrollo, uso de Cursor IDE y asistentes IA en el día a día.
  * **Chatbots e IA Conversacional:** Lógica e integración con la API de OpenAI para el recomendador de Tripmatch y el asistente del ERP TraIA.
  * **Portal del Cliente/Viajero:** Desarrollo de React Hooks y Contextos para la visualización del estado de las reservas.
  * **Optimización y Estabilidad:** Tipado fuerte con TypeScript y correcciones finales para despliegue en producción.
  * **Cierre y Lecciones Aprendidas:** Gestión del ciclo de vida del software en proyectos reales.
