# Taller Práctico: NumPy y Análisis Exploratorio de Datos para Inteligencia Artificial

## Descripción

Este proyecto tiene como objetivo fortalecer los conocimientos en el uso de la biblioteca **NumPy** para la manipulación y análisis de datos numéricos en Python. Además, se desarrollan actividades relacionadas con estadísticas descriptivas, generación de datos sintéticos y visualización de información, herramientas fundamentales en Ciencia de Datos, Machine Learning e Inteligencia Artificial.

---

## Objetivos

### Objetivo General

Aplicar los conceptos fundamentales de NumPy para el procesamiento, análisis y visualización de datos orientados a la Inteligencia Artificial.

### Objetivos Específicos

* Comprender la estructura y funcionamiento de los arreglos multidimensionales (ndarray).
* Realizar operaciones matemáticas y estadísticas utilizando NumPy.
* Generar datos sintéticos mediante distribuciones probabilísticas.
* Interpretar medidas estadísticas descriptivas.
* Analizar gráficamente el comportamiento de los datos.
* Identificar patrones asociados a posibles eventos de fraude mediante análisis exploratorio.

---

## Tecnologías Utilizadas

* Python 3.x
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Google Colab

---

## Actividades Desarrolladas

### 1. Investigación sobre NumPy

Se realizó una investigación sobre la biblioteca NumPy, destacando sus principales características:

* Manejo eficiente de grandes volúmenes de datos.
* Soporte para arreglos multidimensionales.
* Operaciones matemáticas vectorizadas.
* Funciones estadísticas integradas.
* Base fundamental para bibliotecas como Pandas, Scikit-Learn y TensorFlow.

---

### 2. Manipulación de Arreglos

Se trabajó con matrices y arreglos multidimensionales utilizando técnicas de indexación y segmentación para acceder a elementos específicos de las estructuras de datos.

---

### 3. Estadística Descriptiva

Se calcularon indicadores estadísticos fundamentales:

* Promedio (Media)
* Valor máximo
* Valor mínimo
* Desviación estándar

Estos indicadores permiten comprender la tendencia central y la dispersión de los datos analizados.

---

### 4. Generación de Datos Sintéticos

Se generaron 1.000 observaciones aleatorias mediante una distribución normal con:

* Media = 50
* Desviación estándar = 10

Este procedimiento permite simular escenarios reales utilizados en el entrenamiento y validación de modelos de Inteligencia Artificial.

---

### 5. Visualización de Datos

Se utilizaron histogramas y gráficos de dispersión para analizar el comportamiento de los datos y facilitar la identificación de patrones.

---

# Análisis Exploratorio de Fraude Financiero

Para complementar el estudio, se realizó un análisis exploratorio sobre un conjunto de datos relacionado con transacciones financieras y detección de fraude.

Las variables estudiadas fueron:

* Valor_Transaccion
* Hora_Del_Dia
* Numero_Transacciones_Diarias
* Distancia_Geografica
* Fraude (Sí / No)

---

## Interpretación del Pairplot

El Pairplot permite visualizar simultáneamente la distribución de cada variable y la relación existente entre ellas, diferenciando las observaciones según la categoría de fraude.

### Valor de la Transacción

Se observa que las transacciones catalogadas como fraudulentas presentan una tendencia hacia valores monetarios más altos en comparación con las transacciones legítimas.

Sin embargo, existe una zona de superposición entre ambas categorías, indicando que el valor de la transacción no es suficiente por sí solo para determinar un fraude.

**Interpretación:** Los montos elevados pueden incrementar la probabilidad de fraude, pero deben analizarse junto con otras variables.

---

### Hora del Día

La distribución de las transacciones durante las diferentes horas del día es relativamente uniforme para ambas categorías.

No se evidencia una concentración significativa de fraudes en horarios específicos.

**Interpretación:** La hora de la transacción tiene una influencia limitada como variable predictora dentro de este conjunto de datos.

---

### Número de Transacciones Diarias

Los registros clasificados como fraude tienden a aparecer con mayor frecuencia cuando el número de transacciones realizadas durante el día es elevado.

**Interpretación:** Una actividad transaccional inusualmente alta puede representar un comportamiento sospechoso y convertirse en un indicador de riesgo.

---

### Distancia Geográfica

Esta variable presenta una de las diferencias más claras entre los grupos analizados.

Las transacciones fraudulentas suelen registrarse a mayores distancias geográficas, mientras que las transacciones legítimas se concentran en distancias menores.

**Interpretación:** Los cambios geográficos significativos pueden ser un factor importante para detectar posibles actividades fraudulentas.

---

## Relación entre Variables

Los diagramas de dispersión muestran que no existen relaciones lineales fuertes entre las variables analizadas.

La dispersión observada sugiere que el fraude no depende de una única característica, sino de la combinación de múltiples factores.

Las variables que presentan mayor capacidad para diferenciar transacciones fraudulentas de las legítimas son:

* Valor_Transaccion
* Numero_Transacciones_Diarias
* Distancia_Geografica

# Conclusiones

## 1. El valor de la transacción es un factor relevante para la detección de fraude

El análisis realizado permitió identificar que las transacciones clasificadas como fraudulentas presentan una tendencia a concentrarse en montos más elevados que las transacciones legítimas. Esto sugiere que el valor económico de una operación puede constituir una señal de alerta importante para los sistemas de monitoreo financiero.

---

## 2. La frecuencia de transacciones diarias influye en la identificación de comportamientos sospechosos

Se evidenció que los registros asociados a fraude suelen presentar una mayor cantidad de transacciones realizadas durante un mismo día. Este comportamiento podría indicar intentos de aprovechar múltiples operaciones antes de que los mecanismos de seguridad detecten la actividad irregular.

---

## 3. La distancia geográfica es una de las variables con mayor capacidad predictiva

Los resultados muestran que las transacciones fraudulentas tienden a realizarse desde ubicaciones geográficas más distantes en comparación con las operaciones legítimas. Esto demuestra que los cambios abruptos en la ubicación de las transacciones pueden ser un indicador importante para la detección temprana de fraude.

---

## 4. La hora del día tiene una influencia limitada en la detección de fraude

El análisis exploratorio mostró que las transacciones fraudulentas y legítimas se distribuyen de manera relativamente uniforme a lo largo de las diferentes horas del día. Por lo tanto, esta variable presenta una capacidad limitada para diferenciar entre ambos tipos de transacciones cuando se analiza de forma individual.

---

## 5. La detección efectiva de fraude requiere la combinación de múltiples variables

Ninguna de las variables analizadas logró separar completamente los casos de fraude de los casos legítimos. Esto evidencia que la identificación de actividades fraudulentas depende de la interacción entre diferentes factores, por lo que resulta necesario emplear modelos analíticos capaces de evaluar múltiples características simultáneamente.

---

## 6. El análisis exploratorio de datos facilita la identificación de patrones de riesgo

La utilización de herramientas estadísticas y de visualización permitió identificar tendencias y comportamientos relevantes dentro del conjunto de datos. Esto demuestra que el análisis exploratorio constituye una etapa fundamental para comprender los factores asociados al fraude financiero y apoyar la toma de decisiones basada en datos.

---

# Recomendaciones Empresariales

## 1. Implementar sistemas automáticos de alerta basados en niveles de riesgo

La entidad bancaria debería configurar alertas automáticas para transacciones que superen determinados umbrales de valor o que presenten características inusuales, como una alta frecuencia de operaciones o ubicaciones geográficas atípicas. Esto permitiría actuar de forma preventiva y reducir posibles pérdidas económicas.

---

## 2. Incorporar modelos de Machine Learning para la detección de fraude

Se recomienda implementar algoritmos de aprendizaje automático capaces de analizar múltiples variables simultáneamente y asignar una probabilidad de riesgo a cada transacción. Esta estrategia permitiría mejorar la precisión en la identificación de operaciones fraudulentas y optimizar los procesos de monitoreo.

---

## 3. Fortalecer los mecanismos de autenticación para operaciones de alto riesgo

Cuando una transacción presente características sospechosas, la entidad debería solicitar mecanismos adicionales de validación, tales como autenticación multifactor, códigos de verificación o confirmaciones mediante aplicaciones móviles. Esto contribuiría a reducir el riesgo de accesos no autorizados.

---

## 4. Implementar monitoreo continuo del comportamiento de los clientes

La creación de perfiles de comportamiento transaccional permitiría detectar desviaciones significativas respecto a los hábitos habituales de cada usuario. Este enfoque facilitaría la identificación temprana de posibles eventos de fraude y mejoraría la capacidad de respuesta de la organización.

---

## 5. Capacitar al personal en análisis de datos y prevención de fraude

Es recomendable fortalecer las competencias del personal encargado de la gestión de riesgos mediante programas de formación en análisis de datos, ciberseguridad e Inteligencia Artificial. Esto permitirá una mejor interpretación de las alertas generadas por los sistemas automatizados y una toma de decisiones más eficiente.

---

# Aplicación de Machine Learning e Inteligencia Artificial

## ¿Cómo podrían utilizarse técnicas de Machine Learning o Inteligencia Artificial para automatizar la toma de decisiones en este caso?

Las técnicas de Machine Learning e Inteligencia Artificial pueden utilizarse para automatizar la detección de fraude mediante el análisis continuo de las transacciones financieras en tiempo real. A partir de variables como el valor de la transacción, la cantidad de operaciones realizadas por un usuario, la distancia geográfica y otros factores relevantes, los modelos pueden aprender patrones de comportamiento normales y diferenciarlos de actividades potencialmente fraudulentas.

Algoritmos de clasificación supervisada como:

- Regresión Logística
- Árboles de Decisión
- Random Forest
- Redes Neuronales

pueden entrenarse utilizando datos históricos previamente etiquetados como **Fraude** y **No Fraude**. Una vez entrenados, estos modelos son capaces de evaluar automáticamente cada nueva transacción y asignar una probabilidad de riesgo.

Cuando una operación supera un nivel determinado de riesgo, el sistema puede ejecutar acciones automáticas como:

- Generar alertas para el área de seguridad.
- Solicitar autenticación adicional al cliente.
- Retener temporalmente la transacción para validación.
- Bloquear preventivamente operaciones sospechosas.

Adicionalmente, técnicas de aprendizaje no supervisado como:

- Clustering
- Detección de anomalías
- Isolation Forest

permiten identificar patrones inusuales incluso cuando no existen ejemplos previos de fraude registrados en la base de datos.

La implementación de estas tecnologías permite a las entidades bancarias mejorar la precisión en la detección de fraude, reducir pérdidas económicas, optimizar los tiempos de respuesta y fortalecer la seguridad de los clientes mediante procesos de decisión automatizados basados en datos.

---

## Conclusiones

* NumPy es una herramienta fundamental para el procesamiento eficiente de datos numéricos.
* Las medidas estadísticas descriptivas permiten comprender el comportamiento general de un conjunto de datos.
* La generación de datos sintéticos facilita la simulación de escenarios utilizados en Inteligencia Artificial.
* La visualización de datos permite identificar patrones y tendencias que no son evidentes a simple vista.
* En el análisis de fraude, las variables relacionadas con el valor de la transacción, la frecuencia de operaciones y la distancia geográfica mostraron mayor relevancia para la identificación de comportamientos sospechosos.
* La detección de fraude requiere el análisis conjunto de múltiples variables, lo que justifica el uso de técnicas de Machine Learning para mejorar la precisión de los modelos predictivos.

---

## Integrantes

* Karol Caicedo
* Luisa Fernanda
* Elkin Andrés Chalarca
* Dairon Valencia

---

## Licencia

Este proyecto fue desarrollado con fines académicos para el fortalecimiento de competencias en Ciencia de Datos e Inteligencia Artificial.

