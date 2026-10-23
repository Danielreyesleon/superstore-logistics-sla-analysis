DERI Solutions - Análisis de Eficiencia Logística y Cumplimiento de SLA
Descripción del Proyecto
Este proyecto fue desarrollado por el equipo consultor DERI Solutions como parte del Proyecto Integrador de Análisis de Datos.

El estudio analiza la eficiencia operativa del proceso de despacho de la empresa ficticia Superstore, una cadena minorista global especializada en la venta de suministros de oficina, mobiliario y tecnología.

El objetivo principal consiste en determinar si los pedidos se están procesando dentro de los tiempos comprometidos con los clientes mediante el análisis de los Acuerdos de Nivel de Servicio (SLA), identificando retrasos operativos y posibles cuellos de botella en la cadena logística.

Problema de Negocio
La organización no dispone de una medición centralizada que permita conocer con precisión cuánto tiempo transcurre entre la creación de una orden y su despacho desde bodega.

Esta situación provoca:

Falta de visibilidad sobre el desempeño logístico.
Posibles incumplimientos de SLA.
Riesgo de insatisfacción del cliente.
Pérdidas económicas asociadas a retrasos operativos.
Dificultad para identificar regiones o categorías problemáticas.
Objetivo General
Evaluar la eficiencia del proceso de despacho mediante el cálculo y análisis de los días de procesamiento de los pedidos, identificando desviaciones frente a los tiempos establecidos por prioridad de envío y detectando posibles cuellos de botella operativos.

Objetivos Específicos
Calcular la variable Processing Time utilizando:
Processing Time = Ship Date - Order Date
Medir el porcentaje de cumplimiento e incumplimiento de SLA.
Identificar categorías y mercados con mayores retrasos.
Detectar patrones relacionados con volumen de ventas y rentabilidad.
Generar indicadores clave para apoyar la toma de decisiones.
Dataset Utilizado
Fuente: Superstore Sales Analytics

Origen: Kaggle

Características del conjunto de datos:

Más de 51,000 registros.
21 variables.
Información comercial, geográfica y logística.
Datos relacionados con ventas, envíos, ganancias y clientes.
Variables relevantes:

Order Date
Ship Date
Order Priority
Category
Market
Sales
Profit
Shipping Cost
Tecnologías Utilizadas
Lenguajes
Python
Librerías
Pandas
NumPy
Matplotlib
Seaborn
Herramientas
Google Colab
Git
GitHub
Power BI
Proceso de Desarrollo
1. Exploración Inicial
Se realizó una revisión completa de la calidad de los datos para identificar:

Valores nulos
Errores de formato
Categorías inconsistentes
Valores atípicos
Tipos de datos incorrectos
2. Limpieza de Datos
Entre las transformaciones realizadas se encuentran:

Estandarización de nombres de columnas.
Corrección de errores ortográficos.
Conversión de fechas.
Eliminación de espacios innecesarios.
Corrección de categorías.
Conversión de variables numéricas.
Tratamiento de valores nulos.
Detección de registros atípicos.
3. Ingeniería de Variables
Se crearon indicadores adicionales para enriquecer el análisis:

Processing Time
Limit Day
Difference
Delay
On Time
Late Shipment
4. Análisis Exploratorio de Datos (EDA)
Se desarrollaron diferentes análisis:

Distribución de tiempos de procesamiento.
Cumplimiento de SLA.
Retrasos por prioridad.
Participación por país.
Análisis de Pareto.
Correlaciones operativas y financieras.
Identificación de anomalías.
5. Visualización
Se diseñó un dashboard interactivo en Power BI orientado a la toma de decisiones ejecutivas.

KPIs Definidos
KPI 1 - Tiempo Promedio de Procesamiento
Mide la velocidad operativa del proceso de despacho.

Processing Time = Ship Date - Order Date
KPI 2 - Cumplimiento de SLA
(Pedidos a tiempo / Total pedidos) × 100
KPI 3 - Retrasos Críticos
(Pedidos fuera de SLA / Total pedidos) × 100
KPI 4 - Cuello de Botella Operativo
Permite identificar las regiones y categorías con peor desempeño logístico.

Reglas de Negocio
Se definieron los siguientes tiempos máximos permitidos para cada prioridad:

Prioridad	SLA
Critical	0 días
High	2 días
Medium	4 días
Low	6 días
Los pedidos que superan estos límites son clasificados como incumplimientos de SLA.

Hallazgos Principales
Más del 60% de los pedidos presentan incumplimiento del SLA.
Las órdenes críticas son las que muestran mayores retrasos.
La categoría Tecnología representa el mayor riesgo económico.
Estados Unidos concentra la mayor cantidad de pedidos y retrasos.
29 países acumulan aproximadamente el 80% de las operaciones.
Recomendaciones
Priorizar la optimización logística en los pedidos críticos.
Intervenir la categoría Tecnología debido a su alto impacto económico.
Mejorar los procesos operativos en Estados Unidos.
Implementar monitoreo continuo de SLA mediante dashboards ejecutivos.
Establecer alertas tempranas para prevenir retrasos recurrentes.
Equipo de Trabajo
DERI Solutions
Integrante	Rol
Daniel J. Reyes	Data Engineer
Derinia Zhang Gu	Data Analyst
Luis Felipe Rodríguez Arce	Business Translator / Project Lead
Angeline Sandoval Arguedas	Business Translator / Project Lead
Estructura del Proyecto
DERI-Solutions/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── Limpieza_Datos.ipynb
│   ├── Fase_EDA.ipynb
│
├── dashboard/
│   └── Dashboard_PowerBI.pbix
│
├── images/
│
├── README.md
│
└── requirements.txt
Licencia
Proyecto desarrollado con fines académicos para el Programa de Especialización en Ciencia de Datos del Instituto Técnico Profesional de Costa Rica.

DERI Solutions | Data Analytics & Business Intelligence
