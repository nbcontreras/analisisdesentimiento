# Análisis de Sentimiento Libre de Contexto
  Existen distintas técnicas que permiten realizar análisis de sentimientos y obtener resultados en base a estos, pero comúnmente estos algoritmos comparten un problema que es el contexto del cual se obtienen los mensajes, debiendo tener un sistema específico para cada caso. El objetivo de esta investigación es buscar un método para poder realizar esta operación sin la problemática mencionada  anteriormente, para llevar a cabo esto se utilizó tecnologías como Deep learning,  Word Embeddings.

# 1-Dataset
## 1.1-Reviews Amazon  (amazon_vfl_reviews_test.csv)
  El dataset posee comentarios en inglés sobre variados productos de la plataforma de Amazon. Profundizando, los comentarios están clasificados en 3 polaridades, negativos, neutros y positivos en donde estas polaridades están estructuradas de la siguiente manera, 0 negativo, 1 neutro, 2 positivo. Por otra parte, el dataset posee 1098 registros en el idioma inglés, de los cuales 284 son negativos, 74 son neutros y 740 son positivos, además de poseer un diccionario de 4.734 palabras.

## 1.2-Tweets Variados Temas (twitter_sentiment_test.csv)
  La base de datos posee tweets en inglés sobre variados temas. Entrando en detalle, los comentarios están clasificados en 3 polaridades, negativos, neutros y positivos en donde estas polaridades están estructuradas de la siguiente manera, 0 negativo, 1 neutro, 2 positivo. Por otra parte, el dataset posee 1304 registros en el idioma inglés, de los cuales 256 son negativos, 589 son neutros y 459 son positivos, además de poseer un diccionario de 5.182 palabras.

## 1.3-Recopilación (Train.csv)
  Pose información sobre, noticias financieras, comentarios de diferentes videojuegos obtenidos de la plataforma de Steam, observaciones sobre aplicaciones móviles de la Play Store, tweets sobre diferentes aerolíneas de USA, tweets sobre el video juego Valorant y finalmente sobre tweets de variados temas.
Los diferentes mensajes están clasificados en 3 polaridades, negativos, neutros y positivos en donde estas polaridades están estructuradas de la siguiente manera, 0 negativo, 1 neutro, 2 positivo. Por otra parte, el dataset posee 41.512 registros en el idioma inglés, de los cuales 14.476 son negativos, 9.096 son neutros y 17.940 son positivos, además de poseer un diccionario de 64.274 palabras.

## 1.4-Representación de polaridas
  La siguiente tabla muestra como se trabajan las polaridades con su respectivo vector binario.
  
|Clase | Polaridad | Vector Binario|
| -- | -- | -- |
| 0 | Negativo |1,0,0|
| 1 | Positivo |0,1,0|
| 2 | Negativo |0,0,1|


# Word Embeddings
## Conceptnet Numberbatch
  El word embedding utilizado correspen al del proyecto de Concepnet el cual puede ser descargado de la documentación oficial:
  * https://github.com/commonsense/conceptnet-numberbatch
