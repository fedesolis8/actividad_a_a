# Actividad 5: Comparación de Clasificadores K-NN y Árbol de Decisión

## Introducción
En esta actividad, se utilizó el dataset **"Wine"** de `scikit-learn` para resolver un problema de clasificación. El objetivo es predecir a cuál de las tres clases pertenece un vino basándose en sus características químicas. Se implementaron y compararon dos algoritmos de aprendizaje supervisado: K-Nearest Neighbors (K-NN) y Árbol de Decisión, siguiendo la consigna de la Clase N° 5 de Aprendizaje Automático.

## Resultados Obtenidos
La precisión de cada modelo, evaluada sobre el conjunto de datos de prueba, fue la siguiente:

-   **Precisión del Modelo K-NN (k=5):** 0.7222
-   **Precisión del Modelo de Árbol de Decisión (max_depth=3):** 0.9444

## Análisis y Comparación

Los resultados muestran una diferencia de rendimiento considerable entre los dos modelos para este conjunto de datos.

-   **Árbol de Decisión:** Con una precisión del **94.44%**, este modelo demostró ser extremadamente efectivo y robusto para clasificar los vinos. Una de sus mayores ventajas es la **interpretabilidad**. Sería posible visualizar el árbol para entender las reglas exactas que el modelo aprendió para tomar sus decisiones (por ejemplo, "si el nivel de alcohol es mayor a X y el color es menor que Y, entonces pertenece a la clase 0").

-   **K-NN:** Este modelo alcanzó una precisión del **72.22%**, un resultado notablemente inferior. Esto sugiere que la simple proximidad entre los puntos (basada en la distancia euclidiana por defecto) no fue suficiente para capturar la complejidad de la separación entre las clases de vino. Si bien su concepto es simple, su rendimiento fue limitado en este caso.

## Conclusión
Para el problema de clasificación del dataset "Wine", el **Árbol de Decisión es claramente el modelo superior**, ofreciendo no solo una mayor precisión predictiva sino también la ventaja de ser un modelo interpretable.

Como próximos pasos para mejorar el rendimiento del modelo K-NN, se podría realizar una búsqueda del valor óptimo de `k` (en lugar de usar `k=5` por defecto) y aplicar un escalado de características a los datos, ya que K-NN es sensible a las diferentes escalas de las variables.
