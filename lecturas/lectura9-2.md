# Comentario: Carousel Personalization in Music Streaming Apps with Contextual Bandits
## Resumen
En este paper se profundiza en la visualizacion de "carruseles", donde empíricamnete se muestran las eficiencias de cada caracterísitca de los "carruseles" en la vida real.

En la introducción se habla de lo crucial que se han convertido las recomendaciones personalizadas en los distintos servicios, y que en consecuencia muchas de las investigaciones del área inician con aspectos de aplicaciones industriales. Muchas de las aplicaciones a nivel mundial usan estos "carruseles" y es por eso que en este paper modelan el problema de *multi-armed bandit with multiple plays* en esta visualización.

Luego explican más o menos en que consiste este *multi-armed bandit with multiple plays* para luego explicar su relación con los carruseles. En pocas palabras, hay un conjunto K que representa a todos los items, el conjunto L que son los items que irían dentro del carrusel y el conjunto N de usuarios. Si el usuario aprenta uno de los items dentro del carrusel, entonces ese item tendría puntaje 1 y en caso contrario, 0.

El problema de la modelación anterior es que el costo computacional es altísimo, por lo que presentan de forma rápida 2 algoritmos: *Semi-Personalization via User Clustering* y *Constextual Multi-Armed Bandits*.

En el paper agregaron el supuesto de que no todos los usuarios ven todos los items que se encuentran en el carrusel y que las actualizaciones de las preferencias de cada usuarios tienen un *delay*.

Para el experimento usaron un dataset muy grande de Deezer, con $K = 862$ y $N = 974960$. El carrusel puede tener hasta 12 items e inicialmente solo muestra 3. Para comparar entre los distintos algoritmos, agregaron un total de 10 al experimento los cuales todos tienen distintas características que ayudarán a sacar conclusiones.

Los resultados para el experimento *offline* nos muestran que los algoritmos que son *semi-personalization* y *no-cascade* tienen un mejor rendimiento con *user clustering*. Sin embargo, para el experimento *online* no se pudo ver lo mismo sobre el *no-cascade* pero si se vió con el *semi-personalization*.

## Opinión
Es interesante el foco del paper, si no me equivoco es el segundo que leemos que involucra una empresa conocida como Deezer. Esto hace que inicie el documento con mucha curiosidad y más atento.

Encontré que era un texto muy completo, con una buena explicación sobre cómo va a hacer el experimento y cómo llegaron a eso. Explicaron muy bien el modelo y los dos algoritmos que usaron para la información contextual del usuario.

También siento que el experimento está bien hecho, con muchísimos algoritmos y con una base da datos bastante grande. Para esta ocasión no encuentro necesario usar más de una base de datos porque se estaban enfocando solamente en Deezer.

Me gustó mucho el supuesto que agregaron de que no todos los usaurios ven todos los items del "carrusel", creo que es muy real.

Me gustó la gran variedad de algoritmos que usaron para representar las distintas características que existen, pero a su vez lo encontré un poco confuso. Creo que me faltó una tabla resumen que relacione los algoritmos con las características ya que me costaba mucho la transición de ver los resultados a concluír los versus de las características.

Para ir cerrando, me gustó harto el paper. Me pareció muy interesante que viniera del mundo industrial. También me gustó leer sobre los "carruseles" que siento que son muy comunes hoy en día y se ven en la mayoría de las aplicaciones. Todo esto ayudó que se me hiciera muy fácil leer el texto.