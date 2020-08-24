# Crítica: "BPR: Bayesian Personalized Ranking from Implicit Feedback"
Al igual que el otro paper, este documento comienza con la importancia de los sistemas recomendadores hoy en día, de que la mayoría de sus investigaciones son de feedback explícito y, sin embargo, abunda mucho más el feedback implícito.

Luego muestra los algoritmos que ya existen sobre el feedback implícito donde nombra *kNN CF* y el algoritmo basado en *Matrix factorization* que leímos en el primer paper. Explican que a diferencia de esos papers anteriores ellos van a directamente optimizar los parámetros de los modelos de ranking.

El algoritmo comienza a ordenar el rating final por medio de una relación lógica que separa los datos que tenemos observaciones de los que no tenemos observaciones, lo que nos llevará a dos ventajas:
1. Nos ayudará a separar el *training data* del *test data*.
2. Nos crea un subconjunto D<sub>S</sub> que nos servirá de *training data*.

Más adelante en el paper por medio de maximizar el *likelihood function* y del *BPR Optimization Criterion* logran generar un ranking personalizado por usuario. Al compararlo con la optimización *AUC*, muestran que la gran diferencia esta en el *loss function*.

Otra parte importante del documento es el algoritmo de aprendizaje, LearnBPR. Es un *stochastic gradient descent* que lo hacen de forma aleatoria para acelerar el proceso.

En los resultados, comparan un MF y un kNN con la optimización, dos MF extras, un *Cosine-kNN* y el algoritmo no personalizado, *most popular*. Resulta que para los dos *datasets* que usaron, los algoritmos con *BPR* son notablemente mejores.

Me gustó mucho que la optimización sea tan genérica y que se pueda aplicar a todos los sistemas recomendadores de ranking. Me hace pensar lo poderoso e importante que fue este paper en el área de investigación.

Los diagramas y gráficos ayudaron mucho a entender el algoritmo. Creo que son escenciales para entender lo que querían expresar, especialmente para un paper complejo como este.

También me gustó de que a pesar de ser matemática compleja, lograron modelar todo bastante bien y de forma ordenada, agregando las variables necesarias para entender su idea.

Sentí que en este paper se necesitaba un poco más de conocimiento del que yo tenía. Asumía que el lector sabía mucho terminos que yo no conocía y las matemáticas eran complejas. Esto hizo que le tuviera que dedicar más tiempo que los otros papers. De todas formas no concidero que esto sea malo, simplemente es una observación.

Me pareció un poco extraño el *dataset* de Netflix que usaron para experimentar el algoritmo, ya que en el contexto de sistemas recomendadores, me parece extraño que el ranking se base en la posibilidad de que el usuario haga un *rating* del item sin tener en cuenta si va a ser bueno o malo.

Otra cosa que me pareció extraño en el paper es que le dan un espacio a la explicación de *Maximum Margin Matrix Factorization* y sin embargo, no lo usan en la experimentación. Quedé con muchas ganas de ver su rendimiento en comparación a los otros algoritmos.

Para ir cerrando, me impresionó mucho este paper. Se nota que su optimización es bastante poderosa y que abarca un espectro muy amplio de algoritmos. A pesar de que era bastante complejo disfruté aprender con este documento.