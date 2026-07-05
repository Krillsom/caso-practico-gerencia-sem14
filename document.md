# Propuesta Técnica



<div style="page-break-after: always;"></div>

## Contexto

### Antecedentes

El Instituto Nacional de Innovación Tecnológica (INITEC) es una entidad pública que administra 18 Centros Tecnológicos Regionales (CTR) distribuidos a nivel nacional. Cada centro gestiona cientos de activos tecnológicos —equipos de laboratorio, equipos industriales, vehículos, instrumentos de medición y equipos informáticos—, sumando aproximadamente 35,000 activos registrados en todo el país.

Actualmente, cada sede controla sus activos mediante hojas de cálculo, documentos de texto y registros físicos, sin ninguna herramienta que centralice o estandarice esta información entre los 18 centros.

### Problemática

La ausencia de un sistema centralizado ha generado, entre otros, los siguientes problemas:

- Mantenimientos preventivos que nunca se ejecutan.
- Pérdida del historial de mantenimiento de los activos.
- Duplicidad de información entre sedes.
- Ausencia de indicadores para la toma de decisiones.
- Inexistencia de trazabilidad sobre el ciclo de vida de los activos.
- Reportes elaborados manualmente, con el consiguiente riesgo de error y demora.

### Objetivo del proyecto

Ante este escenario, la Dirección Nacional de Tecnología ha decidido contratar a una empresa consultora para diseñar, desarrollar e implementar un Sistema Web de Gestión de Mantenimiento de Activos que centralice la información de los 18 centros tecnológicos, cubriendo:

- Inventario de activos.
- Mantenimiento preventivo, correctivo y predictivo.
- Programación de actividades.
- Historial de mantenimiento.
- Dashboard ejecutivo y reportes gerenciales.
- Gestión documental.
- Indicadores MTBF y MTTR.
- Gestión de incidencias.

### Alcance y condiciones del proyecto

SoftSolutions Consulting SAC presenta la presente Propuesta Técnica en el marco del proceso de selección convocado por INITEC, considerando las siguientes condiciones establecidas por el cliente:

- Duración del proyecto: seis (6) meses, con entregables mensuales.
- Modalidad de trabajo: híbrida.
- Cobertura: 18 sedes regionales, con usuarios finales distribuidos en distintas regiones del país.
- Naturaleza de la solución: aplicación web, implementada bajo un enfoque basado en el ciclo de vida de desarrollo de software, con entrega progresiva mediante productos parciales.


<div style="page-break-after: always;"></div>

## Enfoque Metodológico

### Enfoque seleccionado

SoftSolutions Consulting SAC propone abordar el presente proyecto bajo un **enfoque metodológico tradicional (predictivo)**, basado en un ciclo de vida secuencial de desarrollo de software, con planificación detallada desde el inicio y control formal de avance por fases.

### Justificación

La elección de un enfoque predictivo, en lugar de uno ágil o híbrido, responde a las características propias del proyecto y del cliente:

- **Naturaleza gubernamental de la entidad.** INITEC, como entidad pública, requiere procesos de contratación y seguimiento formales, con trazabilidad documental completa y rendición de cuentas ante organismos de control. Un enfoque predictivo facilita la generación de la documentación exigida en este tipo de contratos (actas, líneas base, informes de avance).
- **Alcance bien delimitado y cerrado.** El objetivo del sistema y sus módulos (inventario, mantenimiento preventivo/correctivo/predictivo, programación, historial, dashboard, reportes, gestión documental, indicadores MTBF/MTTR y gestión de incidencias) están definidos desde el caso y **no podrán modificarse ni reducirse** durante la ejecución, lo que elimina la necesidad de un descubrimiento iterativo del alcance propio de los enfoques ágiles.
- **Duración y contrato fijos.** El proyecto tiene una duración contractual establecida de seis meses, que no puede extenderse, y no se permite la contratación de personal externo adicional. Un enfoque predictivo permite planificar de manera determinística el uso de los recursos y del tiempo disponible frente a un alcance que no cambiará.
- **Entregables mensuales predecibles.** El esquema de entregas mensuales solicitado por el cliente se ajusta de forma natural a hitos y fases de un cronograma predictivo (levantamiento, análisis, diseño, construcción, pruebas, capacitación, implementación, puesta en producción y cierre), permitiendo un seguimiento claro del avance contra lo planificado.
- **Múltiples sedes con necesidades homogéneas.** Al tratarse de 18 centros con el mismo problema de fondo (falta de un sistema centralizado), los requerimientos pueden levantarse y consolidarse de forma integral al inicio del proyecto, sin necesidad de ciclos de retroalimentación continua por sede.


<div style="page-break-after: always;"></div>

## Metodología

Consistente con el enfoque tradicional declarado, la metodología de SoftSolutions Consulting SAC combina un estándar de ciclo de vida de software, un estándar de definición de necesidades del usuario y un marco de gestión de proyectos, de modo que el "qué" (procesos técnicos del software) y el "cómo se gestiona" (procesos de dirección de proyecto) queden claramente separados y trazables ante el comité evaluador:

<div style="page-break-after: always;"></div>

### ISO/IEC/IEEE 12207 — Procesos del Ciclo de Vida del Software

La ISO/IEC/IEEE 12207 organiza los procesos técnicos del ciclo de vida del software que sigue el proyecto. A continuación se detalla, por cada fase del proyecto, el proceso de la norma que la sustenta, sus actividades principales y su(s) entregable(s).

#### Levantamiento de Requerimientos

- **Proceso 12207 asociado:** Proceso de Definición de Requisitos, apoyado en ISO/IEC 25070 para la recolección estructurada de necesidades del usuario.
- **Actividades principales:** entrevistas y talleres con representantes de INITEC y de las 18 sedes; recopilación de necesidades sobre inventario, mantenimiento y reportes; consolidación de requisitos funcionales y no funcionales.
- **Entregable:**
  - Mapa de roles de usuario.
  - Documento de Requerimientos por tipo de usuario.

#### Análisis

- **Proceso 12207 asociado:** Proceso de Análisis de Requisitos del Sistema y del Software.
- **Actividades principales:** priorización de requisitos; modelado de los procesos de mantenimiento preventivo, correctivo y predictivo; validación de requisitos con el cliente.
- **Entregables:** Documento de Especificacion Funcional listo para desarrollo.

#### Diseño

- **Proceso 12207 asociado:** Procesos de Diseño de Arquitectura y Diseño Detallado.
- **Actividades principales:**
  - Definición de la arquitectura monolítica de la solución monolítica Java Servlet.
  - Diseño de la topología de red tipo estrella a distintos niveles, incluyendo la conectividad VPN entre las 18 sedes y el centro de datos.
  - Diseño del modelo de datos ERD.
  - Elaboración de diagramas de arquitectura C4 (contexto, contenedores, componentes).
  - Elaboración de diagramas de despliegue.
  - Diseño del cálculo de los indicadores MTBF y MTTR.
- **Entregables:**
  - Documento de Arquitectura y Diseño, incluyendo diagramas C4, diagrama de despliegue y diagrama de topología de red.

#### Construcción

- **Proceso 12207 asociado:** Proceso de desarrollo con programación.
- **Actividades principales:**
  - Desarrollo de los módulos:
    - Inventario
    - Mantenimiento
    - Programación de actividades
    - Reportes
    - Gestión documental
    - Gestión de incidencias
  - Gestión de código y artefactos de software.
- **Entregable:** Módulos de software construidos:
  - Inventario
  - Mantenimiento
  - Programación de actividades
  - Reportes
  - Gestión documental
  - Gestión de incidencias

#### Pruebas

- **Proceso 12207 asociado:** Procesos de Integración, Verificación y Validación.
- **Actividades principales:**
  - Pruebas unitarias.
  - Pruebas de integración.
  - Pruebas de aceptación de usuario.
- **Entregable:** Informe de resultados de pruebas.

#### Capacitación

- **Proceso 12207 asociado:** Proceso de Transición.
- **Actividades principales:** preparación de material de capacitación; sesiones de capacitación dirigidas a los usuarios finales de las 18 sedes.
- **Entregable:** Material de capacitación y actas de asistencia.

#### Implementación

- **Proceso 12207 asociado:** Proceso de Transición.
- **Actividades principales:**
  - Despliegue del sistema en el ambiente productivo.
  - Migración de datos desde las fuentes existentes en las 18 sedes:
    - Hojas de cálculo (Excel)
    - Documentos de texto (Word)
    - Registros físicos
- **Entregable:** Sistema desplegado en ambiente de producción.

#### Puesta en Producción

- **Proceso 12207 asociado:** Proceso de Operación.
- **Actividades principales:** acompañamiento post-despliegue; monitoreo inicial de la operación del sistema en las 18 sedes.
- **Entregable:** Acta de Puesta en Producción.


<div style="page-break-after: always;"></div>

### ISO/IEC 25070 — Definición de Necesidades del Usuario

La ISO/IEC 25070 (SQuaRE — Common Industry Format para la Definición de Necesidades del Usuario) se aplica durante el levantamiento de requerimientos del Proceso de Definición de Requisitos de la ISO/IEC 12207, estructurando la recolección de necesidades antes de pasar a Análisis. A continuación se detalla cada elemento de la norma aplicado al proyecto.

#### Contexto de Uso

- **Elemento CIF asociado:** Contexto de Uso.
- **Actividades principales:**
  - Identificación de los perfiles de usuario en las 18 sedes regionales (operadores de mantenimiento, encargados de sede, dirección nacional).
  - Descripción del entorno físico y tecnológico de uso: modalidad híbrida, conectividad VPN entre sedes y centro de datos, acceso vía navegador web.
- **Entregable:** Documento de Contexto de Uso.

#### Necesidades del Usuario

- **Elemento CIF asociado:** Necesidades del Usuario.
- **Actividades principales:**
  - Recolección de necesidades funcionales por módulo:
    - Inventario
    - Mantenimiento
    - Programación de actividades
    - Reportes
    - Gestión documental
    - Gestión de incidencias
  - Recolección de necesidades de calidad (disponibilidad, usabilidad, desempeño), insumo para la estrategia de aseguramiento de la calidad del proyecto.
- **Entregable:** Documento de Necesidades del Usuario.

#### Restricciones de Diseño e Implementación

- **Elemento CIF asociado:** Restricciones.
- **Actividades principales:**
  - Documentación de las restricciones contractuales: alcance fijo, duración fija de seis meses, sin contratación de personal externo adicional.
  - Documentación de las restricciones técnicas: arquitectura monolítica en Java sobre WildFly, balanceador de carga NGINX, conectividad VPN y topología de red en estrella.
- **Entregable:** Documento de Restricciones.

#### Validación de Necesidades

- **Elemento CIF asociado:** Validación con partes interesadas.
- **Actividades principales:**
  - Revisión conjunta del Documento de Necesidades del Usuario con representantes de INITEC.
  - Aprobación formal previa al inicio de la fase de Análisis.
- **Entregable:** Acta de Validación de Necesidades del Usuario.


<div style="page-break-after: always;"></div>

### PMBOK — Gestión del Proyecto

El PMBOK (PMI) aporta los grupos de procesos de dirección de proyectos que envuelven, de principio a fin, a las fases técnicas descritas en la ISO/IEC 12207. A continuación se detalla cada grupo de procesos aplicado al proyecto.

#### Inicio del Proyecto

- **Grupo de procesos PMBOK asociado:** Inicio.
- **Actividades principales:**
  - Elaboración del Acta de Constitución del Proyecto (Project Charter).
  - Identificación y registro de interesados (INITEC, las 18 sedes regionales, equipo consultor).
  - Confirmación del alcance, la duración de seis meses y las restricciones contractuales establecidas por el cliente.
- **Entregable:**
  - Acta de Constitución del Proyecto.
  - Registro de Interesados.

#### Planificación

- **Grupo de procesos PMBOK asociado:** Planificación.
- **Actividades principales:**
  - Elaboración del Plan de Gestión del Proyecto, integrando el plan de trabajo, la gestión de riesgos, el aseguramiento de la calidad y el plan de comunicación desarrollados en las demás secciones de esta propuesta.
  - Definición de las líneas base de alcance, cronograma y costo.
- **Entregable:** Plan de Gestión del Proyecto (línea base integrada).

#### Ejecución

- **Grupo de procesos PMBOK asociado:** Ejecución.
- **Actividades principales:**
  - Dirección y gestión del trabajo del proyecto durante las fases técnicas de Levantamiento de Requerimientos, Análisis, Diseño, Construcción, Pruebas, Capacitación e Implementación (ISO/IEC 12207).
  - Gestión y desarrollo del equipo de proyecto.
- **Entregable:** Entregables técnicos de cada fase (referenciados en ISO/IEC 12207).

#### Monitoreo y Control

- **Grupo de procesos PMBOK asociado:** Monitoreo y Control.
- **Actividades principales:**
  - Seguimiento del avance del cronograma y del presupuesto frente a la línea base.
  - Control integrado de cambios, dado que el contrato no permite modificar alcance ni duración.
  - Control de calidad de los entregables por fase.
- **Entregable:** Informes de desempeño del proyecto.

#### Cierre

- **Grupo de procesos PMBOK asociado:** Cierre.
- **Actividades principales:**
  - Entrega formal del sistema y de la documentación del proyecto a INITEC.
  - Recolección y documentación de lecciones aprendidas.
  - Cierre administrativo del contrato.
- **Entregable:** Acta de Cierre del Proyecto.


<div style="page-break-after: always;"></div>

## Restricciones

El proyecto se encuentra sujeto a estrictas limitaciones establecidas por INITEC que SoftSolutions Consulting SAC cumplirá a cabalidad:

- No se puede modificar el alcance original del proyecto.
- No se permite reducir las funcionalidades solicitadas del sistema.
- No se puede aumentar el tiempo del proyecto.
- La duración total del proyecto está fijada de manera inamovible en seis meses.
- Está prohibido contratar personal externo adicional al propuesto inicialmente.


<div style="page-break-after: always;"></div>

## Equipo

Para cumplir con los requerimientos, hemos conformado un equipo multidisciplinario.
| Rol | Persona | Funcionalidades |
|-|-|-|
| Director de proyecto | Álvaro Orozco | Gestión de interesados, control de alcance y cronograma. Entregables: Actas de reunión, Reportes gerenciales de avance. |
| Arquitecto de Software | Paolo Reaño | Diseño de la Arquitectura Hexagonal y topología de red. Entregables: Documento de Arquitectura de Software. |
| Especialista QA | Kevin Chi | QA: Aseguramiento de calidad funcional y no funcional. Entregables: Casos de prueba, Reportes de bugs. |
| Especialista DevOps | Por definir | DevOps: Gestión de infraestructura, pipelines CI/CD y automatización. Entregables: Ambientes configurados, Scripts de pase a producción. |
| Desarrollador Backend | Jesús Uribe | Construcción de APIs y lógica de negocio (Cálculos predictivos, MTBF/MTTR). Entregables: Código fuente backend documentado. |
| Desarrollador Frontend | Ángel Anampa | Creación del Dashboard ejecutivo y vistas del sistema web. Entregables: Código fuente frontend y componentes UI. |
| Analista funcional | Braulio Torrejón | Interacción con usuarios regionales para mapeo de procesos. Entregables: Historias de Usuario, Backlog del Producto. |


<div style="page-break-after: always;"></div>

## Gestión de Riesgos

La gestión de riesgos se realiza de forma continua a lo largo del proyecto: los riesgos se identifican, se analizan según su probabilidad e impacto, se priorizan y se les asigna una estrategia de respuesta y un responsable. El registro de riesgos se revisa en el comité de dirección mensual y en las retrospectivas de sprint, incorporando nuevos riesgos a medida que se detectan.

| Cód. | Riesgo | Prob. | Impacto | Estrategia de mitigación | Responsable |
|------|---------|-------|---------|--------------------------|-------------|
| R1 | Migración de ~35 000 activos con datos heterogéneos y de baja calidad | Alto | Alto | Proceso de migración por etapas con limpieza, validación y carga controlada; iniciar temprano con un piloto por sede. | Arquitecto / Dev. Backend |
| R2 | Dispersión geográfica de 18 sedes y problemas de conectividad | Media | Alto | Aplicación web con buenas prácticas de rendimiento; coordinación de accesos y ventanas; capacitaciones remotas. | Arquitecto / Director |
| R3 | Resistencia al cambio y baja adopción por parte de los usuarios | Media | Alto | Involucrar a usuarios clave desde el inicio, demos mensuales, plan de capacitación y acompañamiento. | Director / Analista |
| R4 | Baja calidad o inconsistencia de los datos de origen | Alta | Medio | Reglas de validación, saneamiento de datos y criterios de aceptación de la migración. | Analista / QA |
| R5 | Plazo fijo de seis meses frente a un alcance amplio | Alta | Alto | Priorización por valor del backlog, entregas incrementales y automatización de pruebas. | Director del Proyecto |
| R6 | Disponibilidad limitada de usuarios de las sedes para levantamiento y validación | Media | Medio | Acordar un calendario de disponibilidad y puntos de contacto por sede. | Director del Proyecto |
| R7 | Solicitudes de cambio que afecten el alcance o el cronograma | Media | Alto | Control de cambios formal; absorber ajustes menores mediante la repriorización del backlog. | Director del Proyecto |
| R8 | Seguridad de la información y protección de datos | Media | Alto | Controles de seguridad desde el diseño, gestión de accesos y pruebas de seguridad. | Arquitecto / QA / DevOps |
| R9 | Dependencia de la disponibilidad de ambientes e infraestructura | Media | Medio | Preparar ambientes de forma temprana con DevOps y acordar responsabilidades con el cliente. | DevOps / Director |


<div style="page-break-after: always;"></div>

## Plan de Trabajo



<div style="page-break-after: always;"></div>

## Aseguramiento de la Calidad del Proyecto

# 8. Aseguramiento de la calidad
## 8.1 Modelo de calidad (ISO/IEC 25010)
La estrategia de aseguramiento de la calidad se orienta por el modelo de calidad de producto de la norma ISO/IEC 25010, considerando de manera especial las características de adecuación funcional, eficiencia de desempeño (relevante por el volumen de aproximadamente 35 000 activos), compatibilidad, usabilidad, fiabilidad, seguridad, mantenibilidad y portabilidad. Para cada característica se definen criterios verificables que se incorporan a los criterios de aceptación de los entregables.
## 8.2 Estrategia de pruebas
La estrategia de pruebas es integral y se aplica de forma continua:
•	Pruebas unitarias durante el desarrollo.
•	Pruebas de integración entre componentes y servicios.
•	Pruebas de sistema sobre los flujos completos.
•	Pruebas de aceptación de usuario (UAT) con INITEC.
•	Pruebas de rendimiento y de carga, considerando el volumen de activos y de usuarios en distintas regiones.
•	Pruebas de seguridad y de control de accesos.
•	Pruebas de regresión automatizadas antes de cada entrega.
## 8.3 Prácticas de aseguramiento
Se aplican prácticas que aseguran la calidad de manera preventiva:
•	Definición de Terminado (Definition of Done) por historia y por sprint.
•	Revisiones de código y estándares de desarrollo.
•	Integración y despliegue continuo (CI/CD) con ejecución automática de pruebas.
•	Compuertas de calidad (quality gates) que deben superarse antes de cada puesta en producción.
## 8.4 Métricas y gestión de defectos
Se realiza seguimiento de métricas como la cobertura de pruebas, la densidad de defectos, el porcentaje de casos de prueba superados y el cumplimiento de los criterios de aceptación. Los defectos se registran, se clasifican por severidad y se gestionan mediante el tablero Kanban hasta su resolución y verificación. Ningún módulo pasa a producción sin haber superado las pruebas y las compuertas de calidad definidas.


<div style="page-break-after: always;"></div>

## Plan de Comunicación y Asignación de Roles (RACI)



<div style="page-break-after: always;"></div>

