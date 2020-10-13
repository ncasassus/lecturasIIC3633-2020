# Comentario: Multi-Armed Recommender System Bandit Ensembles
## Resumen
En este paper se propone un método de *ensembles* con una perspectiva más "realista" a los que se han investigado últimamente. Creen que debe ser un proceso más cíclico con la posibilidad de observar y aprender la efectividad de la combinación de algoritmos.

En la introducción hablan de que la busqueda a maximizar la efectividad de los sistemas recomendadores, rapidamente convergió a combinar varios algoritmos que se potenciaran creando estos *ensembles*. Pero también nos dicen que siempre se han investigado con un problema: son muy simplificados y, *testean* y comparan con una no-interactiva corrida de código.

Es por eso, para solucionar este problema, propenen este *multi-armed bandit* que contiene un proceso cíclico donde se da la posibilidad de observar, de aprender y de mejorar el rendimiento del recomendador.

En *related work* nos cuentan un poco sobre cómo se han llevado a cabo los *ensembles* y los *bandit* en los sistemas recomendadores hasta el momento, para luego introducirnos los *Bandit Recommender System Ensembles*. En esta parte nos enseñan los términos más básicos de este tipo de recomendadores y nos dan una breve explicación de los algoritmos que se usarán para probar la idea principal del paper: *$\epsilon$-greed* y *Thompson sampling*.

Para el experimento usan el clásico dataser de *Movielens*. Para entrenar los algoritmos comenzarán solo con el 5% de los datos, para usar el resto como *user feedback*.

Los resultados fueron bastante positivos para los recomendadores *bandit ensembles* y superan por bastante a los algoritmos clásicos como *kNN* y *Matrix Factorization*, pero también superan por mucho al *dynamic ensemble* que luego explican que puede ser debido al sesgo a favor del algoritmo que recolectó los *ratings*.

Terminan concluyendo que de que los *Bandit Recommender System Ensembles* son bastante mejores a todos los otros algoritmos que compararon, no solo por si eficiencia empírica si no que también porque tiene un costo computacional mucho menor.

## Opinión
En mi opinión, este paper parece tener un contenido muy potente e infuyente en cómo se hacen los *ensembles* en los sistemas recomendadores. Dejan bastante en claro que supera por bastante a otros algoritmos muy conocidos como: *kNN* y *Matrix Factorization*.

No me había dado cuenta hasta el final del documento que un importante punto a favor de los *bandit ensembles* es su bajo costo computacional, ya que necesitan correr solo un algortimo de recomendación elegido.

Me gustó mucho su elección del experimento porque prueban con más de un *bandit ensemble* probando que no era la casualidad del algoritmo. Eso si quizás hubiera sido aún más enriquecedor el usar más de un dataset.

El paper es bastante corto y no es complicado, sin embargo logran explicar sus ideas muy bien. Esto permite que sea muchísimo más fácil de entender.

Para ir cerrando, me gustó mucho el paper. Sentí que su contenido es super influyente en cómo funcionan los sistemas recomendadores hoy en día. Encontré muy curioso que una idea tan buena cómo hacer *ensembles* recursivos apareciera recién en 2019 y no antes, pero que sea actual me motiva mucho más.