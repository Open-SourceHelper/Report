# Informe de AV1 — Kinemo

## Carátula

![Logo UPC](imagenes/upc-logo.png)

| Campo | Valor                                           |
|---|-------------------------------------------------|
| Universidad | Universidad Peruana de Ciencias Aplicadas (UPC) |
| Carrera | Ingeniería de Software                          |
| Ciclo | 2026-20                                         |
| Código y Nombre del Curso | 1ASI0729 - Desarrollo de Aplicaciones Open Source                     |
| NRC | 7793                                            |
| Profesor | Ivan Robles Fernández                   |
| Nombre del Startup | NeuroSync                               |
| Nombre del Producto | Kinemo                                          |
| año | 2026                                            |

**Integrantes**

| Código     | Apellidos y Nombres        |
|------------|----------------------------|
|  u20241b932 | Huamanchumo Chicchon, Felipe Marcelo |
|  u202416903 | Vilchez Vite, Gabriel Alejandro     |
| u202212327 | Flores Chavez, Fabricio     |
| u202419311 | Matthew Shinko Okuhama Diaz     |
| u202318865 | Trigoso Garrido, Cristian Joseph     |

## Registro de Versiones del Informe

| Versión | Fecha | Autor | Descripción de modificación |
|---|---|---|---|
| 1.0 | |  |  |

## Project Report Collaboration Insights

Repositorio del Project Report: 

> _Pendiente — a partir de AV1, agregar explicación del proceso de elaboración del informe y capturas de los analíticos de colaboración/commits de GitHub._

## Contenido

- [Student Outcome](#student-outcome)
- [Capítulo I: Introducción](#capítulo-i-introducción)
    - [1.1 Startup Profile](#11-startup-profile)
        - [1.1.1 Descripción de la Startup](#111-descripción-de-la-startup)
        - [1.1.2 Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
    - [1.2 Solution Profile](#12-solution-profile)
        - [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problemática)
        - [1.2.2 Lean UX Process](#122-lean-ux-process)
            - [1.2.2.1 Lean UX Problem Statements](#1221-lean-ux-problem-statements)
            - [1.2.2.2 Lean UX Assumptions](#1222-lean-ux-assumptions)
            - [1.2.2.3 Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
            - [1.2.2.4 Lean UX Canvas](#1224-lean-ux-canvas)
    - [1.3 Segmentos objetivo](#13-segmentos-objetivo)
- [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
    - [2.1 Competidores](#21-competidores)
        - [2.1.1 Análisis competitivo](#211-análisis-competitivo)
        - [2.1.2 Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
    - [2.2 Entrevistas](#22-entrevistas)
        - [2.2.1 Diseño de entrevistas](#221-diseño-de-entrevistas)
        - [2.2.2 Registro de entrevistas](#222-registro-de-entrevistas)
        - [2.2.3 Análisis de entrevistas](#223-análisis-de-entrevistas)
    - [2.3 Needfinding](#23-needfinding)
        - [2.3.1 User Personas](#231-user-personas)
        - [2.3.2 User Task Matrix](#232-user-task-matrix)
        - [2.3.3 User Journey Mapping](#233-user-journey-mapping)
        - [2.3.4 Empathy Mapping](#234-empathy-mapping)
    - [2.4 Big Picture EventStorming](#24-big-picture-eventstorming)
    - [2.5 Ubiquitous Language](#25-ubiquitous-language)
- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
    - [3.1 User Stories](#31-user-stories)
    - [3.2 Impact Mapping](#32-impact-mapping)
    - [3.3 Product Backlog](#33-product-backlog)
- [Capítulo IV: Product Design](#capítulo-iv-product-design)
    - [4.1 Style Guidelines](#41-style-guidelines)
        - [4.1.1 General Style Guidelines](#411-general-style-guidelines)
        - [4.1.2 Web Style Guidelines](#412-web-style-guidelines)
    - [4.2 Information Architecture](#42-information-architecture)
        - [4.2.1 Organization Systems](#421-organization-systems)
        - [4.2.2 Labeling Systems](#422-labeling-systems)
        - [4.2.3 SEO Tags and Meta Tags](#423-seo-tags-and-meta-tags)
        - [4.2.4 Searching Systems](#424-searching-systems)
        - [4.2.5 Navigation Systems](#425-navigation-systems)
    - [4.3 Landing Page UI Design](#43-landing-page-ui-design)
        - [4.3.1 Landing Page Wireframe](#431-landing-page-wireframe)
        - [4.3.2 Landing Page Mock-up](#432-landing-page-mock-up)
    - [4.4 Web Applications UX/UI Design](#44-web-applications-uxui-design)
        - [4.4.1 Web Applications Wireframes](#441-web-applications-wireframes)
        - [4.4.2 Web Applications Wireflow Diagrams](#442-web-applications-wireflow-diagrams)
        - [4.4.3 Web Applications Mock-ups](#443-web-applications-mock-ups)
        - [4.4.4 Web Applications User Flow Diagrams](#444-web-applications-user-flow-diagrams)
    - [4.5 Web Applications Prototyping](#45-web-applications-prototyping)
    - [4.6 Domain-Driven Software Architecture](#46-domain-driven-software-architecture)
        - [4.6.1 Design-Level EventStorming](#461-design-level-eventstorming)
        - [4.6.2 Software Architecture Context Diagram](#462-software-architecture-context-diagram)
        - [4.6.3 Software Architecture Container Diagrams](#463-software-architecture-container-diagrams)
        - [4.6.4 Software Architecture Component Diagrams](#464-software-architecture-component-diagrams)
    - [4.7 Software Object-Oriented Design](#47-software-object-oriented-design)
        - [4.7.1 Class Diagrams](#471-class-diagrams)
    - [4.8 Database Design](#48-database-design)
        - [4.8.1 Database Diagrams](#481-database-diagrams)
- [Capítulo V: Product Implementation, Validation & Deployment](#capítulo-v-product-implementation-validation--deployment)
    - [5.1 Software Configuration Management](#51-software-configuration-management)
        - [5.1.1 Software Development Environment Configuration](#511-software-development-environment-configuration)
        - [5.1.2 Source Code Management](#512-source-code-management)
        - [5.1.3 Source Code Style Guide & Coding Conventions](#513-source-code-style-guide--coding-conventions)
        - [5.1.4 Software Deployment Configuration](#514-software-deployment-configuration)
    - [5.2 Landing Page, Services & Applications Implementation](#52-landing-page-services--applications-implementation)
        - [5.2.1 Sprint 1 (AV1)](#521-sprint-1-av1)
        - [5.2.2 Sprint 2 (TB1)](#522-sprint-2-tb1)
        - [5.2.3 Sprint 3 (AV2)](#523-sprint-3-av2)
        - [5.2.4 Sprint 4 (TB2)](#524-sprint-4-tb2)
    - [5.3 Validation Interviews](#53-validation-interviews)
        - [5.3.1 Diseño de Entrevistas](#531-diseño-de-entrevistas)
        - [5.3.2 Registro de Entrevistas](#532-registro-de-entrevistas)
        - [5.3.3 Evaluaciones según heurísticas](#533-evaluaciones-según-heurísticas)
    - [5.4 Video About-the-Product](#54-video-about-the-product)
- [Conclusiones](#conclusiones)
    - [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)
    - [Video About-the-Team](#video-about-the-team)
- [Bibliografía](#bibliografía)
- [Anexos](#anexos)
    - [Anexo A. Videos de Exposiciones](#anexo-a-videos-de-exposiciones)

> Nota: estos enlaces se generaron manualmente siguiendo la convención de anchors de GitHub. Verifícalos una vez renderizado el archivo (clic en el ícono de enlace de cada título) y corrígelos si alguno no coincide, tal como pide el enunciado antes de cada entrega.

## Student Outcome

El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET – EAC - Student Outcome 5**

Criterio: Capacidad de comunicarse efectivamente con un rango de audiencias.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 5.

| Criterio específico | Acciones realizadas | Conclusiones |
|--|---|---|
|  |  |  |

## Capítulo I: Introducción

### 1.1 Startup Profile

#### 1.1.1 Descripción de la Startup

> _Pendiente — completar en `feature/startup-profile`._

#### 1.1.2 Perfiles de integrantes del equipo

> _Pendiente — completar en `feature/startup-profile` (foto, nombres, código, carrera, conocimientos técnicos por integrante)._

### 1.2 Solution Profile

#### 1.2.1 Antecedentes y problemática

#### 1.2.2 Lean UX Process

##### 1.2.2.1 Lean UX Problem Statements

> _Pendiente — completar en `feature/lean-ux-process`._

##### 1.2.2.2 Lean UX Assumptions

> _Pendiente — completar en `feature/lean-ux-process`._

##### 1.2.2.3 Lean UX Hypothesis Statements

> _Pendiente — completar en `feature/lean-ux-process`._

##### 1.2.2.4 Lean UX Canvas

> _Pendiente — completar en `feature/lean-ux-process`._

### 1.3 Segmentos objetivo

> _Pendiente — completar en `feature/target-segments`._

## Capítulo II: Requirements Elicitation & Analysis

### 2.1 Competidores

#### 2.1.1 Análisis competitivo

> _Pendiente — completar en `feature/competitive-analysis`._

#### 2.1.2 Estrategias y tácticas frente a competidores

> _Pendiente — completar en `feature/competitive-analysis`._

### 2.2 Entrevistas

#### 2.2.1 Diseño de entrevistas

> _Pendiente — completar en `feature/interview-design`._

#### 2.2.2 Registro de entrevistas

> _Bloqueado — depende de realizar las entrevistas reales a ambos segmentos objetivo._

#### 2.2.3 Análisis de entrevistas

> _Bloqueado — depende de 2.2.2._

### 2.3 Needfinding

#### 2.3.1 User Personas

> _Pendiente — completar en `feature/user-personas`._

#### 2.3.2 User Task Matrix

> _Pendiente — completar en `feature/user-task-matrix`._

#### 2.3.3 User Journey Mapping

> _Pendiente — completar en `feature/journey-maps`._

#### 2.3.4 Empathy Mapping

> _Pendiente — completar en `feature/empathy-maps`._

### 2.4 Big Picture EventStorming

> _Pendiente — completar en `feature/event-storming-big-picture`._

### 2.5 Ubiquitous Language

> _Pendiente — completar en `feature/ubiquitous-language`._

## Capítulo III: Requirements Specification

### 3.1 User Stories

> _Pendiente — completar en `feature/user-stories`._

### 3.2 Impact Mapping

> _Pendiente — completar en `feature/impact-mapping`._

### 3.3 Product Backlog

> _Pendiente — completar en `feature/product-backlog`._

## Capítulo IV: Product Design

### 4.1 Style Guidelines

#### 4.1.1 General Style Guidelines

> _Pendiente — completar en `feature/style-guidelines`._

#### 4.1.2 Web Style Guidelines

> _Pendiente — completar en `feature/style-guidelines`._

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

#### 4.4.2 Web Applications Wireflow Diagrams

> _Pendiente — completar en `feature/web-app-ux`._

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

![Class Diagram BC01](imagenes/DC%201.png)

El diagrama de clases del Bounded Context Identity & Access Management representa la estructura encargada de gestionar la identidad, autenticación y acceso de los usuarios de Kinemo. User se define como Aggregate Root, ya que centraliza las principales operaciones relacionadas con el registro, autenticación, asignación de roles y administración de la cuenta.

Dentro del agregado se encuentran entidades como UserProfile, PasswordRecovery y UserSession, responsables de gestionar la información personal, la recuperación de contraseñas y las sesiones del usuario. Asimismo, se incorpora Email como Value Object y enumeraciones para representar los roles y estados definidos por el dominio. Los Domain Events, como UserRegistered y PasswordChanged, permiten representar acontecimientos relevantes producidos durante el ciclo de vida de una cuenta.

![Class Diagram BC02](imagenes/DC%202.png)

El diagrama de clases del Bounded Context Child Profile Management representa la administración de la información del niño y su perfil de apoyo. Child se establece como Aggregate Root, siendo responsable de mantener los datos principales del menor y controlar los elementos asociados a su perfil.

ClinicalProfile permite registrar las necesidades particulares, detonantes y reguladores del niño, mientras que CaregiverAuthorization administra las autorizaciones de acceso. Se utilizan referencias mediante identificadores para evitar duplicar entidades pertenecientes a otros Bounded Contexts. Además, se incorporan un Value Object para representar el nombre del niño, enumeraciones para controlar los estados de autorización y Domain Events relacionados con el registro del niño y la actualización de su perfil clínico.

![Class Diagram BC03](imagenes/DC%203.png)

El diagrama de clases del Bounded Context Care Network Management representa la gestión de la red de personas autorizadas para participar en el cuidado del niño. CareNetwork funciona como Aggregate Root y administra tanto las invitaciones como los integrantes pertenecientes a la red.

CareNetworkInvitation representa las invitaciones enviadas a nuevos cuidadores, mientras que CareNetworkMember mantiene la información de los integrantes incorporados, sus roles, permisos y estado de acceso. Se utilizan enumeraciones para controlar los estados de las invitaciones y miembros, y PermissionSet representa los permisos como Value Object. Los Domain Events permiten representar situaciones relevantes como el envío de una invitación o la revocación del acceso de un cuidador. Las entidades de otros contextos no son duplicadas y se referencian mediante sus identificadores.

![Class Diagram BC04](imagenes/DC%204.png)

El diagrama de clases del Bounded Context Routine & Activity Management representa la creación, organización y ejecución de las rutinas utilizadas en el acompañamiento cotidiano del niño. Routine se define como Aggregate Root y administra el conjunto de actividades que conforman cada rutina.

RoutineActivity representa las actividades individuales y permite registrar su orden, duración, estado, temporizador y tipo de alerta. VisualSupport permite asociar imágenes o recursos visuales a las actividades. Las enumeraciones controlan los estados de rutinas y actividades, así como los tipos de alerta, mientras que Duration se representa como Value Object. También se mantiene una relación recursiva entre rutinas para conservar la trazabilidad cuando una rutina es duplicada. Los Domain Events representan acontecimientos como la creación y duplicación de una rutina o la finalización de una actividad.

![Class Diagram BC05](imagenes/DC%205.png)

El diagrama de clases del Bounded Context Clinical Guidance Management representa la gestión de las pautas clínicas y orientaciones utilizadas para apoyar el cuidado del niño. ClinicalGuideline se establece como Aggregate Root, encargándose del registro, actualización, validación y disponibilidad de las pautas creadas por los profesionales.

PatientAssignment permite comprobar que exista una asignación profesional activa antes de gestionar una pauta, mientras que PracticalGuide representa el repositorio independiente de guías prácticas que pueden consultarse por categoría o situación. Las instrucciones de una pauta se representan mediante un Value Object, y las enumeraciones permiten controlar estados y categorías. Los Domain Events registran acontecimientos relevantes como la creación o actualización de una pauta clínica. Las referencias a psicólogos y niños se mantienen mediante identificadores para respetar los límites entre Bounded Contexts.

![Class Diagram BC06](imagenes/DC%206.png)

El diagrama de clases del Bounded Context Observation & Crisis Management representa el registro y seguimiento de observaciones relacionadas con el comportamiento, rutinas y situaciones de crisis del niño. Observation se define como Aggregate Root y concentra las operaciones principales relacionadas con el registro, validación, consulta y filtrado del historial.

CrisisClassification permite clasificar una crisis según su nivel de intensidad, mientras que ObservationEvidence permite adjuntar evidencia y PsychologistComment almacena la retroalimentación profesional. Los niveles de intensidad se representan mediante una Enumeration con los valores leve, moderado y severo, evitando manejar esta regla únicamente como texto. También se incorporan Domain Events para representar el registro de observaciones, la clasificación de crisis y la incorporación de comentarios profesionales.

![Class Diagram BC07](imagenes/DC%207.png)

El diagrama de clases del Bounded Context Dashboard & Reporting representa la consulta de información consolidada y la generación de reportes sobre el seguimiento del niño. GeneratedReport se establece como Aggregate Root, ya que administra el proceso de solicitud, generación, almacenamiento y exportación de los reportes.

DailySummary se identifica como Read Model, debido a que consolida información proveniente de otros contextos para mostrar indicadores sin asumir la responsabilidad de modificar los registros originales. ReportObservation permite conservar la trazabilidad de las observaciones incluidas en cada reporte y ReportPeriod representa el intervalo temporal como Value Object. Asimismo, los estados del reporte se controlan mediante una enumeración y ReportGenerated representa el Domain Event producido cuando un reporte es generado correctamente.

![Class Diagram BC08](imagenes/DC%208.png)

El diagrama de clases del Bounded Context Subscription & Payment Management representa la administración de los planes, suscripciones, pagos y solicitudes de cancelación de Kinemo. Subscription se define como Aggregate Root, controlando el ciclo de vida de la suscripción y su relación con las operaciones de pago y cancelación.

SubscriptionPlan representa los planes familiares y profesionales disponibles, mientras que Payment mantiene el historial de las transacciones realizadas y CancellationRequest gestiona las solicitudes de cancelación al finalizar el ciclo correspondiente. El precio se representa mediante Money como Value Object, y diferentes enumeraciones controlan los tipos de plan y los estados de planes, suscripciones y pagos. Los Domain Events representan acontecimientos relevantes como la confirmación de un pago, la activación de una suscripción y la solicitud de cancelación. La activación de una suscripción se encuentra condicionada a la confirmación válida del pago, manteniendo además la separación con Identity & Access mediante la referencia userId.

### 4.8 Database Design

#### 4.8.1 Database Diagrams

> _Pendiente — completar en `feature/database-design`._

## Capítulo V: Product Implementation, Validation & Deployment

### 5.1 Software Configuration Management

#### 5.1.1 Software Development Environment Configuration

> _Pendiente — completar en `feature/software-configuration-management` (urgente para AV1)._

#### 5.1.2 Source Code Management

> _Pendiente — agregar URLs de los 4 repositorios, explicación de GitFlow, convenciones de branches y Conventional Commits. Completar en `feature/software-configuration-management` (urgente para AV1)._

#### 5.1.3 Source Code Style Guide & Coding Conventions

> _Pendiente — completar en `feature/software-configuration-management`._

#### 5.1.4 Software Deployment Configuration

> _Pendiente — completar en `feature/software-configuration-management`._

### 5.2 Landing Page, Services & Applications Implementation

#### 5.2.1 Sprint 1 (AV1)

##### 5.2.1.1 Sprint Planning 1
> _Pendiente._
##### 5.2.1.2 Aspect Leaders and Collaborators
> _Pendiente._
##### 5.2.1.3 Sprint Backlog 1
> _Pendiente._
##### 5.2.1.4 Development Evidence for Sprint Review
> _Pendiente._
##### 5.2.1.5 Execution Evidence for Sprint Review
> _Pendiente._
##### 5.2.1.6 Services Documentation Evidence for Sprint Review
> _Pendiente._
##### 5.2.1.7 Software Deployment Evidence for Sprint Review
> _Pendiente._
##### 5.2.1.8 Team Collaboration Insights during Sprint
> _Pendiente._

#### 5.2.2 Sprint 2 (TB1)

> _A completar a partir de la entrega TB1. Misma estructura que Sprint 1 (Planning, Aspect Leaders, Backlog, Development/Execution/Services/Deployment Evidence, Team Collaboration Insights)._

#### 5.2.3 Sprint 3 (AV2)

> _A completar a partir de la entrega AV2. Misma estructura que Sprint 1._

#### 5.2.4 Sprint 4 (TB2)

> _A completar a partir de la entrega TB2. Misma estructura que Sprint 1._

### 5.3 Validation Interviews

#### 5.3.1 Diseño de Entrevistas

> _Bloqueado — depende de tener un producto/prototipo validable (a partir de AV2)._

#### 5.3.2 Registro de Entrevistas

> _Bloqueado — depende de 5.3.1._

#### 5.3.3 Evaluaciones según heurísticas

> _Bloqueado — depende de 5.3.2. Usar el formato del Anexo D del enunciado._

### 5.4 Video About-the-Product

> _A completar a partir de AV2 (primera versión), versión final en TB2._

## Conclusiones

### Conclusiones y recomendaciones

> _Pendiente — sección acumulable, versión final en TB2._

### Video About-the-Team

> _A completar a partir de AV2 (primera versión), versión final en TB2._

## Bibliografía

> _Pendiente — agregar referencias en formato APA conforme se citen fuentes en cada sección._

## Anexos

### Anexo A. Videos de Exposiciones

| Entrega | Título del video | Enlace |
|---|---|---|
| AV1 | `[Pendiente]` | `[Pendiente]` |