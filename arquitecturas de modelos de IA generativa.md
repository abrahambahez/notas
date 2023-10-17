Un  [[modelo de IA generativa]] centrado en texto, especialmente un [[LLM]] puede ser bueno para distintas tareas dependiendo de su arquitectura.

Tareas como escribir prosa, resumir, traducir, traer información y conectarse a APIs. Así:

- Un modelo tipo *Encoder only* (*Autoencoding, Masked Language Modeling*) como Bert y Roberta, enmascara aleatoriamente *tokens* para ser reconstruidos con un contexto bidireccional
    - Es bueno para inferencia de sentimiento, reconocimiento de entidades y clasificación de palabras
- Un modelo tipo *Decoder Only* (*Autoregresive, Causal Languaje Modeling*) como GPT o BloomGPT predice el nuevo *token* basado en el anterior con un contexto unidireccional
    - Es bueno para generar texto y dependiendo de su tamaño, puede presentar [[propiedades emergentes]]
- Un modelo tipo *Encoder Decoder* (*Sequence to sequence o Seq2Seq*) como T5 o Bart, enmascara *token* de *tokens* llamados *spans* y reconstruye el *span*
    - Es bueno para traducción, resumenes y chatbots

#memo 
¿Cuáles son las 3 arquitecturas de modelos generativos de AI? :: encoder-only, decoder-only, encoder-decoder
<!--SR:!2023-10-19,3,250-->

Al modelo *encoder-only* se le llama ==autoencoding==
<!--SR:!2023-10-17,1,230-->

Al modelo *decoder-only* se le llama ==autoregresive==
<!--SR:!2023-10-17,1,230-->

Al modelo *encoder-decoder* se le llama ==sequence to sequence==
<!--SR:!2023-10-19,3,250-->
