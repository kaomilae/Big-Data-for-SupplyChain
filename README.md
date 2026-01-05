
# **Big Data Analysis- Proyecto Big-Data**

**OBJETIVO GENERAL**:
Integrar el análisis de datos de la cadena de suministro (supply chain) con técnicas de machine learning para desarrollar un modelo de clasificación que prediga el riesgo de entrega tardía. Este modelo considerará diversos factores operacionales, logísticos y de producto (distancia, peso, transportista, ciudad destino, tipo de producto, tiempo de procesamiento) para identificar anticipadamente qué envíos presentan mayor probabilidad de retraso, permitiendo tomar decisiones proactivas que reduzcan las incidencias y mejoren la satisfacción del cliente.

**OBJETIVO DE NEGOCIO**
Reducir significativamente el número de entregas tardías mediante predicción temprana del riesgo, lo cual permitirá:

Disminuir quejas y reclamos
Mejorar la reputación de la marca
Incrementar la retención de clientes
Optimizar recursos logísticos
Tomar decisiones informadas sobre rutas, transportistas y priorización


**OBJETIVOS ESPECÍFICOS DEL NOTEBOOK**
1. Análisis Exploratorio Enfocado en Supply Chain
Desarrollar un análisis exploratorio de datos (EDA) utilizando Pandas-Profiling y otras librerías de Python, con enfoque específico en variables de la cadena de suministro:

Identificar y analizar factores clave: distancia de envío, peso del paquete, tipo de transportista, ciudad de origen/destino, categoría de producto, tiempos de procesamiento
Examinar la distribución de entregas tardías vs puntuales
Detectar patrones y relaciones entre variables del supply chain
Documentar conclusiones relevantes para el negocio

2. Limpieza y Preparación de Datos
Ejecutar procesos de limpieza basados en los hallazgos del EDA:

Gestión de valores faltantes y registros duplicados
Identificación y tratamiento de valores atípicos
Transformación de variables categóricas (codificación)
Estandarización de escalas cuando sea necesario
Evaluación del balance de clases (entregas tardías vs puntuales)

3. Análisis Multivariable y Visualización de Factores
Realizar análisis de múltiples variables utilizando librerías de visualización (Matplotlib, Seaborn, Plotly):

Correlaciones entre factores del supply chain y entregas tardías
Comparación de tasas de retraso por transportista, ciudad, categoría de producto
Análisis de impacto de distancia y peso en tiempos de entrega
Gráficos interpretativos: mapas de calor, diagramas de caja, gráficos de dispersión
Identificación visual de factores de mayor riesgo

4. Validación Estadística de Factores de Riesgo
Plantear y evaluar hipótesis sobre los factores que causan entregas tardías mediante estadística inferencial:
Hipótesis ejemplo:

H0: La distancia del envío no afecta la probabilidad de entrega tardía
H1: Mayor distancia incrementa el riesgo de retraso

Otras hipótesis a explorar:

Diferencias entre transportistas
Impacto del peso del producto
Influencia de la ciudad destino
Efecto del tiempo de procesamiento

Métodos estadísticos: Chi-cuadrado, pruebas t, ANOVA (α = 0.05)
5. Desarrollo de Modelos Predictivos de Clasificación
Construir y comparar diferentes algoritmos de machine learning que permitan predecir el riesgo de entrega tardía basándose en los factores identificados:

Modelos candidatos: Regresión Logística, Random Forest, XGBoost, Gradient Boosting
Métricas de evaluación: Accuracy, Precision, Recall, F1-Score, Curva ROC-AUC
Interpretabilidad: Identificar qué variables tienen mayor peso en la predicción
Selección final: Elegir el modelo con mejor balance entre precisión y aplicabilidad operativa


**ENTREGABLE FINAL**
Un modelo predictivo operacional que:

Identifique en tiempo real qué envíos tienen alto riesgo de llegar tarde
Cuantifique el riesgo (probabilidad de retraso)
Explique los factores que contribuyen al riesgo en cada caso
Permita acciones preventivas: reasignación de transportista, ajuste de rutas, comunicación proactiva al cliente, priorización de procesamiento

Impacto esperado: Reducción medible de entregas tardías, disminución de quejas, mejor planificación del supply chain y mayor satisfacción del cliente.
# Dataset
El conjunto de datos contiene información de la cadena de suministro para un comercio electrónico. Los datos describen procesos de aprovisionamiento, producción, ventas y distribución comercial. También permite la correlación de Datos Estructurados con Datos No Estructurados para la generación de conocimiento. El dataset  ha sido tomado del repositorio kaggle y se encuentra disponible a través del siguiente enlace: https://www.kaggle.com/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis
