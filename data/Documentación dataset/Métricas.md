## Métricas 

Las métricas en el contexto de un dataset son medidas o valores cuantitativos que se utilizan para evaluar y comparar el rendimiento de modelos de machine learning, la calidad de los datos o las características del propio dataset. Estas métricas ayudan a entender qué tan bien un modelo está funcionando o a analizar ciertos aspectos del dataset, como la distribución de las clases, la variabilidad de los datos o la presencia de desequilibrios.

Existen varios tipos de métricas dependiendo del contexto:

### Métricas de evaluación del rendimiento del modelo

Estas métricas se utilizan para medir el rendimiento de los modelos de machine learning. La elección de la métrica adecuada depende del tipo de problema (clasificación, regresión, clustering, etc.).

Métricas de clasificación:

Estas métricas son útiles cuando el modelo tiene que clasificar los datos en categorías o clases.

	•	Accuracy (Exactitud): Proporción de predicciones correctas sobre el total de predicciones.

\text{Accuracy} = \frac{\text{Predicciones correctas}}{\text{Total de predicciones}}

``

	•	Precision (Precisión): Proporción de verdaderos positivos sobre el total de predicciones positivas hechas por el modelo.

\text{Precisión} = \frac{\text{Verdaderos Positivos}}{\text{Verdaderos Positivos} + \text{Falsos Positivos}}

	•	Recall (Sensibilidad o Tasa de Verdaderos Positivos): Proporción de verdaderos positivos sobre el total de positivos reales en los datos.

\text{Recall} = \frac{\text{Verdaderos Positivos}}{\text{Verdaderos Positivos} + \text{Falsos Negativos}}

	•	F1-Score: Media armónica de la precisión y el recall. Es útil cuando hay un desequilibrio entre las clases.

\text{F1} = 2 \times \frac{\text{Precisión} \times \text{Recall}}{\text{Precisión} + \text{Recall}}

	•	AUC-ROC: Área bajo la curva ROC, que mide el rendimiento de un clasificador binario en diferentes umbrales de decisión.

Métricas de regresión:

Estas métricas se utilizan en problemas donde el objetivo es predecir un valor continuo.

	•	Mean Absolute Error (MAE): Promedio de los valores absolutos de los errores entre las predicciones y los valores reales.

\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} \left| y_i - \hat{y}_i \right|

	•	Mean Squared Error (MSE): Promedio de los cuadrados de los errores entre las predicciones y los valores reales.

\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} \left( y_i - \hat{y}_i \right)^2

	•	R² (Coeficiente de Determinación): Mide qué tan bien se ajusta el modelo a los datos. Un valor cercano a 1 indica que el modelo explica la mayoría de la variabilidad en los datos.

R^2 = 1 - \frac{\sum_{i=1}^{n} (y_i - \hat{y}i)^2}{\sum{i=1}^{n} (y_i - \bar{y})^2}


2. Métricas descriptivas del dataset

Estas métricas ayudan a describir las características básicas de un dataset. Son útiles en la fase de Exploratory Data Analysis (EDA), cuando intentas comprender la estructura de los datos.

	•	Media: El promedio de todos los valores en una columna.

\text{Media} = \frac{\sum_{i=1}^{n} x_i}{n}

	•	Mediana: El valor central en un conjunto de datos ordenado.
	•	Varianza: Mide la dispersión de los datos respecto a la media.

\text{Varianza} = \frac{1}{n} \sum_{i=1}^{n} (x_i - \bar{x})^2

	•	Desviación estándar: La raíz cuadrada de la varianza, que indica qué tan dispersos están los datos respecto a la media.

\text{Desviación Estándar} = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (x_i - \bar{x})^2}

	•	Distribución de clases: En un problema de clasificación, la cantidad o proporción de ejemplos que pertenecen a cada clase.
	•	Correlación: Indica la relación entre dos variables. Puede ser positiva, negativa o nula.

\text{Coeficiente de correlación de Pearson} = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum (x_i - \bar{x})^2 \sum (y_i - \bar{y})^2}}


3. Métricas de calidad de los datos

Estas métricas miden la calidad de los datos y pueden identificar problemas como valores faltantes o datos duplicados.

	•	Valores faltantes (Missing values): Proporción de valores faltantes en el dataset.
	•	Duplicados: Cantidad de registros duplicados en el dataset.
	•	Outliers: Observaciones que están muy alejadas del resto de los datos.

Resumen

Las métricas en un dataset son herramientas fundamentales que ayudan a medir el rendimiento de los modelos, describir los datos y evaluar la calidad de los mismos. Según el tipo de problema y los datos con los que estés trabajando, seleccionarás las métricas más apropiadas para obtener una evaluación adecuada.