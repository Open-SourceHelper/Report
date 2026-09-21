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

El Product Backlog de NeuroSync reúne las historias de usuario que describen las funcionalidades necesarias para desarrollar la plataforma. Cada historia identifica una necesidad específica desde la perspectiva del usuario o del equipo de desarrollo y cuenta con una estimación en Story Points.

A continuación, se presenta el Product Backlog del proyecto.

| **#** | **User Story ID** | **Título** | **Descripción** | **Story Points** |
|---|---|---|---|---|
| 1 | US01 | Visualización de propuesta de valor | Como visitante, deseo visualizar el propósito general de NeuroSync para entender cómo ayuda al cuidado de niños neurodivergentes. | 3 |
| 2 | US02 | Beneficios por segmento | Como visitante, deseo leer los beneficios segmentados para identificar la utilidad de la plataforma según mi rol (padre, cuidador o psicólogo). | 3 |
| 3 | US37 | Visualización de planes | Como usuario, quiero ver la tabla de precios (familiar vs. profesional) para elegir el esquema de suscripción adecuado. | 3 |
| 4 | US04 | Redirección a la aplicación web | Como visitante, deseo acceder a los enlaces de inicio de sesión o registro para transicionar desde la página informativa hacia el sistema operativo. | 2 |
| 5 | US38 | Pago de suscripción | Como usuario, quiero ingresar los datos de mi tarjeta para adquirir una suscripción premium mediante un servicio de terceros. | 8 |
| 6 | US09 | Perfil clínico del niño | Como cuidador autorizado, deseo consultar las necesidades y detonantes del niño para actuar correctamente frente a una desregulación. | 5 |
| 7 | US12 | Consulta de guía rápida | Como cuidador autorizado, deseo acceder a instrucciones paso a paso durante una crisis para intervenir de forma segura e inmediata. | 5 |
| 8 | US19 | Redacción de pautas clínicas | Como psicólogo autorizado, deseo redactar instrucciones formales de intervención para estandarizar la atención que brinda la familia. | 5 |
| 9 | US23 | Invitación a red de cuidado | Como padre o tutor, quiero invitar a un cuidador secundario mediante su correo para que acceda al perfil del niño. | 5 |
| 10 | US24 | Aceptación de invitación | Como cuidador secundario, quiero aceptar una invitación recibida para integrarme a la red de cuidado de un niño. | 3 |
| 11 | US15 | Creación de rutina | Como padre o psicólogo, deseo configurar una nueva secuencia de actividades asignando duración y orden para estructurar el día. | 5 |
| 12 | US13 | Visualización de rutina | Como cuidador, deseo visualizar la secuencia diaria con apoyos visuales para guiar al niño a través de sus actividades. | 5 |
| 13 | US17 | Registro de observación | Como cuidador, deseo registrar una observación o incidente ocurrido durante el día para notificar al psicólogo y a la familia. | 5 |
| 14 | US10 | Edición del perfil del niño | Como padre o tutor, deseo modificar el perfil clínico del menor para mantener los datos de apoyo actualizados para toda la red. | 5 |
| 15 | US18 | Visualización de red de cuidado | Como padre o tutor, deseo visualizar el listado de personas con acceso al perfil de mi hijo para auditar la privacidad de la información. | 3 |
| 16 | US25 | Revocación de accesos | Como padre o tutor, quiero eliminar a un integrante de la red de cuidado para proteger la privacidad del menor. | 5 |
| 17 | US26 | Visualización de pacientes | Como psicólogo, quiero visualizar un listado de todos mis pacientes vinculados para acceder rápidamente a sus pautas. | 3 |
| 18 | US08 | Panel principal (Dashboard) | Como cuidador autorizado, deseo visualizar un resumen de las rutinas diarias para identificar rápidamente las actividades programadas. | 5 |
| 19 | US11 | Búsqueda de guías prácticas | Como cuidador autorizado, deseo buscar pautas por categoría o situación para encontrar rápidamente la estrategia de apoyo necesaria. | 3 |
| 20 | US14 | Marcado de actividad completada | Como cuidador, deseo marcar una tarea como completada para registrar el progreso del niño a lo largo de su jornada. | 3 |
| 21 | US16 | Temporizador de transición | Como cuidador, deseo activar un temporizador visual para ayudar al niño a anticipar la transición hacia la siguiente tarea de la rutina. | 3 |
| 22 | US34 | Comentarios del psicólogo | Como psicólogo autorizado, quiero añadir un comentario en una observación registrada por la familia para brindar retroalimentación clínica. | 5 |
| 23 | US35 | Filtro de observaciones | Como psicólogo, quiero filtrar el historial de observaciones por tipo de evento (crisis, rutina, hito) para agilizar mi análisis. | 3 |
| 24 | US27 | Subida de apoyos visuales | Como padre o terapeuta, quiero subir imágenes o pictogramas personalizados para utilizarlos en las actividades de la rutina. | 5 |
| 25 | US32 | Categorización de crisis | Como cuidador, quiero etiquetar el nivel de intensidad de una desregulación sensorial registrada para generar un historial preciso. | 3 |
| 26 | US36 | Exportación de reporte | Como psicólogo, quiero exportar el historial de observaciones a un archivo PDF para adjuntarlo a la historia clínica del paciente. | 5 |
| 27 | US03 | Preguntas frecuentes | Como visitante, deseo consultar una sección de preguntas frecuentes para resolver dudas básicas sobre el manejo de la plataforma. | 2 |
| 28 | US39 | Cancelación de suscripción | Como usuario premium, quiero cancelar mi plan de pago mensual para evitar futuros cobros automatizados. | 5 |
| 29 | US05 | Formulario de registro | Como usuario no registrado, deseo crear una cuenta seleccionando mi rol para integrarme a la plataforma NeuroSync. | 5 |
| 30 | US06 | Validación de registro | Como usuario no registrado, deseo que el sistema valide mis datos de entrada para evitar errores en la creación de mi cuenta. | 3 |
| 31 | US07 | Inicio de sesión | Como usuario registrado, deseo autenticarme con mis credenciales para acceder a la información confidencial de la red de cuidado. | 5 |
| 32 | US22 | Cierre de sesión seguro | Como usuario autenticado, quiero cerrar mi sesión para proteger la privacidad de la información clínica. | 2 |
| 33 | US20 | Recuperación de contraseña | Como usuario registrado, quiero solicitar el restablecimiento de mi contraseña para recuperar el acceso a mi cuenta. | 5 |
| 34 | US21 | Edición de perfil de usuario | Como cuidador o psicólogo, quiero modificar mis datos personales para mantener mi información de contacto actualizada. | 3 |
| 35 | US28 | Duplicación de rutinas | Como padre o tutor, quiero duplicar una rutina existente para crear variaciones para diferentes días sin configurarla desde cero. | 3 |
| 36 | US29 | Eliminación de rutinas | Como padre o tutor, quiero eliminar una rutina que ya no se utiliza para mantener el panel organizado. | 3 |
| 37 | US30 | Marcado de actividad omitida | Como cuidador, quiero marcar una actividad como omitida para reflejar variaciones reales en el día del niño. | 2 |
| 38 | US31 | Configuración de alertas visuales | Como cuidador, quiero elegir el tipo de alerta del temporizador (solo visual o sonora leve) para evitar sobreestimulación. | 3 |
| 39 | US33 | Adjuntar evidencia visual | Como cuidador, quiero adjuntar una fotografía al registrar una observación para brindar mejor contexto al psicólogo. | 5 |
| 40 | US42 | Endpoint GET Perfil del Niño | Como Developer, deseo contar con un servicio REST para recuperar los datos terapéuticos del paciente. | 5 |
| 41 | US43 | Endpoint PUT Actualización Perfil | Como Developer, deseo tener un endpoint PUT para sobrescribir las preferencias y pautas de un perfil existente. | 5 |
| 42 | US49 | Endpoint POST Pautas Clínicas | Como Developer, deseo un endpoint para que el especialista guarde las directrices formales de intervención. | 5 |
| 43 | US50 | Endpoint POST Invitación Red | Como Developer, deseo un servicio que procese la lógica de vinculación entre un usuario nuevo y el paciente. | 8 |
| 44 | US51 | Endpoint DELETE Integrante Red | Como Developer, deseo un endpoint DELETE para eliminar los privilegios de un cuidador sobre un perfil. | 5 |
| 45 | US45 | Endpoint POST Crear Rutina | Como Developer, deseo un endpoint POST para registrar una nueva secuencia de actividades visuales en la base de datos. | 5 |
| 46 | US44 | Endpoint GET Rutinas | Como Developer, deseo implementar un servicio GET para listar las actividades diarias programadas. | 3 |
| 47 | US47 | Endpoint POST Observaciones | Como Developer, deseo un endpoint para insertar nuevos registros de observación en el historial clínico. | 5 |
| 48 | US48 | Endpoint GET Filtro de Observaciones | Como Developer, deseo implementar un servicio GET parametrizado para recuperar observaciones por rango de fechas. | 5 |
| 49 | US40 | Endpoint POST Registro de Usuario | Como Developer, deseo contar con un endpoint POST para almacenar de manera segura los datos del nuevo usuario en el sistema. | 5 |
| 50 | US41 | Endpoint POST Autenticación | Como Developer, deseo implementar un endpoint de login que genere un token de sesión seguro (JWT). | 8 |
| 51 | US46 | Endpoint DELETE Eliminar Rutina | Como Developer, deseo habilitar un endpoint DELETE para inactivar rutinas obsoletas. | 3 |
| 52 | US52 | Integración API Terceros | Como Developer, deseo conectar el sistema con un API de notificaciones push o mensajería. | 8 |

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