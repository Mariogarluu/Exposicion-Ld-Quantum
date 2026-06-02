# Guion de Presentación: LDQuantum (TraIA & Tripmatch)

**Duración Total:** 15 minutos
**Audiencia:** Tribunal Académico (TFG / Proyecto Final)
**Ponentes:** Mario García y Samuel García

---

## PARTE 1: Presentación Conjunta de la Empresa y Proyectos (00:00 - 05:00)
**Hablan Mario y Samuel (pueden alternarse)**

**(Minuto 0:00 - 1:00) Introducción a LDQuantum**
*   **Mario/Samuel:** "Buenos días a los miembros del tribunal. Hoy venimos a presentaros el ecosistema de software desarrollado bajo nuestra empresa **LDQuantum**. Nuestro objetivo como empresa B2B es revolucionar y digitalizar el sector del turismo, proporcionando software avanzado a las agencias de viaje tradicionales que necesitan modernizarse para sobrevivir y competir."

**(Minuto 1:00 - 2:30) Producto Estrella: TraIA**
*   **Mario/Samuel:** "Para resolver este problema, hemos creado nuestro producto principal: **TraIA**. TraIA es un CRM/ERP integral diseñado específicamente para agencias de viaje, pero potenciado con Inteligencia Artificial.
*   No solo permite gestionar reservas y clientes, sino que automatiza tareas repetitivas.
*   **A nivel técnico**, TraIA está construido con una arquitectura moderna: el Frontend utiliza **React y Vite**, con estilizado mediante Tailwind CSS. En el Backend, nos apoyamos en **Supabase** para la base de datos y autenticación, y contamos con integraciones complejas con la API de Meta (WhatsApp, Facebook, Instagram) a través de Edge Functions."

**(Minuto 2:30 - 4:00) El Ecosistema B2C: Tripmatch**
*   **Mario/Samuel:** "Pero no queríamos quedarnos solo en la gestión interna de la agencia. Nos dimos cuenta de que el viajero moderno busca algo más: conexión. Así nace **Tripmatch**.
*   Tripmatch funciona de forma análoga a un 'Tinder de viajes'. Es una plataforma para los usuarios finales que permite hacer *match* entre viajeros con intereses compatibles o que van a los mismos destinos.
*   **A nivel tecnológico**, a diferencia de TraIA, Tripmatch está desarrollado utilizando **Next.js** (aprovechando SSR y optimización SEO), integrado directamente con modelos de lenguaje de **OpenAI** para procesar afinidades."

**(Minuto 4:00 - 5:00) Cierre de la primera parte**
*   **Mario/Samuel:** "Como podéis ver, en LDQuantum ofrecemos un ecosistema doble: TraIA para la agencia (B2B) y Tripmatch para el viajero (B2C). A continuación, vamos a desglosar cómo nos hemos dividido el trabajo arquitectónico y de desarrollo para sacar ambos proyectos adelante."

---

## PARTE 2: Desarrollo Individual - Mario García (05:00 - 10:00)
**Habla Mario García**

**(Minuto 5:00 - 6:00) Metodología y Gestión del Proyecto**
*   **Mario:** "En mi rol dentro del equipo, no solo me he centrado en el desarrollo de código, sino también en la **cultura de ingeniería y metodologías ágiles**. 
*   Fui el responsable de **instaurar JIRA** en la empresa. Esto nos ha permitido organizar sprints, gestionar tickets, y tener trazabilidad total de bugs y nuevas features, algo crucial al manejar dos proyectos simultáneamente.
*   Además, integré el uso de **herramientas de Inteligencia Artificial como Gemini y el IDE Cursor** en nuestro flujo de trabajo diario. Esto ha acelerado enormemente nuestro desarrollo, permitiéndonos iterar rápido, resolver bugs complejos y refactorizar código de forma eficiente."

**(Minuto 6:00 - 7:30) IA y Chatbots: Tripmatch y TraIA**
*   **Mario:** "Entrando en la parte técnica de desarrollo, fui el encargado de implementar la lógica conversacional de nuestros sistemas.
*   En **Tripmatch**, desarrollé el Chatbot inteligente integrado con la API de OpenAI. Este bot actúa como asistente para los usuarios, ayudándoles a definir su viaje ideal y sugiriendo 'matches' basándose en procesamiento de lenguaje natural.
*   De igual forma, trasladé y adapté esa lógica para crear el **Chatbot de TraIA**, dotando a las agencias de viaje de un asistente virtual que les ayuda a navegar por el CRM o atender consultas."

**(Minuto 7:30 - 9:00) Frontend: Portal de Reservas y Clientes**
*   **Mario:** "Mi otro gran foco ha sido el Frontend en TraIA, concretamente el **Portal de Reservas y el Portal del Cliente/Viajero**.
*   Esta ha sido una de las partes más desafiantes a nivel de UI/UX. Tuve que gestionar estados complejos en React (utilizando Contextos y custom hooks) para asegurar que la visualización de itinerarios y reservas se actualizara en tiempo real sin parpadeos ni peticiones redundantes.
*   Desarrollé la interfaz para reservas tanto grupales como individuales."

**(Minuto 9:00 - 10:00) Arreglos Generales y Mantenimiento**
*   **Mario:** "Finalmente, he llevado a cabo múltiples arreglos generales a lo largo de la aplicación, optimizando el rendimiento, asegurando el tipado y estabilizando el paso a producción. En resumen, mi labor ha sido de Fullstack con fuerte énfasis en la integración de IA, el portal de cara al usuario, y la gestión eficiente del ciclo de vida del software."

---

## PARTE 3: Desarrollo Individual - Samuel García (10:00 - 15:00)
**Habla Samuel García**

> *[Nota: Samuel está preparando esta parte por su cuenta, pero aquí tienes una estructura sugerida para que encaje con el tono general del tribunal].*

**(Minuto 10:00 - 11:00) Introducción de su rol**
*   **Samuel:** Explicación de sus responsabilidades principales (arquitectura backend, integraciones, bases de datos, etc.).

**(Minuto 11:00 - 13:30) Profundidad Técnica**
*   **Samuel:** Detalles técnicos de los módulos de los que se ha encargado (por ejemplo: la complejidad de Edge Functions, webhooks de Meta, integraciones de pago, o modelos de datos en Supabase).

**(Minuto 13:30 - 14:30) Resolución de Retos**
*   **Samuel:** Explicación de un reto técnico concreto que haya tenido que resolver (seguridad, rendimiento, etc.).

**(Minuto 14:30 - 15:00) Cierre Final Conjunto**
*   **Samuel / Mario:** Agradecimiento al tribunal y apertura del turno de preguntas y respuestas.
