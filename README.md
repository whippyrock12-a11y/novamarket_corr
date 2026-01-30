# 📊 NovaMarket: Análisis de Correlación y Comportamiento de Usuario
Este repositorio contiene el análisis exploratorio y estadístico realizado para NovaMarket, enfocado en identificar las relaciones existentes entre la actividad de los usuarios, sus hábitos de compra y los ingresos mensuales generados.

El proyecto utiliza técnicas estadísticas avanzadas (Pearson, Spearman, Punto-Biserial y V de Cramér) para validar hipótesis de negocio mediante evidencia numérica y visual.

**📂 Contenido del Repositorio**
NovaMarket_Correlation_Analysis.ipynb: Notebook principal que incluye la limpieza de datos, visualización de relaciones (Heatmaps/Pairplots) y cálculo de coeficientes estadísticos.

nova_market_activity.csv: Dataset con métricas de visitas, compras, gasto publicitario, satisfacción y perfiles demográficos.

**🧠 Objetivo del Análisis**
El propósito es transformar datos de actividad en hipótesis estratégicas, respondiendo a preguntas clave:

¿Existe una relación directa entre la frecuencia de visitas y las compras efectivas?

¿El estado de suscripción es un predictor confiable de los ingresos mensuales?

¿Cómo interactúan las variables categóricas como la región y el dispositivo?

**🛠️ Tecnologías Utilizadas**
Python 3.x
Pandas: Procesamiento de datos y filtrado de usuarios activos.
Seaborn & Matplotlib: Generación de matrices de correlación y diagramas de dispersión.
SciPy: Cálculo de coeficientes de correlación especializados (Point-Biserial y Chi-cuadrado).

**📈 Metodología y Hallazgos (Insights)**
1. Relación Actividad vs. Transacción
Se analizó la conexión entre visitas_ultimos_30d y compras.
Evidencia: Pearson: 0.299 | Spearman: 0.280.
Insight: Existe una correlación positiva moderada. Los usuarios que visitan más la plataforma tienden a comprar más, sugiriendo que el engagement es un precursor del ingreso.

2. Segmentación por Suscripción
Se aplicó la correlación Punto-Biserial para entender si los suscriptores generan más ingresos.
Resultado: Coeficiente de 0.063.
Insight: La asociación es prácticamente nula. Estar suscrito no garantiza un mayor nivel de ingresos mensuales, lo que sugiere que el modelo de suscripción actual no está capturando a los clientes de alto valor de forma exclusiva.

3. Análisis de Categorías (Región y Dispositivo)
Utilizando la V de Cramér, se midió la fuerza de asociación entre variables no numéricas.
Resultado: Asociación débil entre la región geográfica y el tipo de dispositivo utilizado.

**🚀 Conclusiones de Negocio**
[!IMPORTANT] Estrategia Recomendada: No utilizar la suscripción como único criterio de segmentación de clientes VIP. Se recomienda realizar análisis de cohortes y experimentos controlados (A/B Testing) para verificar si incentivar las visitas aumenta directamente el volumen de compras.
