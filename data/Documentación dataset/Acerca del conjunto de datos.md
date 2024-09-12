# Acerca del conjunto de datos

## Contexto

La diabetes es una de las enfermedades crónicas más prevalentes en Estados Unidos, afecta a millones de estadounidenses cada año y supone una importante carga financiera para la economía. La diabetes es una enfermedad crónica grave en la que los individuos pierden la capacidad de regular eficazmente los niveles de glucosa en la sangre, y puede conducir a una reducción de la calidad y la esperanza de vida. Después de que los distintos alimentos se descompongan en azúcares durante la digestión, éstos se liberan en el torrente sanguíneo. Esto indica al páncreas que libere insulina. La insulina ayuda a las células del organismo a utilizar los azúcares del torrente sanguíneo como fuente de energía. En general, la diabetes se caracteriza porque el organismo no produce suficiente insulina o porque es incapaz de utilizar la insulina producida con la eficacia necesaria.

Complicaciones como las cardiopatías, la pérdida de visión, la amputación de miembros inferiores y las enfermedades renales están asociadas a los niveles crónicamente altos de azúcar que permanecen en el torrente sanguíneo de los diabéticos. Aunque la diabetes no tiene cura, estrategias como perder peso, comer sano, mantenerse activo y recibir tratamientos médicos pueden mitigar los daños de esta enfermedad en muchos pacientes. Un diagnóstico precoz puede conducir a cambios en el estilo de vida y a un tratamiento más eficaz, lo que convierte a los modelos de predicción del riesgo de diabetes en herramientas importantes para los responsables de la salud pública.

También es importante reconocer la magnitud de este problema. Los Centros para el Control y la Prevención de Enfermedades han indicado que a partir de 2018, 34,2 millones de estadounidenses tienen diabetes y 88 millones tienen prediabetes. Además, los CDC estiman que 1 de cada 5 diabéticos, y aproximadamente 8 de cada 10 prediabéticos desconocen su riesgo. Aunque existen distintos tipos de diabetes, la de tipo II es la más común y su prevalencia varía en función de la edad, la educación, los ingresos, la ubicación, la raza y otros determinantes sociales de la salud. Gran parte de la carga de la enfermedad recae también en las personas de nivel socioeconómico más bajo. La diabetes también supone una enorme carga para la economía, ya que los costes de la diabetes diagnosticada rondan los 327.000 millones de dólares y los costes totales de la diabetes no diagnosticada y la prediabetes se aproximan a los 400.000 millones de dólares anuales.

## Contenido

El Sistema de Vigilancia de Factores de Riesgo en el Comportamiento (BRFSS) es una encuesta telefónica relacionada con la salud que recogen anualmente los CDC. Cada año, la encuesta recoge respuestas de más de 400.000 estadounidenses sobre comportamientos de riesgo relacionados con la salud, enfermedades crónicas y el uso de servicios preventivos. Se lleva realizando todos los años desde 1984. Para este proyecto, se utilizó un csv del conjunto de datos disponible en Kaggle para el año 2015. Este conjunto de datos original contiene respuestas de 441.455 individuos y tiene 330 características. Estas características son preguntas formuladas directamente a los participantes o variables calculadas a partir de las respuestas individuales de los participantes.

- Este conjunto de datos contiene 3 archivos:

  - **diabetes _ 012 _ health _ indicators _ BRFSS2015.csv** es un conjunto de datos limpio de 253.680 respuestas a la encuesta BRFSS2015 de los CDC. 

    La variable **objetivo Diabetes_012** tiene 3 clases. 0 es para no diabetes o sólo durante el embarazo, 1 es para prediabetes y 2 es para diabetes. Hay desequilibrio de clases en este conjunto de datos. Este conjunto de datos tiene 21 variables de características

  - **diabetes _ binary _ 5050split _ health _ indicators _ BRFSS2015.csv** es un conjunto de datos limpio de 70.692 respuestas a la encuesta BRFSS2015 de los CDC. Tiene una división igual 50-50 de encuestados sin diabetes y con prediabetes o diabetes. La variable **objetivo Diabetes_binaria** tiene 2 clases. 0 corresponde a no diabetes y 1 a prediabetes o diabetes. Este conjunto de datos tiene 21 variables de características y está equilibrado.

  - **diabetes _ binary _ health _ indicators _ BRFSS2015.csv** es un conjunto de datos limpio de 253.680 respuestas a la encuesta BRFSS2015 de los CDC. La variable **objetivo Diabetes_binary** tiene 2 clases. 0 es para no diabetes, y 1 es para prediabetes o diabetes. Este conjunto de datos tiene 21 variables de características y no está equilibrado.

Explore algunas de las siguientes preguntas de investigación:

- ¿Pueden las preguntas de la encuesta BRFSS proporcionar predicciones precisas sobre si un individuo tiene diabetes?
- ¿Qué factores de riesgo predicen mejor el riesgo de diabetes?
- ¿Podemos utilizar un subconjunto de factores de riesgo para predecir con exactitud si un individuo tiene diabetes?
- ¿Podemos crear un formulario abreviado de preguntas del BRFSS utilizando la selección de características para predecir con exactitud si alguien podría tener diabetes o está en alto riesgo de padecerla?

  ## Agradecimientos

Es importante reiterar que yo no he creado este conjunto de datos, es sólo un conjunto de datos limpio y consolidado creado a partir del conjunto de datos BRFSS 2015 que ya está en Kaggle. Ese conjunto de datos se puede encontrar aquí y el cuaderno que utilicé para la limpieza de datos se puede encontrar aquí.
  ## Inspiración

  Zidian Xie et al para Building Risk Prediction Models for Type 2 Diabetes Using Machine Learning Techniques using the 2014 BRFSS fue la inspiración para crear este conjunto de datos y explorar el BRFSS en general. [Enlace](https://www.cdc.gov/pcd/issues/2019/19_0109.htm)

  

  ## Para plantear un buen proyecto con los datos de la encuesta BRFSS2015, y considerando que ya tienes tres CSV con distintas variables relacionadas con la salud, te sugiero seguir estos pasos para guiar el análisis y los objetivos del proyecto. Aquí van algunas ideas sin entrar en código, solo en la planificación general:

1. Definir el objetivo principal

Lo primero es tener claro qué quieres predecir o explorar. Dado que estás trabajando con temas de salud, podrías enfocarte en:

  • Predicción de la probabilidad de que una persona sea diabética basada en variables de estilo de vida y factores de riesgo.
  • Evaluar la relación entre diferentes factores (como actividad física, consumo de frutas y verduras, hábito de fumar) y el riesgo de desarrollar diabetes u otras enfermedades como hipertensión o problemas cardíacos.
  • Clasificación de las personas en diferentes grupos de riesgo para enfermedades crónicas en función de hábitos y características demográficas.

Ejemplo:

  • Predicción: ¿Cuál es la probabilidad de que una persona desarrolle diabetes en función de variables como edad, actividad física, IMC, y consumo de frutas/verduras?
  • Segmentación: ¿Qué grupos de personas tienen más riesgo de padecer enfermedades cardíacas en función de su nivel de educación, ingresos y acceso a atención médica?

2. Explorar correlaciones y patrones entre variables

Una excelente manera de comenzar es realizando un análisis exploratorio de los datos (EDA). Podrías:

  • Explorar cómo se correlacionan las variables demográficas (edad, sexo, educación) con las variables de salud (diabetes, hipertensión, colesterol alto).
  • Visualizar distribuciones para ver si ciertos comportamientos o características son más comunes en grupos con enfermedades específicas.
  • Identificar factores protectores y factores de riesgo.

Ejemplo:

  • ¿Existe una correlación entre el nivel de ingresos y la probabilidad de tener acceso a atención médica y, por ende, un mejor control de la diabetes?

3. Elegir un modelo de predicción o segmentación

Una vez tengas claros los patrones y relaciones, puedes decidir qué tipo de análisis realizar. Algunas ideas:

  • Clasificación binaria: Como mencionaste, podrías usar todas las variables disponibles para predecir si una persona tiene diabetes o no. Este enfoque es directo y te permitirá probar diferentes algoritmos de Machine Learning.
  • Análisis de regresión: Para explorar qué variables influyen más en el desarrollo de condiciones como la diabetes o enfermedades cardíacas, podrías utilizar una regresión logística que te diga qué factores tienen un mayor peso en la predicción de esas enfermedades.
  • Análisis de clustering: Podrías usar técnicas de agrupamiento para identificar perfiles o clusters de personas con características similares. Esto podría ayudarte a descubrir subgrupos en la población que presentan mayor o menor riesgo de ciertas enfermedades.

4. Segmentación por población vulnerable

Puedes centrarte en identificar qué grupos de la población son más vulnerables en términos de salud, ya sea por ingresos, falta de acceso a atención médica, educación, o comportamientos de riesgo como fumar y consumo excesivo de alcohol.

Ejemplo:

  • ¿Cómo varía el riesgo de hipertensión en función del acceso a atención médica y el nivel educativo? ¿Las personas con menos recursos económicos tienen peor salud general?

5. Proponer acciones o políticas

El valor de tu proyecto puede ir más allá de la predicción de enfermedades. Puedes plantear sugerencias sobre cómo mejorar la salud pública basándote en los hallazgos de tu análisis. Podrías:

  • Identificar áreas donde la intervención (como campañas de salud o promoción de la actividad física) sería más efectiva para reducir el riesgo de enfermedades.
  • Proponer políticas de acceso a salud o programas educativos enfocados en los grupos que más lo necesitan.

6. Considerar la interpretabilidad del modelo

En un proyecto sobre salud, la interpretabilidad es clave. Si eliges modelos complejos como XGBoost o redes neuronales, considera incluir análisis adicionales que expliquen por qué el modelo tomó ciertas decisiones, como SHAP values o feature importance.

Resumen del proyecto planteado:

- Objetivo: Predecir si una persona es diabética usando factores de estilo de vida, salud y
  características demográficas.
- EDA: Analizar correlaciones, distribuciones y patrones entre las variables.
- Modelo: Clasificación binaria o regresión logística, quizás complementado con análisis de
  clustering.
- Resultados: Identificar los factores clave que predicen diabetes y hacer recomendaciones para
  políticas de salud pública o intervenciones específicas." 
