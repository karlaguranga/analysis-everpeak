# analysis-everpeak
# 📊 Análisis de Segmentación de Clientes - ConnectaTel

🎯 Objetivo del Proyecto
Este proyecto analiza el comportamiento de uso de servicios móviles de ConnectaTel, una empresa de telecomunicaciones con operaciones en México y Colombia. El objetivo principal es identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos de clientes muestran necesidades diferenciadas para optimizar la oferta comercial y mejorar la experiencia del usuario.

Preguntas de Negocio Clave
¿Qué segmentos de clientes muestran mayor o menor uso de llamadas y mensajes?
¿Qué usuarios presentan valores atípicos que puedan indicar comportamientos inusuales?
¿Cómo varía el uso según la edad y el tipo de plan contratado?
¿Qué patrones pueden ayudar a diseñar mejores planes y optimizar la oferta?
📁 Datasets Utilizados
El análisis se basa en tres fuentes principales de datos:

### 1. plans.csv
- Descripción: Catálogo de planes disponibles
- Contenido: Precios, minutos incluidos, GB incluidos, costos por extras
- Registros: Información de planes Básico y Premium

### 2. users_latam.csv
- Descripción: Información demográfica y contractual de clientes
- Contenido: Edad, ciudad, país, fecha de registro, plan contratado, estado de churn
- Registros: 4,000 usuarios activos

### 3. usage.csv
- Descripción: Detalle de uso real de servicios
- Contenido: Número de llamadas, duración total, número de mensajes, longitud de mensajes
- Registros: Actividad mensual por usuario

🔄 Etapas del Análisis
### 1. Exploración y Carga de Datos
- Importación de las tres fuentes de datos
- Análisis inicial de estructura y tipos de datos
- Identificación de relaciones entre datasets

### 2. Limpieza y Preprocesamiento
- Detección y corrección de valores sentinel (-999 en edad)
- Manejo de fechas imposibles (2026)
- Tratamiento de valores faltantes y inconsistentes
- Estandarización de tipos de datos

### 3. Integración de Datos
- Merge de los tres datasets usando user_id como clave
- Creación del dataset consolidado user_profile
- Validación de integridad de datos

### 4. Análisis Estadístico Descriptivo
- Estadísticas descriptivas por variable
- Distribuciones de uso por plan y demografía
- Análisis de correlaciones

### 5. Detección de Outliers
- Aplicación del método IQR (Rango Intercuartílico)
- Análisis de valores extremos en llamadas, mensajes y duración
- Decisiones de negocio sobre mantenimiento de outliers

### 6. Segmentación de Clientes
- Creación de segmentos por edad (Joven, Adulto, Adulto Mayor)
- Segmentación por nivel de uso (Bajo, Medio, Alto)
- Análisis cruzado de segmentos

### 7. Visualización y Insights
- Gráficos de distribución por segmentos
- Análisis comparativo entre grupos
- Identificación de patrones de comportamiento

### 8. Análisis Ejecutivo
- Traducción de hallazgos



