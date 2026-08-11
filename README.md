# CONTEXTO DEL PROYECTO
El presente proyecto se enfoca en realizar la transcripción automática de baterias mediante el uso de señales vibratorias provenientes de las membranas de los cuerpos de la bateria y capturadas con sensores del tipo piezoelectrico llamados "triggers", y elementos de Machine Learning, de esta manera el sistema podra transcribir golpes con distintas dinamicas. Para lograr esto se grabaron grandes numeros de muestras de golpes individuales de los cuerpos de la bateria, estos cuerpos son el BOMBO (KD), la caja (SD) y los toms de 12, 14 y 16 pulgadas (T12, T14, T16), se grabaron muestras en frecuencias de muestreo de 8KHZ y 12KHZ y con dinamicas de golpes fuertes, medios y suaves o ghost notes. El modelo a emplearse para este proyecto es el usado en los papers:
- M. Zehren, M. Alunno, and P. Bientinesi, “ADTOF: A large dataset of non-synthetic music for automatic drum transcription,” in Proceedings of the 22st International Society for Music Information Retrieval Conference, Online, 2021, pp. 818–824.
- Zehren, M.; Alunno, M.; Bientinesi, P. High-Quality and Reproducible Automatic Drum Transcription from Crowdsourced Data. Signals 2023, 4, 768-787. https://doi.org/10.3390/signals4040042

Este modelo utiliza muestras o frases de bateria, aqui definimos una frase como un fragmento corto de golpes sucesivos de bateria, donde se utilizan distintos elementos de la bateria, en pocas palabras, pueden definirse como pequeñas improvisaciones o fills que usan distintos cuerpos de la bateria, a distintos tempos y dinamicas.
# OBJETIVO
Debido a esta particularidad del modelo, el objetivo especifico de este repo es el de realizar la generacion procedural de estas frases de bateria para el entrenamiento del modelo.
# DATASET
Los datos grabados o golpes individuales estan almacenados en la carpeta "MUESTRAS" y estan divididos en las siguientes clases: KD (kick drum), SD (snare drum), T12 (tom de 12 pulgadas), T14 (tom de 14 pulgadas) y T16 (tom de 16 pulgadas), debemos considerar que estos datos fueron grabados con frecuencias de muestreo de 8KHZ y 12KHZ.
# PIPELINE
La forma en la que se va a trabajar consiste en:

## GENERACION DE FRASES DE BATERIA
Se debe utilzar el gran numero de datos de los golpes individuales de los elementos mencionados de la bateria para crear frases de bateria.
## EXPORTACION DE WAV y LABELS
Cada una de estas frases de bateria se va a exportar en formato WAV y con sus labels correspondientes.
## ENTRENAMIENTO DEL MODELO ADTOF
Estas frases exportadas en WAV junto con sus labels seran alimentadas al modelo de ADTOF para realizar la transcripción.

# CURRENT OBJECTIVE:
Implementar un generador proceradural de frases de bateria que evite los siguientes problemas:
- Anteriores intentos por realizar el generador de frases resultaron en que las frases creadas se crearan exitosamente pero el resultado tenia demasiada distorsion.
- Estos intentos tambien mostraban que los golpes estaban completamente desordenados y sin sentido musical.
- Tambien se observo que varios de los golpes que se podia distinguir se solapaban uno encima del otro, lo que contribuia a que los audios resultantes y sus respectivas formas de ondas se vieran mas distorsionadas e inentendibles.
Ademas, todos los audios generados deben ser mono, ser exportados en WAV y normalizar una frecuencia de muestreo ideal.
# AVANCES ACTUALES:
-  Ahora se logro crear un generador de frases que genere una frase de prueba.
- Esta frase es un ritmo simple de KD+SD+KD+SD
- La frase creada no contiene distorsion, clipping casi inexistente y la forma de onda es consistente con los golpes que separados del dataset de golpes separados.
- Se consiguió crear las 100 frases, pero ahora es mas notable un truncamiento de los golpes, especialmente al introducir las frases creadas en el software Audacity, se nota que gran parte del decaimiento de la onda es cortado y esto se nota al escucharlo, eso si, la distorsion sigue siendo inexistente y las frases suenan casi naturales.
- Luego de los avances del anterior punto se pudo conseguir que el truncamiento de los golpes sea menor, casi hasta eliminado, ahora el decaimiento de la onda ya no se corta ni se oye cortado.
- Ahora la musicalidad de las frases generadas se siente mas natural y tiene mas coherencia con lo que un baterista tocaria.