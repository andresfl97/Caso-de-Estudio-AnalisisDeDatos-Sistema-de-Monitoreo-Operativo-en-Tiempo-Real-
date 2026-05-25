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
En el sector de los Proveedores de Servicios de Internet (ISP), la calidad de la conectividad en el hogar depende directamente de la ejecución técnica. Sin embargo, en nuestra operación **no se contaba con un sistema de reportes ni un repositorio centralizado para auditar el rendimiento de los contratistas, soporte técnico (help desk) y atención al cliente**. La ejecución de estos roles se encontraba bajo un punto ciego de rendimiento para la empresa. 

Esta **falta de visibilidad operativa**  impedía identificar cuellos de botella, evaluar los tiempos de resolución de incidencias de conectividad. En una industria donde la estabilidad del servicio y el servicio al cliente lo es todo, operar sin datos estructurados limitaba la gestión a una estrategia puramente reactiva ante los reclamos de los usuarios.

#### 🛠️ La Solución 
Para resolver este vacío de información, diseñé e implementé un pipeline de datos automatizado, integrado de extremo a extremo (End-to-End) y *Cloud-Native*. La arquitectura utiliza:
1. **`Google Forms`**: Para la captura inmediata de datos de satisfacción post-servicio (instalación o soporte de internet).
2. **`Google Sheets`**: Como repositorio centralizado (*Data Store*) y motor de procesos ETL/ELT para la depuración, normalización y transformación de las variables operativas.
3. **`Looker Studio`**: Como capa de Inteligencia de Negocio, sirviendo como un sistema de reportería en tiempo real.

<p align="center">
  <img width="500" alt="Diagrama de Flujo del Sistema" src="https://github.com/user-attachments/assets/2483cee7-8f79-49d4-b122-58a3b536527f" />
</p>


El diagrama de flujo se puede interpretar a traves de los siguientes niveles: 
* Primero, la Ingesta captura la experiencia del cliente mediante llamadas en frío centralizadas en Google Forms.
* Segundo, el Almacenamiento y Lógica actúa como el motor del sistema en Google Sheets, procesando los datos crudos en una matriz de cálculos y consultas estructuradas mediante procesos ETL.
* Finalmente, la Capa de Negocio conecta esta información de forma directa con Looker Studio, transformando los datos limpios en dos cuadros de mando interactivos que permiten auditar en tiempo real tanto el desempeño del equipo técnico y atención al cliente.

---

## 🛠️ Módulo 1: Análisis de Desempeño de Contratistas (Rendimiento Técnico de ejecución de actividades)

### ❓ ¿Estamos gestionando la carga laboral de nuestras cuadrillas de manera que proyecten profesionalismo y calidad, asegurando que cada cliente se sienta satisfecho con el servicio contratado?

#### 💡 Primeras Percepciones de los Datos (Módulo Técnico)
Al centralizar y analizar la muestra piloto de este módulo, los primeros patrones de los datos revelaron tendencias clave sobre el rendimiento operativo y la distribución de la carga laboral:
* **📦 Distribución Asimétrica de Operaciones:** El **Contratista A absorbió el 55.9% de las órdenes de trabajo**  frente al 44.1% del Contratista B, concentrando su despliegue principalmente en el *Sector Alpha* y el *Sector Beta*.
* **📉 Niveles de Servicio:** El **Contratista B presentó una brecha de rendimiento negativa** en los indicadores de eficiencia de resolución ($92.38\%$) y puntualidad ($93.33\%$) al ser contrastado de forma directa con los estándares de calidad demostrados por el Contratista A.

---
<img width="1103" height="868" alt="contratistas_anonimizado" src="https://github.com/user-attachments/assets/e53f70d2-e614-4866-affe-1e83d61536a6" />


---

#### 🚀 Oportunidades de Mejora Identificadas (Módulo Técnico)
* **🤝 Plan de Homologación de SLAs:** Establecer un plan de acción técnico y mesas de trabajo con el **Contratista B** para auditar sus cuellos de botella operativos, con el objetivo de homologar sus niveles de eficiencia con los estándares demostrados por el Contratista A.
* **📍 Optimización de Rutas Logísticas:** Rediseñar y optimizar la asignación geográfica de las órdenes de trabajo para balancear la carga operativa entre ambos contratistas, minimizando los tiempos de traslado por sector y agilizando el tiempo de respuesta en el domicilio del usuario.

---

## 📞 Módulo 2: Informe de Soporte Técnico, Atención al Cliente y Percepción del Servicio (Customer Experience - CX)

### ❓ ¿Es suficiente medir la satisfacción del cliente o también se debe validar si los recursos de soporte realmente generan valor operativo?

## 💡 Auditoría de Calidad del Dato y Percepción del Servicio (Módulo CX)

Este análisis integró la matriz operativa del equipo *Helpdesk* (presencial y remoto) con indicadores de experiencia del cliente, permitiendo contrastar desempeño operativo, percepción del servicio y utilización real de recursos.

### 📈 Indicadores Operativos y Experiencia del Cliente

- **CSAT:** 92.2%
- **Tiempo Medio de Espera (TME):** 1.9 minutos
- **Valoración de atención:** 4.6/5
- **Percepción general del servicio:** 8/10
- **Nivel de recomendación:** 4.1/5

Los indicadores reflejan una experiencia positiva del cliente; sin embargo, el análisis detectó un comportamiento atípico en horarios especiales (nocturnos y fines de semana), con niveles de inactividad del **90.74%** y **87.04%** respectivamente.

### ⚠️ Hallazgo Analítico: Sesgo en la Recolección

El porcentaje de “inactividad” inicialmente fue interpretado como baja utilización del soporte fuera del horario regular. No obstante, la auditoría del dato crudo permitió identificar una contaminación de variables en el instrumento de captura:

Muchos usuarios que calificaban el servicio como “excelente” y que nunca necesitaron contactar soporte seleccionaban la opción *“No sabe / No usa”*, generando una falsa percepción de desperdicio operativo.

### 🔍 Interpretación Estratégica

El problema no estaba únicamente en la demanda del servicio, sino en la ausencia de comunicación efectiva sobre la disponibilidad de soporte 24/7. La percepción positiva del servicio coexistía con desconocimiento de los canales de atención.

Este hallazgo permitió evidenciar cómo un diseño ambiguo en la captura puede distorsionar indicadores gerenciales y afectar decisiones sobre asignación de recursos.

### 💡 Aprendizaje Técnico

La detección temprana de este sesgo permitió validar, en un entorno real, el impacto de la regla *Garbage In, Garbage Out*: datos ambiguos producen análisis imprecisos.

El proyecto evidenció la necesidad de fortalecer la calidad del dato desde el origen antes de escalar la muestra e implementar procesos analíticos, dashboards o métricas de negocio.

---

<img width="1411" height="1071" alt="informe_general" src="https://github.com/user-attachments/assets/6b19ab06-0afa-4da9-a6a3-de5c453572ed" />


---

#### 🚀 Oportunidades de Mejora Identificadas (Módulo CX)
### 📐 Reingeniería de Captura de Datos

Rediseño del flujo de recolección mediante lógica de exclusión condicional (*Skip Logic*), separando de forma precisa:

- Usuarios que desconocen la existencia del canal de soporte.
- Usuarios que no utilizan soporte debido a la estabilidad y correcto funcionamiento del servicio.

La modificación permitió reducir ambigüedad en la captura y mejorar la trazabilidad analítica de los indicadores operativos.

### 🧠 Análisis de Sentimientos y Contexto Operativo

Durante la captura y interacciones telefónicas, se identificó que las encuestas tradicionales no reflejaban completamente la percepción del cliente.

Aunque muchos usuarios calificaban positivamente el servicio, las conversaciones telefónicas revelaban molestias, frustraciones y observaciones operativas que no aparecían en los formularios estructurados.

Esto permitió detectar una fuente complementaria de información para realizar un análisis de sentimientos, enriqueciendo la interpretación de KPI’s como CSAT, recomendación y percepción del servicio.

### 🧹 Depuración y Recalibración del Histórico

Diseño de un proceso de limpieza secundaria orientado a aislar respuestas contaminadas dentro del histórico de datos, permitiendo recalcular el uso real de horarios especiales.

La depuración permitió generar una visión más precisa para auditoría presupuestaria y evaluación de eficiencia operativa en la asignación de recursos de soporte técnico.

---

## 📐 Consideraciones Metodológicas y Validación Estadística (Fase Piloto)

### ❓ ¿Es ético tomar decisiones de inversión presupuestaria en base a las primeras tendencias de una muestra pequeña?

#### 🎯 Estado Actual: Producto Mínimo Viable y Fase Piloto
El análisis y los dashboards presentados actúan como una prueba de los primeros patrones y tendencias que se enfrenta al empresa día a día. 

* **📋 Población vs. Muestra:** Los gráficos actuales se modelaron con base en una media de 45 a 52 encuestas recolectadas. Si bien este volumen fue clave para el **descubrimiento de sesgos** en el diseño de la captura (como el ruido detectado en el alcance operativo de horarios especiales), es estadísticamente insuficiente para representar con total fidelidad el universo completo de **+XXXX clientes activos** del ISP. Por tanto, el producto final en su estado actual posee un carácter predictivo preliminar y **no debe ser considerado de alta confiabilidad** para la toma de decisiones definitivas de alto presupuesto.
* **🎲 Técnica de Muestreo:** La recolección de datos se ejecutó bajo la metodología de **Muestreo Aleatorio Simple (MAS)**, garantizando que cada cliente encuestado tras una interacción técnica tuviera exactamente la misma probabilidad de selección, minimizando así el sesgo de selección en campo.


---

## 🔄 Recomendaciones & Escalabilidad del Proyecto

Para evolucionar este proyecto hacia una infraestructura de datos empresarial, robusta y funcional, se define el siguiente *Roadmap* de ingeniería:

- [ ] **🗄️ Migración a Base de Datos Relacional:** Sustituir Google Sheets por un motor de código abierto como `PostgreSQL` para garantizar la integridad referencial, mayor concurrencia en consultas simultáneas y optimización del almacenamiento histórico.
- [ ] **⏱️ Análisis de Series Temporales (Time-Series) y Clustering:** Modelar los datos de soporte de forma temporal para identificar patrones de estacionalidad en las caídas del servicio de internet y anticipar picos de demanda. Asimismo, aplicar algoritmos de *Clustering* para identificar proactivamente segmentos de clientes inconformes con el servicio y mitigar un riesgo elevado de cancelación de contratos (*Churn Rate*).
- [ ] **🎛️ Tableros Dinámicos Avanzados:** Desarrollar en la interfaz de Looker Studio filtros cruzados por ventanas de tiempo móviles, selección múltiple de contratistas y segmentación avanzada con la finalidad de que gerencia pueda generar reportes en tiempo real de métricas de su interes, ya sea diario, semanal, mensual o incluso anual si el proyecto escala.
- [ ] **🤖 Automatización Completa:** Automatizar por completo las tareas rutinarias de limpieza y transformación del dato crudo mediante scripts programados, reduciendo a cero el procesamiento manual en el backend.
