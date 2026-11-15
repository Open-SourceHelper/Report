## Capítulo IV: Product Design

### 4.1 Style Guidelines

En esta sección se establecen los lineamientos visuales y comunicativos que guiarán el diseño de la plataforma, con el objetivo de garantizar una experiencia consistente, accesible y alineada al dominio terapéutico. Las decisiones de diseño se fundamentan en principios de claridad, accesibilidad y confianza, tomando como referencia buenas prácticas de sistemas de diseño como Material Design.

#### 4.1.1 General Style Guidelines

**Branding:**

Kinemo está enfocado, fundamentalmente, en familias, cuidadores y profesionales que acompañan a niños y niñas de 3 a 12 años con condiciones del neurodesarrollo como TEA, TDAH y síndrome de Down. Por esto mismo, la identidad visual del mismo busca transmitir confianza, cercanía, accesibilidad y acompañamiento.

La identidad de Kinemo intenta representar una herramienta de apoyo de la organización de rutinas y continuidad del cuidado del niño, facilitando la comunicación entre padres, familiares, cuidadores y profesionales. En consecuencia el diseño evita elementos gráficos complejos o sobrecargados y prioriza una interfaz clara, intuitiva y de fácil comprensión y lenguaje.

Con ello se busca generar la sensación de seguridad y tranquilidad, considerando que los
usuarios pueden consultar la plataforma en situaciones de la vida cotidiana, en las cuales requieren acceder rápidamente a información sobre rutinas, estrategias de apoyo o pautas personalizadas para el niño.

**Typography:**

Para la escritura de la tipografía se ha optado por una sin serifa debido a su buena legibilidad en formatos digitales, y su facilidad para ser leída por los diferentes perfiles de usuario de Kinemo. La tipografía jerárquica se organiza de la siguiente forma:

* Títulos: tamaño grande, peso bold, para marcar las secciones de contenido principal.
* Subtítulos: tamaño medio, peso semi-bold.
* Texto general: tamaño estándar, peso regular.
* Botones y etiquetas: tamaño medio, matiz visual. Esta estructura se traduce en una lectura fácil, lo cual resulta especialmente importante para los padres de familia, que necesitan asimilar rápidamente la información, así como para usuarios con distintas capacidades cognitivas.

Con esta estructura, se puede presentar la información de forma clara y permitir practicar una lectura rápida, sobre todo si se trata de guías prácticas, rutinas visuales, recomendaciones que puedan llegar a consultar los cuidadores del niño, durante los momentos de atención diaria a él.

**Colors:**

La paleta de colores de Kinemo incluye colores principales, secundarios, de acento y neutros. El objetivo es tener una interfaz clara, accesible y coherente.

* Morado (Color principal): El morado es el que representa mayor empatía, sensibilidad y apoyo. El morado es el color sin lugar a dudas, apropiado para un entorno relacionado con la atención y el desarrollo de personas con necesidades especiales, pues transmite la proximidad y comprensión necesarias.
* Azul (Color secundario): Refuerza la confianza, la seguridad y el profesionalismo. El azul será clave para que los padres de familia se sientan tranquilos y tengan credibilidad de que los servicios que ofrece la plataforma son verdaderos.
* Amarillo (Color de acento): Brinda energía, optimismo y dinamismo. Se utiliza en elementos interactivos o enfatizados (botones o notificaciones) para llamar la atención proporcionando una señal de alerta pero sin saturación visual.
* Colores neutros (blanco y grises): Se utilizan como base para los fondos y las estructuras así que permiten que la interfaz sea limpia, legible y fácil de navegar.

**Spacing:**

Se aplica un sistema de espaciado basado en una cuadrícula modular (8px) para poder conseguir una uniformidad visual en toda la interfaz. El espaciado correcto entre los elementos permite:

* Mejorar la legibilidad.
* Evitar la saturación visual.
* Facilitar la navegación.

| **Token** | **Valor (px)** | **Valor (DXA/rem)** | **Aplicación**                                  |
|-----------|----------------|---------------------|-------------------------------------------------|
| space-1   | 4px            | 0.25rem             | Separación interna mínima (icono + texto)       |
| space-2   | 8px            | 0.5rem              | Padding interno de chips y badges               |
| space-3   | 12px           | 0.75rem             | Padding de campos de texto (input)              |
| space-4   | 16px           | 1rem                | Padding estándar de tarjetas y botones          |
| space-5   | 20px           | 1.25rem             | Separación entre componentes relacionados       |
| space-6   | 24px           | 1.5rem              | Margen entre secciones de formulario            |
| space-8   | 32px           | 2rem                | Separación entre secciones de contenido         |
| space-10  | 40px           | 2.5rem              | Padding de secciones principales (contenedores) |
| space-12  | 48px           | 3rem                | Espaciado entre bloques de página               |
| space-16  | 64px           | 4rem                | Margen vertical entre secciones de página       |
| space-24  | 96px           | 6rem                | Hero sections y márgenes de pantalla completa   |

Dado que la plataforma incluye una multitud de funcionalidades (calendario, sesiones, marketplace, etc.), los espacios en blanco se convierten en un aspecto clave para conseguir una interfaz ordenada y que el usuario pueda entender.

**Dimensiones a adoptar:**

El tono de comunicación:

| Dimensión                | Posición            | Justificación                                                                  |
|--------------------------|---------------------|--------------------------------------------------------------------------------|
| Divertido / Serio        | Balanceado (50/50)  | Se usa humor con moderación; no trivializa situaciones sensibles de los niños. |
| Formal / Casual          | Semi-formal (40/60) | Tono cercano y accesible para padres, sin perder credibilidad profesional.     |
| Respetuoso / Irreverente | Respetuoso (90/10)  | Siempre empático y sensible a las necesidades especiales.                      |
| Entusiasta / Sereno      | Sereno (30/70)      | Transmite tranquilidad y confianza; evita generar ansiedad en los padres.      |

Lenguaje aplicado: Claro, empático y directo.

Se excluye el empleo del léxico técnico complicado, preponderando mensajes fáciles de entender para los padres de familia. A la vez, se mantiene un tono respetuoso por la sensibilidad que esta problemática conlleva (niños con necesidades especiales).

**Accesibilidad:**

Kinemo se adapta a las distintas capacidades visuales, cognitivas y motrices de los usuarios. Además, dado que la plataforma iba a ser usada por familiares, cuidadores y profesionales, se tuvo en cuenta el diseño de una interfaz sencilla, clara y accesible para el acceso a la información sobre las rutinas, guías y recomendaciones del niño.

Las Web Content Accessibility Guidelines (WCAG) sirvieron de base para el diseño, considerando el nivel AA como mínimo objetivo de accesibilidad. Entre los criterios considerados, cabe destacar:
* Contraste de color: ratio mínimo 4.5:1 para texto normal y 3:1 para texto grande. Todos los colores de la paleta han sido verificados.
* Tamaños táctiles: todos los elementos interactivos tienen un área mínima de 44×44px (WCAG 2.5.5).
* Navegación por teclado: todos los flujos críticos son completamente navegables sin ratón.
* Etiquetas ARIA: todos los componentes interactivos incluyen atributos aria-label, aria-describedby o roles semánticos correctos.
* Texto alternativo: todas las imágenes informativas incluyen atributo alt descriptivo.
* Indicador de foco visible: se muestra un outline claro (#5B2D8E, 3px) al navegar con teclado.
* Compatibilidad multiplataforma: web (Chrome, Firefox, Safari, Edge), iOS y Android.
* Modo de alto contraste: se respetan las preferencias del sistema operativo (prefers-contrast: more).
* Reducción de movimiento: las animaciones se desactivan si el usuario tiene activado prefers-reduced-motion.

#### 4.1.2 Web Style Guidelines

En esta sección se explican e ilustran las decisiones sobre los estándares visuales y de interacción para las interfaces web responsivas de la plataforma. Se definen los componentes, patrones de interacción y especificaciones técnicas para el desarrollo front-end web.

**Breakpoints y Diseño Responsivo:**

La interfaz web adopta un enfoque mobile-first, escalando progresivamente hacia pantallas más grandes. Se definen los siguientes breakpoints:

* xs — < 480px: Móviles pequeños (diseño base).
* sm — 480px – 767px: Móviles grandes y phablets.
* md — 768px – 1023px: Tablets en orientación vertical.
* lg — 1024px – 1279px: Tablets en horizontal y laptops pequeñas.
* xl — 1280px – 1535px: Desktops estándar.
* 2xl — ≥ 1536px: Pantallas grandes y monitores 4K.

**Componentes Base:**

Los componentes de la interfaz web siguen el sistema de componentes de Material Design 3, adaptados a la identidad visual de la plataforma. A continuación se documentan los principales:

Botones:
* Primario (Filled): Fondo #F5A623 texto blanco, border-radius 8px, padding 12px 24px. Hover: #7B4DB0. Active: #4A2070.
* Acento (Filled Tonal): Fondo #F5A623, texto #111827, border-radius 8px. Para CTAs de alta visibilidad.
* Ghost / Text: Sin borde ni fondo. Texto #5B2D8E. Para acciones de baja prioridad.
* Destructivo: Fondo #C62828, texto blanco. Solo para acciones irreversibles (eliminar, cancelar sesión). Todos los botones incluyen: estado disabled (opacidad 38%), indicador de foco visible, estado loading con spinner, y mínimo 44px de altura para accesibilidad táctil.

Inputs y Formularios:
* Campo de texto: border 1px #5B2D8E, border-radius 6px, padding 12px 16px. Focus: border 2px #5B2D8E + box-shadow 0 0 0 3px #EDE5F7.
* Estado de error: border 2px #C62828, mensaje de error en #C62828 debajo del campo.
* Estado de éxito: border 2px #2E7D32 + icono de check en el campo.
* Labels: siempre visibles (no dependen del placeholder). Texto #343A40, Body Medium.
* Helper text: texto secundario debajo del campo, Color #6C757D, Body Small.

Tarjetas (Cards):
* Fondo: #FFFFFF, border-radius 12px, box-shadow 0 2px 8px rgba(0,0,0,0.08).
* Borde opcional: 1px #DEE2E6 para tarjetas en fondos de mismo color.
* Padding interno: 24px (space-6).
* Hover interactivo: box-shadow 0 4px 16px rgba(91,45,142,0.12), transform translateY(-2px), transición 200ms ease.

Navegación:
* Top App Bar (desktop): altura 64px, fondo #FFFFFF, sombra sutil. Logo a la izquierda, navegación principal centrada, acciones de usuario a la derecha.
* Sidebar (dashboard): ancho 260px colapsado a 72px en tablet. Fondo #F8F9FA, íconos + labels. Ítem activo: fondo #EDE5F7, texto #5B2D8E, borde izquierdo 3px #5B2D8E.
* Bottom Navigation (mobile): 4–5 destinos, íconos + labels cortos, ítem activo en #5B2D8E.
* Breadcrumbs: separador /, texto #111827, ítem activo #343A40, Body Medium.

Iconografía:
* Biblioteca base: Material Symbols (Google) en variante Rounded.
* Tamaños: 20px (inline/label), 24px (estándar), 32px (destacado), 48px (hero/vacío).
* Color por defecto: hereda del contexto. En superficies claras: #343A40. En superficies de color: #FFFFFF.
* Íconos de estado: siempre acompañados de texto (no dependen del ícono solo para transmitir información).

### 4.2 Information Architecture

#### 4.2.1 Organization Systems

> _Pendiente — completar en `feature/information-architecture`._

#### 4.2.2 Labeling Systems

> _Pendiente — completar en `feature/information-architecture`._

#### 4.2.3 SEO Tags and Meta Tags

> _Pendiente — completar en `feature/information-architecture`._

#### 4.2.4 Searching Systems

> _Pendiente — completar en `feature/information-architecture`._

#### 4.2.5 Navigation Systems

> _Pendiente — completar en `feature/information-architecture`._

### 4.3 Landing Page UI Design

#### 4.3.1 Landing Page Wireframe

> _Pendiente — completar en `feature/landing-page-ui`._

#### 4.3.2 Landing Page Mock-up

> _Pendiente — completar en `feature/landing-page-ui`._

### 4.4 Web Applications UX/UI Design

#### 4.4.1 Web Applications Wireframes

> _Pendiente — completar en `feature/web-app-ux`._


#### 4.4.2. Web Applications Wireflow Diagrams

El Wireflow Diagram representa la relación entre las principales interfaces de Kinemo y las acciones que permiten pasar de una pantalla a otra. El flujo comienza con los procesos de autenticación y registro y, una vez iniciada la sesión, conduce al Panel principal.

Desde el Dashboard, el usuario puede acceder a las funcionalidades correspondientes a su rol, como Perfil del niño, Guías prácticas, Rutinas, Observaciones y Red de cuidado. En el caso del psicólogo, se habilita adicionalmente el acceso a Pacientes y a la creación de pautas clínicas. El flujo permite visualizar de manera conjunta la interfaz y la navegación esperada dentro del sistema.


#### 4.4.3 Web Applications Mock-ups

> _Pendiente — completar en `feature/web-app-ux`._

#### 4.4.4 Web Applications User Flow Diagrams

> _Pendiente — completar en `feature/web-app-ux`._

### 4.5 Web Applications Prototyping

> _Pendiente — completar en `feature/web-app-prototyping`._

### 4.6 Domain-Driven Software Architecture

#### 4.6.1 Design-Level EventStorming

> _Pendiente — completar en `feature/domain-driven-architecture`._

#### 4.6.2 Software Architecture Context Diagram

> _Pendiente — completar en `feature/domain-driven-architecture`._

#### 4.6.3 Software Architecture Container Diagrams

> _Pendiente — completar en `feature/domain-driven-architecture`._

#### 4.6.4 Software Architecture Component Diagrams

> _Pendiente — completar en `feature/domain-driven-architecture`._

### 4.7 Software Object-Oriented Design

#### 4.7.1. Class Diagrams

> _Pendiente — completar en `feature/domain-driven-architecture`._

### 4.8 Database Design

#### 4.8.1 Database Diagrams

### BC01 — Identity & Access Management

Este diagrama de base de datos aborda los flujos de la siguiente manera:

- **Users:** Almacena las credenciales de acceso de los usuarios, el correo electrónico único, la contraseña cifrada mediante hash y el estado de validación de la cuenta.
- **User_profiles:** Gestiona los datos personales del usuario, manteniendo una relación de uno a uno con `users` para separar la información personal de las credenciales.
- **Password_recoveries:** Soporta el proceso de recuperación de contraseñas mediante tokens, controlando su estado y fecha de expiración.
- **User_sessions:** Registra las sesiones de los usuarios, incluyendo los momentos de inicio y cierre, permitiendo controlar las sesiones activas.

![Database Diagram BC01](NeuroSync/assets/img/4_8_1-database-diagrams/BC01.png)

### BC02 — Child Profile & Care Network Management

Este Bounded Context fusiona las responsabilidades de **Child Profile Management** y **Care Network Management**.

- **Children:** Gestiona la información principal del niño, incluyendo sus datos personales y la referencia al padre o tutor responsable.
- **Clinical_profiles:** Almacena las características clínicas y conductuales del niño, como necesidades especiales, detonantes y reguladores.
- **Care_networks:** Representa la red de cuidado asociada al niño, permitiendo identificar a las personas que participan en su acompañamiento.
- **Care_network_invitations:** Administra las invitaciones enviadas a nuevos integrantes de la red, incluyendo el estado, token de validación y fecha de expiración.
- **Care_network_members:** Registra los cuidadores incorporados a cada red de cuidado, sus roles, permisos y estado de participación.
- **Caregiver_authorizations:** Controla las autorizaciones otorgadas a los integrantes para consultar información del niño, permitiendo activar o revocar sus accesos.

![Database Diagram BC02](NeuroSync/assets/img/4_8_1-database-diagrams/BC02.png)

### BC03 — Crisis Alert Management

Este Bounded Context está dedicado exclusivamente a la activación, notificación y seguimiento operativo de alertas de crisis. La administración de la red de cuidado corresponde al BC02.

- **Crisis_alerts:** Registra las alertas activadas por cuidadores autorizados, asociándolas con el niño, el usuario que realizó la activación, su estado y fecha de creación. Permite representar los estados de alerta activa, en atención y finalizada.
- **Alert_notifications:** Gestiona las notificaciones generadas a partir de una alerta. Registra el destinatario autorizado, canal, estado del envío y respuesta del proveedor de notificaciones.
- **Alert_status_transitions:** Almacena los cambios de estado realizados sobre una alerta, identificando el estado anterior, el nuevo estado, el usuario responsable y la fecha de modificación.

![Database Diagram BC03](NeuroSync/assets/img/4_8_1-database-diagrams/BC03.png)

### BC04 — Clinical Guidance & Routine Management

Este Bounded Context fusiona las capacidades de **Routine & Activity Management** y **Clinical Guidance Management**, permitiendo administrar las rutinas del niño y las orientaciones proporcionadas por profesionales autorizados.

- **Routines:** Centraliza la creación, eliminación, duplicación y visualización de las rutinas asociadas al niño. Incluye `original_routine_id` para conservar la trazabilidad de las rutinas duplicadas.
- **Routine_activities:** Administra las actividades que conforman una rutina, gestionando su orden, duración, estado y configuración de alertas y temporizadores de transición.
- **Visual_supports:** Gestiona los apoyos visuales y pictogramas asociados a las actividades, almacenando sus URL y formatos.
- **Patient_assignments:** Registra la vinculación profesional entre un psicólogo y un niño. Permite verificar que exista una asignación activa antes de registrar o modificar pautas clínicas.
- **Clinical_guidelines:** Almacena las indicaciones y recomendaciones clínicas redactadas por los profesionales autorizados, permitiendo su creación, consulta y actualización.
- **Practical_guides:** Administra un repositorio de guías prácticas organizadas por categorías, ofreciendo estrategias de acompañamiento que los cuidadores pueden consultar.

![Database Diagram BC04](NeuroSync/assets/img/4_8_1-database-diagrams/BC04.png)

### BC05 — Observation & Crisis History Management

Este Bounded Context se encarga del registro, consulta y seguimiento histórico de observaciones e incidentes de crisis relacionados con el niño.

- **Observations:** Registra las observaciones realizadas por cuidadores autorizados. Contiene la referencia al niño, autor, descripción, fecha y tipo de evento. Permite clasificar las crisis según su intensidad: leve, moderada o severa.
- **Observation_evidences:** Gestiona los archivos adjuntos utilizados como evidencia de una observación, como fotografías u otros apoyos visuales.
- **Psychologist_comments:** Permite a psicólogos autorizados registrar comentarios y retroalimentación sobre las observaciones, facilitando el seguimiento del niño.

![Database Diagram BC05](NeuroSync/assets/img/4_8_1-database-diagrams/BC05.png)