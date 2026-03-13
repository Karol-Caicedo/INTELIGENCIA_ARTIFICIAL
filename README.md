# INTELIGENCIA_ARTIFICIAL

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


### Pasos para ejecutar el proyecto
1. **Descargar** el archivo de la carpeta `ALGORITMO_PYTHON`.
2. **Abre tu Drive** y da clic en **Nuevo** > **Subir archivo**.
3. **Selecciona** el archivo descargado, haz clic en **Abrir** y espera a que cargue.
4. Clic en **Recientes** y doble clic izquierdo en el archivo para abrirlo.
5. Clic izquierdo en **Conectar** (esquina superior derecha) y, por último, clic en **Ejecutar todas**.
 

ENLACE DEL PROYECTO:
https://drive.google.com/file/d/1CvckgRLR-2HDRxhPK_ucPyPZUItRuuwe/view?usp=sharing


      
    
