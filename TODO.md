## TODO: Continuar con el análisis del balanceo artificial de clases

### Ventajas del Balanceo Artificial
1. **Mejora el rendimiento en clases minoritarias**:
   - Al balancear, hago que el modelo **dé más atención a ambas clases** en lugar de centrarse en la clase mayoritaria.
   - Esto me permite obtener **métricas más equilibradas** y evaluar mejor el rendimiento en todas las clases.
2. **Evita el sesgo hacia la clase mayoritaria**:
   - En conjuntos desbalanceados, el modelo tiende a predecir la clase mayoritaria con más frecuencia.
   - Esto puede aumentar la **accuracy**, pero no siempre refleja la capacidad del modelo para identificar correctamente las clases minoritarias.

### Desventajas del Balanceo Artificial
1. **No representa la realidad**:
   - Un conjunto de datos balanceado no refleja la **distribución real** que probablemente encontraría en situaciones prácticas.
   - Esto podría llevar a que el modelo **rinda bien en un conjunto balanceado**, pero no tan bien cuando se enfrenta a datos desbalanceados del mundo real.
2. **Posible sobreajuste en la clase minoritaria**:
   - Al incluir más muestras de la clase minoritaria, el modelo puede **sobreajustarse a patrones específicos** de esta clase.
   - En situaciones reales, donde estas muestras son menos comunes, es posible que el modelo **no generalice adecuadamente**.
3. **Evaluación limitada**:
   - Con un conjunto de datos balanceado artificialmente, se dificulta evaluar cómo el modelo manejará datos **desbalanceados** en la práctica.
   - Las métricas de precisión y recall pueden ofrecer una visión del rendimiento, pero **no brindan una imagen completa**.

### Implicaciones para el Modelo
- Entrenar el modelo en el DataFrame balanceado me permite **comparar y evaluar sin el sesgo del desbalance**.
- Si el objetivo es crear un modelo aplicable a situaciones reales (por ejemplo, donde el diagnóstico de diabetes es menos común que la ausencia de diabetes), será importante **validarlo también en un conjunto desbalanceado**.

### Pasos a Considerar para Mañana
- **Evaluar el modelo en ambos contextos** (balanceado y desbalanceado) para observar cómo se adapta a diferentes escenarios.
- Si quiero un modelo que sea útil en situaciones reales, **entrenarlo en datos desbalanceados** pero ajustando el parámetro `class_weight` para mejorar la capacidad de identificar clases minoritarias.
- Considerar que, aunque el balanceo es útil para experimentar y observar el rendimiento, **mantener la representación natural de los datos es crucial para crear un modelo robusto en aplicaciones prácticas**.

### Checklist
- [ ] Evaluar el modelo en el contexto desbalanceado.
- [ ] Evaluar el modelo en el contexto balanceado.
- [ ] Probar el ajuste de `class_weight` en un modelo desbalanceado.
- [ ] Comparar los resultados de ambos modelos y documentar las observaciones.