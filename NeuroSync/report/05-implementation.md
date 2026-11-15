## Capítulo V: Product Implementation, Validation & Deployment

### 5.1 Software Configuration Management

En esta sección se describen las herramientas, convenciones y procedimientos utilizados por el equipo de NeuroSync para gestionar el desarrollo e implementación de Kinemo. Se documentan los entornos de trabajo empleados para diseño, desarrollo, control de versiones, documentación y despliegue, buscando mantener una forma de trabajo uniforme entre todos los integrantes del equipo.

Asimismo, se establecen las convenciones para la gestión del código fuente, los estándares de desarrollo y la configuración prevista para el despliegue de los diferentes productos que conforman la solución: Landing Page, Web Application y RESTful Web Services.

#### 5.1.1 Software Development Environment Configuration

### Project Management

Para la gestión y organización de las actividades del proyecto se emplea GitHub como plataforma principal de colaboración. Mediante los repositorios de la organización del equipo se realiza el seguimiento de los cambios efectuados en los productos de software y se mantiene la trazabilidad de las contribuciones realizadas por cada integrante durante los sprints.

Adicionalmente, las tareas del Sprint son organizadas mediante un tablero de trabajo que permite identificar las actividades pendientes, en progreso y completadas.

### Software Development

Para el desarrollo de la Landing Page de Kinemo se utilizan HTML5, CSS3 y JavaScript, tecnologías adecuadas para implementar un sitio web estático, responsive y accesible.

La Web Application se plantea como una Single-Page Application desarrollada utilizando Angular y TypeScript, mientras que los RESTful Web Services serán implementados posteriormente mediante Spring Boot y Java.

### Software Documentation

Para la documentación de los RESTful Web Services se utilizará OpenAPI/Swagger, permitiendo documentar y probar de manera interactiva los endpoints desarrollados durante los siguientes sprints.

Para los diagramas de arquitectura se utilizan herramientas como Structurizr y Miro, mientras que los diagramas de flujo y determinados artefactos visuales se desarrollan mediante Lucidchart.

### Software Deployment

Para el despliegue inicial de la Landing Page se utilizará GitHub Pages, debido a que permite publicar directamente sitios web estáticos almacenados en repositorios GitHub.

El despliegue de la Web Application y de los RESTful Web Services será definido e implementado durante los siguientes sprints, conforme avance el desarrollo funcional de la plataforma.

### Version Control

Para el almacenamiento y control de versiones del código fuente se utiliza Git, gestionado mediante GitHub, dentro de la organización del equipo:

**Organización GitHub:**

[https://github.com/orgs/Open-SourceHelper/repositories](https://github.com/orgs/Open-SourceHelper/repositories)

El equipo utilizará un flujo de trabajo basado en ramas para separar el código estable de las funcionalidades que se encuentren en desarrollo. Asimismo, los mensajes de commit seguirán el estándar Conventional Commits, buscando mantener una trazabilidad clara sobre la naturaleza de cada modificación.

#### 5.1.2 Source Code Management


El equipo NeuroSync utiliza GitHub como plataforma principal para el control de versiones y colaboración durante el desarrollo de Kinemo. Los distintos productos que conforman la solución se administran mediante repositorios pertenecientes a la organización:

**GitHub Organization:**

[https://github.com/orgs/Open-SourceHelper/repositories](https://github.com/orgs/Open-SourceHelper/repositories)

| Producto | Repositorio |
|----------|-------------|
| Startup / Project Report | Report |
| Landing Page | Report |
| Frontend Web Application | Report |
| RESTful Web Services | Report |

Para la gestión del código fuente se adopta un flujo de trabajo basado en GitFlow, separando las diferentes etapas de desarrollo mediante ramas específicas:

- **main:** Rama estable destinada al código preparado para producción y despliegue.
- **develop:** Rama de integración en la cual se consolidan las funcionalidades terminadas antes de incorporarlas a producción.
- **feature/:** Ramas utilizadas para desarrollar funcionalidades específicas relacionadas con User Stories o tareas del Sprint.

Las ramas `feature/` parten de `develop` y, una vez completado el trabajo, se integran nuevamente mediante Pull Requests.

### Conventional Commits

Los mensajes de commit seguirán el estándar Conventional Commits utilizando principalmente los siguientes prefijos:

| Prefijo | Uso |
|---------|-----|
| **feat:** | Nueva funcionalidad |
| **fix:** | Corrección de error |
| **docs:** | Cambios de documentación |
| **style:** | Cambios visuales o de formato |
| **refactor:** | Reestructuración sin cambiar comportamiento |
| **test:** | Pruebas |
| **chore:** | Configuración y mantenimiento |

La captura evidencia la estructura de ramas utilizada durante el desarrollo, permitiendo distinguir el código estable y las ramas empleadas por los integrantes para implementar las funcionalidades asignadas.

#### 5.1.3 Source Code Style Guide & Coding Conventions


Esta sección establece los estándares de codificación que serán utilizados durante el desarrollo de Kinemo con el objetivo de mantener consistencia, legibilidad y mantenibilidad en todo el proyecto. Las convenciones se aplicarán de acuerdo con las tecnologías empleadas en la Landing Page, Web Application y RESTful Web Services.

### Principios generales

- Todo el código y los identificadores se escribirán en inglés.
- Se utilizarán nombres descriptivos.
- Se evitará duplicar código.
- Cada función y componente deberá mantener una responsabilidad claramente definida.
- Se mantendrá una estructura uniforme entre archivos del mismo tipo.
- La indentación será consistente en todo el proyecto.

### Nomenclatura

| Elemento | Convención | Ejemplo |
|----------|------------|---------|
| Variables | camelCase | `childProfile` |
| Funciones | camelCase | `getDailyRoutine()` |
| Clases | PascalCase | `ChildProfile` |
| Interfaces | PascalCase | `CareNetwork` |
| Constantes | UPPER_SNAKE_CASE | `API_URL` |
| Archivos web | kebab-case | `child-profile.component.ts` |
| Clases CSS | kebab-case | `routine-card` |

### HTML

Se utilizarán etiquetas semánticas de HTML5 como `header`, `nav`, `main`, `section`, `article` y `footer`. Las etiquetas se escribirán en minúsculas y se utilizará una indentación uniforme.

### CSS

Las clases CSS utilizarán nombres descriptivos escritos en kebab-case. Se priorizará la reutilización de estilos y el uso de variables CSS para elementos recurrentes como colores, tipografías y espaciados.

### JavaScript

Se utilizarán `const` y `let`, evitando `var`. Las funciones deberán mantener una responsabilidad concreta y utilizar nombres descriptivos relacionados con la acción realizada.

### TypeScript / Angular

TypeScript utilizará tipado explícito siempre que sea posible, evitando el uso innecesario de `any`. En Angular se utilizarán componentes reutilizables, servicios para la lógica compartida y separación de responsabilidades por funcionalidades.

### Java / Spring Boot

Para el backend, las clases utilizarán PascalCase y los métodos camelCase. La solución seguirá una estructura organizada en Controller, Application/Service, Domain y Repository, coherente con los Bounded Contexts definidos para Kinemo.

#### 5.1.4 Software Deployment Configuration


Esta sección describe la configuración utilizada para publicar los productos digitales de Kinemo. Para el primer Sprint, el despliegue se concentra en la Landing Page, desarrollada mediante HTML5, CSS3 y JavaScript.

### Landing Page

| Elemento | Tecnología |
|----------|------------|
| Estructura | HTML5 |
| Estilos | CSS3 |
| Interactividad | JavaScript |
| Version Control | Git / GitHub |
| Hosting | GitHub Pages |

### 5.2 Landing Page, Services & Applications Implementation

En esta sección se documenta el proceso de implementación de los productos digitales que conforman Kinemo. Para el primer avance del proyecto se registra el trabajo correspondiente al Sprint 1, concentrado principalmente en la implementación y despliegue de la Landing Page y en el establecimiento de las bases necesarias para el desarrollo de los productos posteriores.

#### 5.2.1 Sprint 1

El Sprint 1 constituye la primera iteración de implementación de Kinemo. Durante este periodo, el equipo transforma los primeros requerimientos y diseños del producto en una versión funcional de la Landing Page.
El alcance prioriza las funcionalidades públicas necesarias para comunicar la propuesta de valor de NeuroSync, explicar los beneficios de Kinemo a sus diferentes segmentos de usuario, presentar los planes disponibles y facilitar la transición desde la página pública hacia la futura Web Application.

##### 5.2.1.1 Sprint Planning 1

| Campo | Información |
|-------|-------------|
| **Sprint #** | Sprint 1 |
| **upDate** | [fecha real de su reunión] |
| **Time** | [hora] |
| **Location** | Reunión virtual |
| **Prepared By** | [integrante responsable] |
| **Attendees** | Felipe Huamanchumo, Gabriel Vilchez, Fabricio Flores, Matthew Shinko Okuhama Diaz, Cristian Trigoso |

### Sprint 0 Review Summary

Al tratarse del primer Sprint del proyecto, no existe una iteración de implementación anterior que deba ser revisada. El equipo parte de los requerimientos, User Stories, Product Backlog y artefactos de diseño desarrollados durante las etapas iniciales de análisis y diseño del producto.

### Sprint 0 Retrospective Summary

Al no existir un Sprint anterior, no corresponde realizar una retrospectiva formal. Sin embargo, el equipo llevó a cabo coordinaciones iniciales para definir herramientas de colaboración, distribución de responsabilidades, organización del código fuente y criterios de desarrollo.

### Sprint Goal

Implementar y desplegar la primera versión funcional y responsive de la Landing Page de Kinemo, permitiendo comunicar la propuesta de valor, los beneficios para cada segmento objetivo, las preguntas frecuentes, los planes de suscripción y el acceso hacia la Web Application.

| Campo | Valor |
|-------|-------|
| **Sprint 1 Velocity** | 13 Story Points |
| **Sum of Story Points** | 13 Story Points |

##### 5.2.1.2 Aspect Leaders and Collaborators

En esta sección se presenta la matriz de liderazgo y colaboración correspondiente al Sprint 1. Su propósito es identificar a los integrantes responsables de liderar cada aspecto del desarrollo y a aquellos que participaron como colaboradores.

Para este Sprint se consideran tres aspectos principales: Landing Page, UX/UI & Responsive Design y GitHub & Deployment.

| Team Member | GitHub Username | Landing Page | UX/UI & Responsive | GitHub & Deployment |
|-------------|-----------------|--------------|---------------------|---------------------|
| Huamanchumo Chicchon, Felipe Marcelo | Ferdwar | L/C | L/C | L/C |
| Vilchez Vite, Gabriel Alejandro | GZ-99 | L/C | L/C | L/C |
| Flores Chavez, Fabricio | Elmiau2341 | L/C | L/C | L/C |
| Shinko Okuhama Diaz, Matthew | okudiaz124 | L/C | L/C | L/C |
| Trigoso Garrido, Cristian Joseph | Crzzz30 | L/C | L/C | L/C |

##### 5.2.1.3 Sprint Backlog 1

El Sprint Backlog 1 reúne las tareas necesarias para implementar las User Stories priorizadas para la primera versión de la Landing Page de Kinemo. El trabajo se concentra en presentar la propuesta de valor, los beneficios según el tipo de usuario, preguntas frecuentes, acceso hacia la aplicación web y los planes disponibles.

### US01 – Visualización de propuesta de valor

| Task ID | Title | Description | Estimation | Assigned To | Status |
|---------|-------|-------------|------------|-------------|--------|
| T001 | Estructura base HTML | Crear la estructura semántica principal de la Landing Page. | 3h | [Asignado] | Done |
| T002 | Hero Section | Implementar el título, descripción y CTA principal de Kinemo. | 3h | [Asignado] | Done |
| T003 | Estilos del Hero | Aplicar tipografía, colores y distribución responsive. | 3h | [Asignado] | Done |

### US02 – Beneficios por segmento

| Task ID | Title | Description | Estimation | Assigned To | Status |
|---------|-------|-------------|------------|-------------|--------|
| T004 | Cards de segmentos | Crear tarjetas para Padre/Tutor, Cuidador y Psicólogo. | 4h | [Asignado] | Done |
| T005 | Contenido por rol | Incorporar los beneficios específicos de cada segmento. | 3h | [Asignado] | Done |
| T006 | Diseño responsive | Adaptar las tarjetas para móvil, tablet y desktop. | 3h | [Asignado] | Done |

### US03 – Preguntas frecuentes

| Task ID | Title | Description | Estimation | Assigned To | Status |
|---------|-------|-------------|------------|-------------|--------|
| T007 | Estructura FAQ | Crear el listado de preguntas y respuestas frecuentes. | 3h | [Asignado] | Done |
| T008 | Interacción del FAQ | Implementar expansión y colapso de las respuestas mediante JavaScript. | 3h | [Asignado] | Done |

### US04 – Redirección a la aplicación web

| Task ID | Title | Description | Estimation | Assigned To | Status |
|---------|-------|-------------|------------|-------------|--------|
| T009 | CTA de acceso | Implementar botones para acceder o registrarse en Kinemo. | 2h | [Asignado] | Done |
| T010 | Configuración de enlaces | Configurar la redirección hacia la futura Web Application. | 2h | [Asignado] | Done |

### US37 – Visualización de planes

| Task ID | Title | Description | Estimation | Assigned To | Status |
|---------|-------|-------------|------------|-------------|--------|
| T011 | Sección de planes | Implementar las tarjetas correspondientes a los planes Familiar y Profesional. | 4h | [Asignado] | Done |
| T012 | Estilos de planes | Aplicar la identidad visual de Kinemo a las tarjetas de precios. | 3h | [Asignado] | Done |
| T013 | Responsive de planes | Adaptar la sección de planes a diferentes tamaños de pantalla. | 2h | [Asignado] | Done |

Las historias seleccionadas para este Sprint corresponden a funcionalidades públicas de la Landing Page, incluyendo la propuesta de valor, los beneficios por segmento, FAQ, redirección hacia la aplicación y visualización de planes.

##### 5.2.1.4 Development Evidence for Sprint Review


Durante el Sprint 1, el equipo NeuroSync avanzó en la implementación de la primera versión funcional de la Landing Page de Kinemo, desarrollada mediante HTML5, CSS3 y JavaScript.

Los principales avances estuvieron relacionados con la implementación de la estructura principal de la página, la presentación de la propuesta de valor, los beneficios para los distintos segmentos objetivo, la sección de preguntas frecuentes, los planes de suscripción y la adaptación responsive para diferentes dispositivos.

Para mantener la trazabilidad del desarrollo, los cambios realizados fueron registrados mediante commits dentro del repositorio correspondiente.

| Repository | Branch | Commit ID | Commit Message | Committed On |
|------------|--------|-----------|----------------|--------------|
| [Repositorio] | [Branch] | [SHA] | [Commit real] | [Fecha] |
| [Repositorio] | [Branch] | [SHA] | [Commit real] | [Fecha] |
| [Repositorio] | [Branch] | [SHA] | [Commit real] | [Fecha] |
| [Repositorio] | [Branch] | [SHA] | [Commit real] | [Fecha] |

Aquí se deben colocar los commits reales obtenidos desde GitHub, indicando repositorio, rama, identificador del commit, mensaje y fecha.

##### 5.2.1.5 Execution Evidence for Sprint Review

Durante el Sprint 1 se implementó la primera versión navegable y responsive de la Landing Page de Kinemo.
La interfaz permite al visitante conocer la propuesta de valor del producto, identificar los beneficios disponibles para padres, cuidadores y psicólogos, comprender el funcionamiento general de la solución, consultar preguntas frecuentes y revisar las alternativas de suscripción disponibles.
La navegación se organiza mediante diferentes secciones dentro de una misma página, permitiendo al usuario desplazarse fácilmente hacia el contenido de interés. Asimismo, la interfaz fue adaptada para mantener una correcta visualización en dispositivos desktop, tablet y móvil.
A continuación se presentan las principales evidencias de ejecución de la Landing Page:
Evidencia 1: Hero Section
La sección principal presenta la propuesta de valor de Kinemo y una llamada a la acción que permite al visitante conocer cómo funciona la solución.

> _Pendiente._

##### 5.2.1.6 Services Documentation Evidence for Sprint Review

Durante el Sprint 1, el alcance de implementación estuvo enfocado principalmente en el desarrollo y despliegue de la primera versión de la Landing Page de Kinemo.
En consecuencia, durante esta iteración todavía no se realizó la implementación de los RESTful Web Services ni de los endpoints correspondientes al backend de la solución.
Por este motivo, no existe documentación mediante OpenAPI/Swagger que deba ser presentada como evidencia en este Sprint.
La documentación de los servicios será incorporada durante los siguientes Sprints, cuando se inicie la implementación de la RESTful API utilizando Spring Boot y Java.
La arquitectura planteada para Kinemo considera una RESTful API desarrollada con Spring Boot y Java, la cual posteriormente expondrá las capacidades de los diferentes Bounded Contexts.

##### 5.2.1.7 Software Deployment Evidence for Sprint Review

> _Pendiente._

##### 5.2.1.8 Team Collaboration Insights during Sprint

> _Pendiente._

#### 5.2.1 Sprint 1 (AV1)

> _Pendiente._

##### 5.2.2.1.Sprint Planning 2.

> _Pendiente._

##### 5.2.2.2. Aspect Leaders and Collaborators.

> _Pendiente._

##### 5.2.2.3.Sprint Backlog 2.

> _Pendiente._

##### 5.2.2.4.Development Evidence for Sprint Review.

> _Pendiente._

##### 5.2.2.5.Execution Evidence for Sprint Review.

> _Pendiente._

##### 5.2.2.6.Services Documentation Evidence for Sprint Review.

> _Pendiente._

##### 5.2.2.7.Software Deployment Evidence for Sprint Review.

> _Pendiente._

##### 5.2.2.8.Team Collaboration Insights during Sprint.

> _Pendiente._

**BC06 — Observation & Crisis Management**

Durante el Sprint 2 se implementaron y probaron los servicios del bounded context Observation & Crisis Management, utilizando Angular para el frontend y json-server como API REST simulada.

Se realizaron solicitudes HTTP GET y POST para verificar el registro y la consulta de observaciones, los comentarios de psicólogos y los enlaces de evidencias asociados a cada observación.

Las siguientes capturas muestran las pruebas realizadas mediante las herramientas de desarrollo del navegador.

**Evidencia 1. Consulta de evidencias de observación**

![Consulta de evidencias de observación](NeuroSync/assets/img/5_2_2_8-team-collaboration-insights-during-sprint/1.JPG)

*Figura 1. Consulta de evidencias asociadas a una observación mediante GET /observationEvidences.*

Se muestra la respuesta de la API simulada, incluyendo el identificador de la evidencia, nombre, enlace URL y fecha de registro.

**Evidencia 2. Registro de observaciones mediante HTTP POST**

![Registro de observaciones](NeuroSync/assets/img/5_2_2_8-team-collaboration-insights-during-sprint/2.JPG)

*Figura 2. Solicitud POST /observations.*

La respuesta HTTP 201 Created confirma que json-server creó correctamente una nueva observación.

**Evidencia 3. Datos enviados en la solicitud POST**

![Datos de la solicitud POST](NeuroSync/assets/img/5_2_2_8-team-collaboration-insights-during-sprint/3.JPG)

*Figura 3. Cuerpo JSON enviado para registrar una observación.*

La solicitud contiene los identificadores del niño y del cuidador, la descripción, fecha de ocurrencia e intensidad de crisis.

**Evidencia 4. Evidencia adicional del servicio**

![Evidencia adicional del servicio](NeuroSync/assets/img/5_2_2_8-team-collaboration-insights-during-sprint/4.JPG)

*Figura 4. Evidencia de ejecución de los servicios del BC06.*

**Evidencia 5. Evidencia complementaria**

![Evidencia complementaria](NeuroSync/assets/img/5_2_2_8-team-collaboration-insights-during-sprint/5.JPG)

*Figura 5. Evidencia complementaria de las pruebas HTTP del BC06.*

**Evidencia 6. Verificación de servicios**

![Verificación de servicios](NeuroSync/assets/img/5_2_2_8-team-collaboration-insights-during-sprint/6.JPG)

*Figura 6. Verificación de las operaciones del BC06 mediante la API simulada.*

**Resultado de las pruebas**

Las pruebas realizadas permitieron verificar la comunicación HTTP entre Angular y json-server, así como las operaciones de consulta y registro de información correspondientes al BC06.

Estas evidencias corresponden a un entorno local de desarrollo. No representan pruebas de un backend Spring Boot desplegado ni de autenticación real de usuarios.

##### 5.2.2 Sprint 2 (TB1)

> _Pendiente._

##### 5.2.2.1. Sprint Planning 2

> _Pendiente._

##### 5.2.2.2 Aspect Leaders and Collaborators

> _Pendiente._

##### 5.2.2.3 Sprint Backlog 2

> _Pendiente._

##### 5.2.2.4 Development Evidence for Sprint Review

> _Pendiente._

##### 5.2.2.5 Execution Evidence for Sprint Review

> _Pendiente._

##### 5.2.2.6 Testing Evidence for Sprint Review

> _Pendiente._

##### 5.2.2.7 Software Deployment Evidence for Sprint Review

> _Pendiente._

##### 5.2.2.8 Team Collaboration Insights during Sprint

> _Pendiente._
