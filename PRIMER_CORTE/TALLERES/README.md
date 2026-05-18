# ALGORTIMO DE BÚSQUEDAS INFORMADA Y EXPLORACIÓN

**ALGORITMO DE BÚSQUEDAS EN GRAFOS**

El siguiente trabajo consiste en la realización de un pequeño grafo en python con algoritmo de búsquedas en anchura (BFS) y la búsqueda en profundidad (DFS) los cuales son fundamentales para recorrer grafos. El algoritmo BFS explora los nodos nivel por nivel utilizando una cola, lo que permite encontrar el camino más corto en grafos no ponderados. Por otro lado, DFS explora cada rama del grafo hasta llegar al nodo más profundo antes de retroceder, utilizando una pila.

En las pruebas realizadas con el  grafo, BFS recorrió los nodos en orden por niveles (S, A, B, C, D, E, F), visitando primero el nodo inicial y luego todos los nodos del siguiente nivel antes de continuar con los demás. Por otro lado, DFS siguió una exploración en profundidad (S, B, E, F, A, D, C), avanzando lo más posible por una rama antes de retroceder para explorar las restantes. En cuanto al uso de memoria, BFS suele consumir más recursos porque mantiene en memoria todos los nodos del nivel actual en la cola, mientras que DFS generalmente utiliza menos memoria al explorar una sola rama a la vez mediante una pila.

Se realizó uso de las siguientes herramientas o librerías:

  **from collections import deque:** Se utiliza deque (double-ended queue) para implementar la cola del algoritmo BFS. Esto permite recorrer el grafo por niveles.
  **import matplotlib.pyplot as plt:** Sirve para crear las visualizaciones del grafo. Con esta librería se dibujan: los nodos, las conexiones y los pasos del                                               algoritmo. 

   * **`plt.figure()`**: crea una nueva gráfica.
   * **`plt.plot()`**: dibuja las conexiones entre nodos.
   * **`plt.scatter()`**: dibuja los nodos.
   * **`plt.text()`**: coloca las etiquetas (S, A, B, etc.).
   * **`plt.title()`**: título de los gráficos.
   * **`plt.axis('off')`**: oculta los ejes.

  **import imageio:**
    imageio se utiliza para generar archivos GIF a partir de varias imágenes. En este proyecto se usa para crear animaciones del recorrido
    de BFS y DFS uniendo las imágenes de cada paso.


  **from IPython.display import Image, display:** permite mostrar imágenes dentro de notebooks como Google Collab o Jupyter. Esto se usa para visualizar          directamente los pasos del recorrido del grafo sin tener que descargar las imágenes.

Las imágenes que representan cada paso de los recorridos BFS y DFS fueron generadas inicialmente mediante código en Python utilizando la librería matplotlib. Posteriormente, estas imágenes fueron descargadas y almacenadas en el repositorio de GitHub del proyecto. Para facilitar su visualización dentro del notebook en Google Colab, las imágenes se cargan directamente desde el repositorio utilizando las URLs en formato RAW de GitHub.

De esta manera, el notebook puede mostrar las visualizaciones sin necesidad de generar nuevamente las imágenes cada vez que se ejecuta el código.


En inteligencia artificial existen diferentes métodos que permiten a los sistemas **resolver problemas, encontrar soluciones eficientes y tomar decisiones estratégicas**.
Entre estos métodos destacan las **heurísticas**, la **teoría de juegos** y algoritmos de búsqueda como **A***, los cuales se utilizan ampliamente en áreas como videojuegos, robótica, sistemas de navegación y análisis estratégico.

---

# 1. Heurística

## ¿Qué es una heurística?

Una **heurística** es una estrategia o método práctico utilizado para **resolver problemas de forma más rápida**, especialmente cuando encontrar la solución exacta sería muy costoso en tiempo o recursos.

Las heurísticas **no siempre garantizan la solución óptima**, pero permiten encontrar **buenas soluciones en menor tiempo**.

## Características

* Reducen el **tiempo de búsqueda**.
* Permiten **priorizar las opciones más prometedoras**.
* Son útiles en problemas **muy grandes o complejos**.
* Se utilizan ampliamente en **algoritmos de inteligencia artificial**.

## Ejemplo

En un problema de búsqueda de rutas, una heurística puede ser **la distancia en línea recta entre dos puntos**, usada como estimación de qué tan cerca se encuentra el objetivo.

---

# 2. Búsqueda A*

## ¿Qué es la Búsqueda A*?

La **Búsqueda A*** es un algoritmo utilizado para **encontrar el camino más corto entre un punto inicial y un objetivo dentro de un grafo o mapa**.

Es uno de los algoritmos más utilizados en **inteligencia artificial y sistemas de navegación**.

Este algoritmo combina:

* El **costo real recorrido** desde el inicio.
* Una **estimación del costo restante** hasta el objetivo.

## Función de evaluación

El algoritmo utiliza la siguiente función:

f(n) = g(n) + h(n)

Donde:

* **g(n)** → costo real desde el nodo inicial hasta el nodo actual
* **h(n)** → estimación del costo desde el nodo actual hasta el objetivo (heurística)
* **f(n)** → valor total utilizado para decidir qué nodo explorar

El algoritmo siempre **expande el nodo con el valor de f(n) más pequeño**.

## Aplicaciones

La búsqueda A* se utiliza en:

* Videojuegos para movimiento de personajes
* Sistemas de navegación (GPS)
* Robótica
* Planeación de rutas
* Inteligencia artificial

---

# 3. Teoría de Juegos

## ¿Qué es la Teoría de Juegos?

La **teoría de juegos** es una rama de las matemáticas que estudia **la toma de decisiones estratégicas entre varios participantes**, donde el resultado de cada uno depende también de las decisiones de los demás.

Se utiliza para analizar situaciones de **competencia, cooperación o conflicto entre agentes**.

## Elementos de un juego

Un modelo de teoría de juegos generalmente incluye:

* **Jugadores**: quienes toman decisiones.
* **Estrategias**: posibles acciones que cada jugador puede elegir.
* **Resultados o recompensas (payoff)**: beneficios obtenidos según las decisiones tomadas.

## Tipos de juegos

### Juegos cooperativos

Los jugadores pueden colaborar para obtener mejores resultados.

### Juegos no cooperativos

Cada jugador busca maximizar su propio beneficio.

---

# 4. Aplicación en Inteligencia Artificial

En inteligencia artificial, la teoría de juegos se utiliza para **modelar situaciones donde un agente debe tomar decisiones considerando las posibles acciones de otros agentes o adversarios**.

Un ejemplo es el algoritmo **Minimax**, utilizado en juegos de estrategia.

## Ejemplos de aplicación

* Ajedrez
* Tres en raya (Tic-Tac-Toe)
* Juegos de estrategia
* Sistemas de toma de decisiones automáticas

---

# 5. Relación entre Heurística, A* y Teoría de Juegos

Estos tres conceptos están relacionados dentro del campo de la inteligencia artificial:

* Las **heurísticas** permiten evaluar rápidamente qué opciones parecen más prometedoras.
* **A*** utiliza heurísticas para encontrar rutas óptimas de manera eficiente.
* La **teoría de juegos** modela la toma de decisiones cuando existen varios agentes o adversarios.

En muchos sistemas de inteligencia artificial, **estos métodos se combinan** para mejorar la eficiencia y la calidad de las decisiones.

---

### Pasos para ejecutar el proyecto
1. **Da clic en el enlace del proyecto**.
2. **Una vez dentro del colab**.
3. **Clic izquierdo en **Conectar** (esquina superior derecha) y, por último, clic en Ejecutar todas**.

 
ENLACE DEL PROYECTO:
* https://colab.research.google.com/drive/1CvckgRLR-2HDRxhPK_ucPyPZUItRuuwe
* https://colab.research.google.com/drive/1w1cExEiG2DbuU3V5-2KOQA4XuyFn9epB?usp=sharing


      
    
