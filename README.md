# INTELIGENCIA_ARTIFICIAL

**ALGORITMOS DE BÚSQUEDA EN GRAFOS**

El siguiente trabajo consiste en la realización de un pequeño grafo en python con algoritmos de búsqueda en anchura (BFS) y la búsqueda en profundidad (DFS) los cuales son fundamentales para recorrer grafos. El algoritmo BFS explora los nodos nivel por nivel utilizando una cola, lo que permite encontrar el camino más corto en grafos no ponderados. Por otro lado, DFS explora cada rama del grafo hasta llegar al nodo más profundo antes de retroceder, utilizando una pila.

En las pruebas realizadas con el  grafo, BFS recorrió los nodos en orden por niveles (S, A, B, C, D, E, F), visitando primero el nodo inicial y luego todos los nodos del siguiente nivel antes de continuar con los demás. Por otro lado, DFS siguió una exploración en profundidad (S, B, E, F, A, D, C), avanzando lo más posible por una rama antes de retroceder para explorar las restantes. En cuanto al uso de memoria, BFS suele consumir más recursos porque mantiene en memoria todos los nodos del nivel actual en la cola, mientras que DFS generalmente utiliza menos memoria al explorar una sola rama a la vez mediante una pila.
