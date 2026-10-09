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

### 2.3. Needfinding

El Needfinding es un proceso de investigación centrado en identificar y comprender las necesidades, motivaciones, dificultades y expectativas de los usuarios. Su propósito es reconocer los problemas que experimentan en su contexto cotidiano y recopilar información que permita orientar el diseño de una solución tecnológica centrada en el usuario.
En el proyecto NeuroSync, este proceso se enfoca en dos segmentos objetivo: las familias y cuidadores de niños de 3 a 12 años con condiciones del neurodesarrollo, como TEA, TDAH y síndrome de Down, y los psicólogos o terapeutas infantiles que participan en su acompañamiento.
A partir de la información recopilada durante las entrevistas, se emplean cuatro herramientas de análisis: **User Personas, User Task Matrix, User Journey Mapping y Empathy Mapping**. Estas permiten representar las características de los usuarios, identificar sus principales actividades, analizar las dificultades que enfrentan y comprender sus experiencias, emociones y expectativas.
Los resultados obtenidos servirán como base para identificar oportunidades de mejora y definir los requerimientos funcionales de Kinemo, una plataforma web orientada a facilitar la organización de rutinas, el acceso a guías prácticas y la coordinación entre familias, cuidadores y profesionales autorizados.

#### 2.3.1 User Personas

> _Pendiente — completar en `feature/user-personas`._

#### 2.3.2 User Task Matrix

> _Pendiente — completar en `feature/user-task-matrix`._

#### 2.3.3 User Journey Mapping

> _Pendiente — completar en `feature/journey-maps`._

#### 2.3.4 Empathy Mapping

> _Pendiente — completar en `feature/empathy-maps`._


### 2.4. Big Picture Event Storming

El equipo llevó a cabo una sesión colaborativa de Big Picture Event Storming con el objetivo de comprender de manera integral el dominio de negocio de NeuroSync y los principales procesos que soportará la plataforma Kinemo. La dinámica se realizó de forma remota utilizando un board colaborativo en Miro, donde los miembros del equipo, tomando como insumo las necesidades identificadas previamente en las User Stories, fueron colocando notas de color naranja representando los hechos relevantes (Domain Events) que ocurren dentro del negocio, redactados en pasado y sin orden predefinido, siguiendo la técnica de "storm" característica de esta dinámica.

La sesión se organizó en dos pasos principales: primero la recopilación libre de eventos y, posteriormente, el refinamiento de los mismos para distinguir los verdaderos eventos de dominio de acciones de consulta.

**Paso 1 – Recopilación de Domain Events**

Durante esta primera etapa, el equipo se enfocó en generar la mayor cantidad de eventos posibles sin filtrar ni discutir su validez, cubriendo las principales funcionalidades identificadas en el backlog: identidad y acceso, perfil del niño, red de cuidado, rutinas y actividades, orientación clínica, observaciones y crisis, dashboard y reportes, y suscripciones y pagos.

Como resultado de esta recopilación libre se identificaron 42 eventos distribuidos en las ocho áreas funcionales mencionadas, agrupados visualmente en el board mediante clusters horizontales por color de post-it.

**Paso 2 – Refinamiento de Domain Events**

En la segunda etapa, el equipo revisó cada uno de los eventos recopilados para diferenciar los verdaderos Domain Events (cambios de estado relevantes para el negocio) de acciones que en realidad correspondían a consultas (Queries), como visualizar un perfil, visualizar una rutina, consultar una guía o filtrar observaciones.

Estos últimos fueron descartados del listado de eventos y quedaron marcados para ser retomados posteriormente como Queries en el Design-Level Event Storming.

Asimismo, se discutió y acordó que la Landing Page y la API RESTful no constituyen Bounded Contexts independientes, sino una superficie pública de interacción y una interfaz técnica de acceso a las capacidades del dominio, respectivamente.

Como resultado de este refinamiento, los eventos válidos quedaron agrupados en ocho clusters que sentaron la base para la posterior identificación de Bounded Contexts en el Design-Level Event Storming:

1. Identity & Access Management
2. Child Profile Management
3. Care Network Management
4. Routine & Activity Management
5. Clinical Guidance Management
6. Observation & Crisis Management
7. Dashboard & Reporting
8. Subscription & Payment Management

**Enlace del Big Picture Event Storming:**

[Ver diagrama en Miro](https://miro.com/app/board/uXjVHkkYYow=/?share_link_id=268152052434)


### 2.5. Ubiquitous Language

El Ubiquitous Language de Kinemo establece un vocabulario común para representar los principales conceptos del dominio de NeuroSync. Los términos definidos a continuación serán utilizados de manera consistente por los integrantes del equipo para describir las necesidades del negocio, las historias de usuario, los procesos identificados mediante Event Storming y, posteriormente, el diseño de la solución.

**Neurodivergent Child**

Niño de entre 3 y 12 años que forma parte del contexto de atención de Kinemo y presenta una condición del neurodesarrollo como TEA, TDAH o síndrome de Down.

**Child Profile**

Conjunto de información del niño que permite a la red de cuidado conocer sus características, necesidades y formas de apoyo. Incluye información como preferencias, reguladores y detonantes.

**Parent / Guardian**

Padre o tutor responsable del niño dentro de Kinemo. Puede administrar información del perfil, gestionar integrantes de la red de cuidado y configurar determinados recursos utilizados para el acompañamiento.

**Caregiver**

Persona que participa directamente en el cuidado cotidiano del niño. Puede consultar el perfil autorizado, ejecutar rutinas, utilizar guías de apoyo y registrar observaciones sobre situaciones ocurridas durante el día.

**Psychologist**

Profesional autorizado que acompaña al niño desde el ámbito psicológico y puede consultar pacientes vinculados, redactar pautas clínicas, revisar observaciones y proporcionar retroalimentación a la familia.

**Care Network**

Conjunto de personas vinculadas al perfil de un niño que participan en su cuidado. Puede estar conformada por padres, tutores, cuidadores secundarios y profesionales autorizados.

**Care Network Member**

Persona que forma parte de la red de cuidado de un niño y posee determinados permisos para acceder a su información de acuerdo con su participación en el cuidado.

**Care Invitation**

Invitación enviada por un padre o tutor a otra persona para incorporarla a la red de cuidado del niño.

**Care Access**

Permiso otorgado a un integrante de la red de cuidado para acceder a la información del perfil del niño. Este acceso puede ser otorgado o revocado por el responsable correspondiente.

**Patient**

Niño vinculado a la cuenta de un psicólogo dentro de su relación profesional de atención. El profesional puede consultar los pacientes asociados para acceder a sus pautas y observaciones.

**Trigger**

Detonante identificado en el perfil del niño que puede provocar o contribuir a una situación de desregulación. Su conocimiento permite a los cuidadores anticipar determinadas situaciones y actuar de acuerdo con las pautas establecidas.

**Regulator**

Recurso, estrategia o elemento identificado como útil para favorecer la regulación del niño frente a determinadas situaciones.

**Sensory Dysregulation**

Situación en la que el niño presenta dificultades para regularse frente a determinados estímulos o circunstancias y requiere la aplicación de estrategias de apoyo.

**Crisis**

Situación de desregulación que requiere que el cuidador consulte y aplique una guía de intervención adecuada según las características y necesidades del niño.

**Crisis Severity**

Nivel de intensidad asignado a una desregulación registrada. Kinemo contempla los niveles Leve, Moderado y Severo para organizar el historial de observaciones y facilitar su análisis posterior.

**Practical Guide**

Guía de apoyo que contiene instrucciones organizadas para orientar al cuidador frente a una determinada situación o necesidad del niño.

**Clinical Guideline**

Directriz formal de intervención redactada por un psicólogo o profesional autorizado y asociada al niño para que pueda ser consultada por los cuidadores responsables de su acompañamiento.

**Routine**

Secuencia estructurada de actividades organizada para establecer y mantener la jornada cotidiana del niño.

**Activity**

Acción individual que forma parte de una rutina. Cada actividad puede tener un orden y una duración estimada dentro de la secuencia diaria.

**Visual Support**

Imagen o pictograma personalizado utilizado para representar una actividad y facilitar su comprensión durante la ejecución de una rutina.

**Transition**

Cambio de una actividad hacia la siguiente dentro de una rutina. Kinemo permite anticipar este cambio mediante un temporizador.

**Transition Timer**

Temporizador utilizado durante una rutina para ayudar al niño a anticipar el cambio hacia la siguiente actividad.

**Visual Alert**

Señal utilizada para comunicar al cuidador o al niño la finalización de un temporizador sin generar una sobreestimulación innecesaria. Puede configurarse para utilizar únicamente señales visuales o incluir una señal sonora leve.

**Observation**

Registro realizado por un cuidador sobre una situación, incidente o hecho relevante ocurrido durante el cuidado cotidiano del niño. La observación queda asociada al niño, al autor y a la fecha correspondiente.

**Incident**

Situación ocurrida durante el día del niño que puede ser registrada mediante una observación para dejar constancia de lo sucedido y facilitar su seguimiento.

**Evidence**

Fotografía u otro soporte visual asociado a una observación para aportar mayor contexto sobre la situación registrada.

**Psychologist Comment**

Retroalimentación registrada por un psicólogo autorizado sobre una observación realizada por la familia o los cuidadores.

**Observation History**

Conjunto de observaciones registradas sobre el niño que permite consultar y analizar situaciones ocurridas a lo largo del tiempo.

**Premium Subscription**

Modalidad de suscripción de pago que permite acceder a las funcionalidades premium de Kinemo.

**Subscription Plan**

Esquema de suscripción ofrecido por Kinemo que define las características y condiciones asociadas al servicio. El usuario puede revisar las opciones disponibles antes de seleccionar una.

**Payment**

Transacción realizada por el usuario para adquirir o mantener una suscripción premium mediante un servicio de terceros.

**Billing Cycle**

Periodo asociado a la vigencia de una suscripción. En una cancelación, el servicio permanece disponible hasta finalizar el ciclo de facturación vigente.

**Subscription Cancellation**

Solicitud realizada por un usuario premium para finalizar su suscripción y evitar futuros cobros automatizados al terminar el ciclo de facturación actual.

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

#### 4.7.1 Class Diagrams

> _Pendiente — completar en `feature/class-diagrams`._

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