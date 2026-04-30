# House-Prices
Modelos predictivos de Machine Learning

# Descripción del problema

Este proyecto aborda un problema de regresión supervisada cuyo objetivo es predecir el precio de venta de viviendas (SalePrice) a partir de sus características físicas, estructurales y de ubicación.
El problema se enmarca en el sector inmobiliario, donde la estimación precisa del valor de una propiedad es clave para la toma de decisiones.

# Dominio del problema

El proyecto pertenece al ámbito de:
Bienes raíces
Finanzas
Análisis de datos
Machine Learning aplicado

# Utilidad
Este proyecto tiene una alta utilidad en el sector inmobiliario, ya que permite estimar de manera precisa el precio de una vivienda a partir de sus características físicas, estructurales y de ubicación. Esto facilita la toma de decisiones tanto para compradores, quienes pueden evaluar si el precio de una propiedad es justo, como para vendedores, que pueden establecer precios competitivos en el mercado. Asimismo, resulta de gran valor para inversionistas inmobiliarios al identificar oportunidades de negocio, y para entidades financieras, como bancos, que requieren estimaciones confiables para la aprobación de créditos hipotecarios. En general, este modelo actúa como una herramienta de apoyo basada en datos que mejora la eficiencia y precisión en la valoración de bienes raíces.

# Dataset
Dataset: House Prices — Advanced Regression Techniques (Kaggle)
Contiene información de viviendas en Ames, Iowa (EE.UU.).

# Variables
El dataset incluye:

# Variables numéricas
Área habitable (GrLivArea)
Área del lote (LotArea)
Área del sótano (TotalBsmtSF)
Área del garaje (GarageArea)
Año de construcción (YearBuilt)
Número de habitaciones y baños
# Variables categóricas
Vecindario (Neighborhood)
Calidad de la vivienda (OverallQual)
Tipo de vivienda
Tipo de garaje
# Variable objetivo
SalePrice

# Tipo de problema
Regresión 

# Pregunta del proyecto
¿Se puede predecir el precio de una vivienda a partir de sus características?

# Solucion del problema
La solución propuesta consistió en desarrollar un modelo de Machine Learning para predecir el precio de las viviendas utilizando técnicas de regresión supervisada. Para ello, se realizó un proceso completo que incluyó el análisis exploratorio de los datos (EDA), el tratamiento de valores nulos, la transformación de variables categóricas y el escalado de variables numéricas mediante un pipeline. Posteriormente, se entrenaron diferentes modelos como Árbol de Decisión, Bagging, Random Forest, AdaBoost y XGBoost, aplicando validación cruzada con 10 folds para garantizar resultados robustos. Finalmente, se optimizaron los hiperparámetros de cada modelo mediante GridSearchCV con el fin de mejorar su desempeño predictivo.

# Resultados encontrados
Los resultados mostraron que los modelos de ensamble obtuvieron un desempeño superior frente a modelos individuales. En particular, XGBoost fue el modelo que presentó el mejor rendimiento, alcanzando el menor Error Cuadrático Medio (ECM ≈ 655 millones) y el mayor coeficiente de determinación (R² ≈ 0.91), lo que indica que logra explicar más del 90% de la variabilidad del precio de las viviendas. Random Forest también mostró resultados sólidos, mientras que AdaBoost tuvo un desempeño intermedio. Por otro lado, el Árbol de Decisión fue el modelo con peor desempeño, evidenciando limitaciones para capturar la complejidad del problema.

# Conclusiones
El proyecto permitió demostrar que el uso de modelos de Machine Learning, especialmente los modelos de ensamble, es altamente efectivo para la predicción de precios de viviendas. Se evidenció que variables como la calidad de la vivienda, el área habitable y el tamaño del garaje son determinantes en la estimación del precio. Además, se concluye que XGBoost es el modelo más adecuado para este problema, ya que presenta el mejor equilibrio entre precisión y capacidad de generalización. En general, este tipo de soluciones basadas en datos aporta un valor significativo al sector inmobiliario, facilitando la toma de decisiones de manera más objetiva y precisa.



