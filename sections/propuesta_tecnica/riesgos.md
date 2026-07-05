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
