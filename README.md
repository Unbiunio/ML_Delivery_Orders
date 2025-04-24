El Objetivo de este ejercicio es saber predecir si los 10 pedidos de df_pred se van a entregar o no

En este ejercicio hemos aprendido un par de cosas relevantes y a tener en cuenta en futuros datasets

Hemos aprendido a trabajar con variables cíclicas en este caso, las horas de pedido. que si las tratasemos de forma lineal nuestro modelo podria pensar que las 12h esta alejada 12 puntos de la 1 cuando en realidad son contiguas. Para ello hemos usado la regla del seno y el coseno. Para mas información visitar:
https://aukera.es/blog/variables-ciclicas/

Y también hemos aprendido el porque de usar TargetEncoder que sustituye una variable categórica por la media del valor de la variable objetivo (target) para cada categoría.

 Hemos también aprendido el parámetro "Smoothing". En nueestro caso como la mayoría de las tiendas tienen pocas observaciones, este es el método ideal. El TargetEncoder con smoothing da más peso a la media global si la tienda tiene pocas entregas.