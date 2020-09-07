# Comentario: Contets-Based Recommendation Systems
## Resumen

En este capítulo se discute sobre los *content-based recommendation systems*. Estos sitemos son los que se le recomienda un *item* a un usuario basado en la descripción del producto y en las preferencias del usuario.

En la introducción hablan de lo común que es econtrarse con ezte tipo de sistemas recomendadores. También escriben sobre los dos tipos de datos que se pueden encontrar, *structed data* y *unstructed data*. El primero se maneja generalmente con tablas, en cambio el segundo es un poco más complicado porque hay que modificar los datos para que se puedan estructurar y poner en tablas.

Luego hablan de los perfiles de los usuarios y sus preferencias. Explican que hay principalmente dos fuentes de información:

1. Las preferencias del usuario: Básicamente consiste en tomar las descripciones de los items que le interesan al usuario.
2. Las interacciones del usuario: Consiste en usar lo que el usuario ha hecho anteriormente. Puede ser desde busquedas hasta información más explícitas como la compre de un producto.

Para aprender los perfiles de los usuario se trata de clasificar el *training data* en una variable binaria como "Le gusta" y "No le gusta" y luego por medio del entrenamiento de algortimos se puede predecir la clasificación de un producto al que no sabemos la opinión del usuario.

Después de pasar por 5 algoritmos de sistemas recomendadores basados en contenido, el capítulo termina con las limitaciones y extenciones de este tipo de algoritmos.

## Opinión

Este capítulo es bastante completo y abarca mucha información sobre los *content-based recommendation systems*, por lo que es muy bueno si quieres saber una pincelada del tema o quieres repasar sobre algún termino o algoritmo. Pero si quieres saber más a detalle sobre el área es probable que te quedes corto, por ejemplo, hay algoritmos super potentes y muy interesantes como el SVM que solo le dedican 3 parrafos.

Personalmente, me gustó harto. Creo que es muy ordenado y explica de forma compacta y correcta. Pude notar esto con los algoritmos que ya conocía, y me impresionó que con un par de parrafos los lograba explicar bien.

Me gustó aprender sobre cómo se manejan los datos no estructurados, e.g., los textos. Encontré bastante impresionante como logró transformar un texto como el de la tabla 10.2 en palabras ordenadas por su repetición en el texto.

También me gustó que al final del capítulo escribiera sus limitaciones y de cómo se utilizan hoy en día. Da una buena imágen de qué tan poderosos son, sin quedar con una idea sobre-valorada o infra-valorada.

Se que quizás no era el enfoque del capítulo, pero me habría encantado ver una comparación de resultados entre los algoritmos con distintos datasets. Así uno podría haber quedado con alguna idea de cuándo utilizar los distintos tipos de algoritmos y si hay alguno que es indudablemente mejor.

Para ir cerrando, creo que es un capítulo muy educativo que se aprende un espectro muy grande de los *content-based recommendation systems*. Es un texto que es bastante simple como para alguien que no sabe mucho del tema, pero lo suficientemente importante para que lo pueda leer cualquiera para repasar terminos o algoritmos sin tener que pasar por matemática y demostraciones muy complicadas.