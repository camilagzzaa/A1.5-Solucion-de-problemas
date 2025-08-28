# A1.5 - Solución de problemas (Calificaciones)

## Índice
1. [Dataset](./A1.5%20Calificaciones.csv)
2. [Notebook](./A1.5%20Solución%20de%20problemas.ipynb)
3. [Reporte HTML](./A1.5%20Solución%20de%20problemas.html)
4. [README](./README.md)

---

## Descripción

Este proyecto implementa un modelo de regresión lineal múltiple con datos de estudiantes, cuyo objetivo es predecir la calificación final (G3) a partir de información académica y demográfica como edad, horas de estudio, materias reprobadas, acceso a internet, faltas y calificaciones de los dos primeros periodos (G1 y G2). 

El código carga el dataset, transforma las variables categóricas en variables dummy, identifica y elimina outliers en la variable de faltas usando el método de Tukey, analiza posibles problemas de colinealidad mediante una matriz de correlaciones, crea términos de interacción entre variables y entrena un modelo con el 80% de los datos para validarlo en el 20% restante. Los coeficientes se calculan mediante la fórmula matricial de mínimos cuadrados ordinarios expresada como: el vector de coeficientes es igual al producto de la pseudo-inversa de la matriz de variables por el vector de valores de la variable dependiente. 

Finalmente, se presenta la fórmula expandida del modelo con sus coeficientes y se evalúa el desempeño a través de una gráfica que compara calificaciones reales contra calificaciones estimadas en el conjunto de prueba. 

Se utilizan únicamente las librerías pandas, numpy y matplotlib.
