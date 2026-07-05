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
