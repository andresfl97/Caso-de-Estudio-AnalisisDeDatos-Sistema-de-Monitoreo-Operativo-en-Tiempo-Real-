## 🔒 Políticas de Confidencialidad y Gobierno de Datos (Cumplimiento LOPDP Ecuador)

Con el fin de garantizar el secreto profesional, la protección de la propiedad intelectual de la organización y el estricto cumplimiento del marco legal ecuatoriano, toda la información sensible contenida en este repositorio ha sido sometida a un proceso técnico de **anonimización y seudonimización**. 

Este tratamiento se sustenta legalmente en la **Ley Orgánica de Protección de Datos Personales (LOPDP)** de la República del Ecuador, bajo los siguientes lineamientos:

* **Cumplimiento del Principio de Confidencialidad (Art. 10 - LOPDP):** Toda métrica de rendimiento operativo, tiempos de respuesta y evaluaciones de desempeño técnico corresponden a la esfera interna de la organización y sus contratistas. En virtud del deber de secreto, se omiten los nombres reales de la empresa y sus proveedores, enmascarándolos bajo etiquetas neutrales (*Contratista A / Contratista B*).
* **Aplicación del Principio de Seguridad de Datos y Anonimización (Art. 11 - LOPDP):** Los datos numéricos, volumétricos y geográficos presentados en los dashboards e informes analíticos han sido transformados y distorsionados mediante técnicas visuales de anonimización. Esto garantiza la imposibilidad de identificar o rastrear el comportamiento comercial o técnico real de la operación, resguardando el secreto de mercado y protegiendo el ecosistema de **+XXXXX clientes activos** de la organización.

Este repositorio constituye un **Caso de Estudio con fines estrictamente académicos y de demostración técnica**, exponiendo la lógica del pipeline, el modelado del dato y el criterio analítico, sin vulnerar los activos de información ni los acuerdos de confidencialidad de las partes involucradas.



# 🌐 Sistema Integral de BI: Rendimiento Operativo y Customer Experience (CX) para ISP

## 📖 Storytelling del Proyecto

### ❓ ¿Puede un proveedor de internet mejorar la experiencia de sus usuarios si no es capaz de medir, en tiempo real, el rendimiento de sus cuadrillas de instalación y soporte técnico?

#### 🔍 El Origen del Desafío
En el sector de los Proveedores de Servicios de Internet (ISP), la calidad de la conectividad en el hogar depende directamente de la ejecución técnica en el campo. Sin embargo, en nuestra operación **no se contaba con un sistema de reportes ni un repositorio centralizado para auditar el rendimiento de las cuadrillas de red, help desk y atención al cliente**. La ejecución de estos roles se encontraba bajo un punto ciego de rendimiento para la gerencia. 

Esta **falta de visibilidad operativa** creaba un punto ciego crítico para la gerencia: impedía identificar cuellos de botella, evaluar los tiempos de resolución de incidencias de conectividad y hacía imposible correlacionar el desempeño técnico con la satisfacción real del cliente (**CSAT**). En una industria donde la estabilidad del servicio lo es todo, operar sin datos estructurados limitaba la gestión a una estrategia puramente reactiva ante los reclamos de los usuarios.

#### 🛠️ La Solución Implementada
Para resolver este vacío de información, diseñé e implementé un pipeline de datos automatizado, integrado de extremo a extremo (End-to-End) y *Cloud-Native*. La arquitectura utiliza:
1. **`Google Forms`**: Para la captura inmediata de datos de satisfacción post-servicio (instalación o soporte de internet).
2. **`Google Sheets`**: Como repositorio centralizado (*Data Store*) y motor de procesos ETL/ELT para la depuración, normalización y transformación de las variables operativas.
3. **`Looker Studio`**: Como capa de Inteligencia de Negocio, sirviendo como un sistema de reportería en tiempo real.

<p align="center">
  <img width="500" alt="Diagrama de Flujo del Sistema" src="https://github.com/user-attachments/assets/2483cee7-8f79-49d4-b122-58a3b536527f" />
</p>

---

## 🛠️ Módulo 1: Análisis de Desempeño de Cuadrillas (Rendimiento Técnico en Campo)

### ❓ ¿Cómo auditar la calidad y eficiencia de las instalaciones de red de múltiples proveedores externos bajo un mismo estándar analítico?

#### 💡 Primeras Percepciones de los Datos (Módulo Técnico)
Al centralizar y analizar la muestra piloto de este módulo, los primeros patrones de los datos revelaron tendencias clave sobre el rendimiento operativo y la distribución de la carga laboral:
* **📦 Distribución Asimétrica de Operaciones:** El **Contratista A absorbió el 55.9% de las órdenes de trabajo** operativas frente al 44.1% gestionado por el Contratista B, concentrando su despliegue principalmente en el *Sector Alpha* y el *Sector Beta*.
* **📉 Varianza Negativa en Niveles de Servicio:** El **Contratista B presentó una brecha de rendimiento negativa** en los indicadores críticos de eficiencia de resolución ($92.38\%$) y puntualidad ($93.33\%$) al ser contrastado de forma directa con los estándares de calidad demostrados por el Contratista A.

---
<img width="1103" height="868" alt="contratistas_anonimizado" src="https://github.com/user-attachments/assets/e53f70d2-e614-4866-affe-1e83d61536a6" />


---

#### 🚀 Oportunidades de Mejora Identificadas (Módulo Técnico)
* **🤝 Plan de Homologación de SLAs:** Establecer un plan de acción técnico y mesas de trabajo con el **Contratista B** para auditar sus cuellos de botella operativos, con el objetivo de homologar sus niveles de eficiencia con los estándares demostrados por el Contratista A.
* **📍 Optimización de Rutas Logísticas:** Rediseñar y optimizar la asignación geográfica de las órdenes de trabajo para balancear la carga operativa entre ambos contratistas, minimizando los tiempos de traslado por sector y agilizando el tiempo de respuesta en el domicilio del usuario.

---

## 📞 Módulo 2: Informe de Rendimiento y Soporte (Customer Experience - CX)

### ❓ ¿Medir el promedio de satisfacción es suficiente, o necesitamos auditar si los recursos invertidos en soporte crítico realmente se están aprovechando?

#### 💡 Primeras Percepciones y Auditoría de Calidad del Dato (Módulo CX)
Este entregable unifica la matriz de carga laboral (oficina y remoto) del equipo de *Helpdesk* con los indicadores de salud del cliente. El análisis arrojó métricas sobresalientes de atención, pero también desveló un sesgo analítico crítico en la recolección:

* **📈 Salud de la Atención y CX:** Los canales de soporte demostraron un rendimiento óptimo en la interacción directa, consolidando un **CSAT del 92.2%**, un **Tiempo Medio de Espera (TME) destacado de 1.9 minutos**, una valoración de trato de **4.6/5** y un índice de recomendación general de **8.0/10**.
* **⚠️ Diagnóstico Imparcial de Datos (Data Quality Issue):** A la gerencia le preocupaba saber si los recursos financieros invertidos para cubrir horarios especiales (nocturno y fines de semana) estaban siendo aprovechados con eficiencia. Inicialmente, el gráfico de *Alcance Operativo* arrojó un alarmante $90.74\%$ de "Inactividad" en el horario nocturno. Al realizar una auditoría profunda del dato crudo, identifiqué una **contaminación de variables**: los usuarios que consideraban que el servicio de internet era excelente y que *nunca tuvieron la necesidad de llamar al soporte*, seleccionaron por descarte la opción de "Inactividad (No saben/No usan)". 
* **💡 Lección Analítica:** Lejos de ocultar este ruido, identificar pronto este sesgo en mi primer proyecto real me permitió observar de primera mano las distorsiones que causa un instrumento de captura mal estructurado. Validó el impacto real de la regla *Garbage In, Garbage Out* (si introduces datos ambiguos, obtienes reportes distorsionados) y la necesidad imperativa de mejorar el diseño de la recopilación en el origen antes de masificar el flujo.

---

<img width="1411" height="1071" alt="informe_general" src="https://github.com/user-attachments/assets/6b19ab06-0afa-4da9-a6a3-de5c453572ed" />


---

#### 🚀 Oportunidades de Mejora Identificadas (Módulo CX)
* **📐 Rediseño de la Captura (Data Collection Re-engineering):** Implementar lógica de exclusión condicional (*Skip Logic*) en los formularios de captura para separar de forma estricta la "Inactividad por desconocimiento del canal o falta de uso" de la "Inactividad debido a la estabilidad óptima y correcto funcionamiento del servicio".
* **🧹 Depuración del Histórico:** Desarrollar un proceso de limpieza secundario para aislar las respuestas contaminadas actuales en el histórico y recalcular el verdadero porcentaje de uso de las ventanas de horarios especiales, asegurando una auditoría presupuestaria transparente y real para la jefatura de la agencia.

---

## 📐 Consideraciones Metodológicas y Validación Estadística (Fase Piloto)

### ❓ ¿Es ético tomar decisiones de inversión presupuestaria en base a las primeras tendencias de una muestra pequeña?

#### 🎯 Estado Actual: Producto Mínimo Viable y Fase Piloto
El análisis y los dashboards presentados actúan como una prueba de concepto analítica para validar la infraestructura del pipeline de datos. 

* **📋 Población vs. Muestra:** Los gráficos actuales se modelaron con base en una media de 45 a 52 encuestas recolectadas. Si bien este volumen fue clave para el **descubrimiento de sesgos** en el diseño de la captura (como el ruido detectado en el alcance operativo de horarios especiales), es estadísticamente insuficiente para representar con total fidelidad el universo completo de **+XXXX clientes activos** del ISP. Por tanto, el producto final en su estado actual posee un carácter predictivo preliminar y **no debe ser considerado de alta confiabilidad** para la toma de decisiones definitivas de alto presupuesto.
* **🎲 Técnica de Muestreo:** La recolección de datos se ejecutó bajo la metodología de **Muestreo Aleatorio Simple (MAS)**, garantizando que cada cliente encuestado tras una interacción técnica tuviera exactamente la misma probabilidad de selección, minimizando así el sesgo de selección en campo.

#### 📈 Ruta de Mitigación y Confiabilidad
Para elevar la madurez del proyecto de un nivel descriptivo/piloto a un **Sistema de Soporte a la Decisión (DSS)** con robustez estadística, se presentó a la jefatura de la agencia la siguiente estrategia de estabilización y escalado:

1. **⏳ Ventana Temporal de Maduración (3 Meses):** Es imperativo mantener el pipeline de recolección activo por un periodo mínimo de **tres meses consecutivos**. Esta ventana de tiempo permitirá mitigar las anomalías estacionales de la red y capturar un volumen de datos lo suficientemente robusto como para estabilizar la varianza.
2. **📉 Reducción del Margen de Error:** Al acumular los datos de este trimestre de operaciones, el tamaño de la muestra ($n$) alcanzará el umbral crítico requerido para calcular los KPIs con un nivel de confianza del $95\%$ y un margen de error inferior al $5\%$, transformando el tablero en una herramienta de auditoría financiera y operativa $100\%$ fiable.

---

## 🔄 Recomendaciones & Escalabilidad del Proyecto

Para evolucionar este MVP hacia una infraestructura de datos empresarial, robusta y funcional, se define el siguiente *Roadmap* de ingeniería:

- [ ] **🗄️ Migración a Base de Datos Relacional:** Sustituir Google Sheets por un motor de código abierto como `PostgreSQL` para garantizar la integridad referencial, mayor concurrencia en consultas simultáneas y optimización del almacenamiento histórico de logs.
- [ ] **⏱️ Análisis de Series Temporales (Time-Series) y Clustering:** Modelar los datos de soporte de forma temporal para identificar patrones de estacionalidad en las caídas del servicio de internet y anticipar picos de demanda. Asimismo, aplicar algoritmos de *Clustering* para identificar proactivamente segmentos de clientes inconformes con el servicio y mitigar un riesgo elevado de cancelación de contratos (*Churn Rate*).
- [ ] **🎛️ Tableros Dinámicos Avanzados:** Desarrollar en la interfaz de Looker Studio filtros cruzados por ventanas de tiempo móviles, selección múltiple de contratistas y segmentación avanzada por tipo de avería (*Internet lento vs. Sin señal*).
- [ ] **🤖 Automatización Completa:** Automatizar por completo las tareas rutinarias de limpieza y transformación del dato crudo mediante scripts programados, reduciendo a cero el procesamiento manual en el backend.
