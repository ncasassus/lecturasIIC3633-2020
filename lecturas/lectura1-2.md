# Crítica: "Netflix Update: Try This at Home"
Este documento no es precisamente un paper, resulta ser una especie de blog. Es muy interesante, lo relata uno de los que sacó el tercer lugar en el Netflix Price. Durante el documento va explicando cómo funciona el algoritmo que usó para sacar ese lugar.

Su algoritmo es un tipo de *singular value descomposition (SVG)*. Los *SVG* son algoritmos en el logran disminuir la cantidad de entradas de una tabla gigante en 2 tablas más pequeñas. Esto lo logra minimizando la cantidad de atributos para describir un item.

Ahora, lo innovador de su algoritmo lo podríamos resumir en dos partes. Primero, logra dar una recomendación básica previo al *SVG* que consisten en la suma de los promedios de los *ratings* del item y el promedio de los *offset's* del usuario.

En segundo lugar, calcula un valor temporal a los valores que están en blanco luego de haber ejecutado el *SVG*. Para luego pasar los valores por una función que lo evaluará en el rango del *rating*.

Me pareció muy interesante este blog porque agrega lo que yo sentí que le faltó al otro paper, relacionar los items con más información que solo el *rating*. Además me gusta mucho que el algoritmo se haya creado en una situación practica: en el Netflix Price.

Eso si me pareció que era bastante desordenado, por lo que tuve que dedicarle más tiempo para entender el documento. Tampoco me gustaron los gráficos, le faltaron los títulos y los nombres de los ejes. La verdad es que no eran tan fáciles de ver. 

De forma más general, me gustó mucho el documento. Aprendí mucho, especialmente sobre cómo compactar información con menos entradas. También me hizo recordar un poco de probabidad y estádistica que no tenía hace tiempo.

