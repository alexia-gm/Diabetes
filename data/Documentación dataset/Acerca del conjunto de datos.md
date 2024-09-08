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
