# Crítica: Collaborative Filtering for Implicit Feedback Datasets
Este paper comienza explicando de que la mayoría de las investigaciones existentes sobre sistemas recomendadores son de feedback explícito y, sin embargo, no siempre son accesibles. Aquí entra la importancia del feedback implícito, ya que a diferencia del explícito, es mucho más abundante y seguro de conseguir.

Luego hablan de las principales características del feedback implícito:
1. No existe el feedback negativo. Esto se debe a que es muy difícil inferir que algo no le gusta solo por la carencia de una acción. Pueden haber muchas explicaciones y no necesariamente es por disgusto. 
2. La información implícita es muy ruidosa. La cantidad de observaciones no aseguran que sea por gusto y pueden darse situaciones en la que no es información del usuario.
3. La interpretación de la cantidad de observaciones no nos da información sobre los gustos del usuario, si no que nos da información de la recurrencia de la acción.
4. La evaluación de la recomendación implícita no se puede medir de la misma forma que una recomendación explícita.

Después explican su algoritmo con sus principales variables: preferencia y confianza. En un inicio definen la preferencia como una variable binaria que nos indica si hay observaciones o no. La confianza es la variable que nos indicará la certeza que hay sobre la preferencia. Luego nos dan la solución de cómo optimizar el algoritmo para que no exista una complejidad tan alta.

Otra parte importante de su algoritmo es cómo agregar una explicación a la recomendación. Explican que la preferencia adquirida por el item recomendado se puede ver como un producto punto entre la semejanza de los items y la confianza de cada uno. En la sumatoria del producto punto se puede revisar cuáles fueron los items que más aportaron y de ahí concluír de adonde vino la recomendación.

Para terminar, comparó un SVD y un *kNN Item-based* con el algoritmo presentado en el paper. Los resultados fueron bastante positivos y se ve claramente que el algoritmo nuevo tiene mejores resultados que los que ya existían.

Me gustó mucho este paper, me logró convencer sobre la importancia de sacar información del feedback implícito. Encontré que el documento era muy ordenado lo que me permitió entenderlo muy bien. Los gráficos tenían título, nombre de ejes y leyenda, lo que aportó enormemente a entender los resultados. También e gustó mucho la introducción. Dejaban todos los términos bien definidos para luego usarlos. Se agradece mucho una introducción completa.

Me habría gustado que usaran más de un *database* para afirmar su conclusión de que su algoritmo es efectivamente mejor que los que ya existían. También me habría gustado que su *"success"* en la explicación de la recomendación fuera más objetivo y no solamente una mirada a los resultados.

Para ir cerrando, me gustó mucho este paper. Me hizo aprender mucho y me deja con muchas ganas de seguir a prendiendo sobre esta área de la computación. Encuentro que por su completitud, es un muy buen documento para alguien que está entrando en el mundo de los sistemas recomendadores.