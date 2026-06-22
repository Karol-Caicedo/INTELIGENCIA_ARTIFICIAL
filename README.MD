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

