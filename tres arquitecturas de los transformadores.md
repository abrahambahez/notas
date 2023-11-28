Los [[transformadores (redes neuronales)]] tienen dos componentes: el codificador (*encoder*) cuyo trabajo es comprender la entrada, y el decodificador (*decoder*) cuyo trabajo es procesar la generación de texto (salida).

Pero a partir de estos dos componentes existen tres combinaciones posibles que han mostrado tener ventajas y desventajas para ciertas tareas, tales como escribir prosa, resumir, traducir, traer información y conectarse a API. Así:

- Un modelo tipo *Encoder only* (*Autoencoding, Masked Language Modeling*) como Bert y Roberta, enmascara aleatoriamente *tokens* para ser reconstruidos con un contexto bidireccional
    - Es bueno para inferencia de sentimiento, reconocimiento de entidades y clasificación de palabras
- Un modelo tipo *Decoder Only* (*Autoregresive, Causal Languaje Modeling*) como GPT o BloomGPT predice el nuevo *token* basado en el anterior con un contexto unidireccional
    - Es bueno para generar texto y dependiendo de su tamaño, puede presentar [[comportamientos emergentes]]
- Un modelo tipo *Encoder Decoder* (*Sequence to sequence o Seq2Seq*) como T5 o Bart, enmascara *token* de *tokens* llamados *spans* y reconstruye el *span*
    - Es bueno para traducción, resúmenes y chatbots

#memo 
¿Cuáles son las 3 arquitecturas de una red transformadora según sus dos componentes principales? :: encoder-only, decoder-only, encoder-decoder
<!--SR:!2023-12-01,9,230-->

Al modelo *encoder-only* se le llama ==autoencoding==
<!--SR:!2023-12-11,18,210-->

Al modelo *decoder-only* se le llama ==autoregresive==
<!--SR:!2023-12-01,9,170-->

Al modelo *encoder-decoder* se le llama ==sequence to sequence==
<!--SR:!2023-12-01,17,230-->
