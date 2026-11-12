# Clase 06 — Conoce tu ciudad: Tránsito, sonidos e inteligencia artificial

**Una experiencia en Acústica Computacional con Python — ACUS220**

> ¿Cómo podemos conocer y cuidar el ambiente sonoro de nuestras escuelas?

## ¿Por qué educar sobre el ruido?

En marzo de 2026, UNICEF publicó el informe
[*Noise and Children's Health*](https://www.unicef.org/reports/noise-and-childrens-health).

El informe destaca que el ruido es un riesgo ambiental prevenible
que puede afectar el sueño, el aprendizaje y el bienestar emocional
de niñas y niños. También menciona la reducción del tránsito
cercano a las escuelas entre las estrategias para disminuir
la exposición al ruido.

**¿Qué significa esto para nuestras propias escuelas?**

¿Cómo podemos conocer el ambiente sonoro que experimentan
sus estudiantes? ¿Qué podemos aprender al observar y
escuchar nuestra ciudad?

**Conoce tu ciudad nace de estas preguntas.**

Queremos que niñas, niños y jóvenes aprendan a escuchar
su entorno, comprenderlo e investigarlo utilizando
herramientas de acústica, ciencia de datos e inteligencia
artificial.

No buscamos solamente medir sonidos. Queremos desarrollar
curiosidad, pensamiento científico y participación en
el cuidado del ambiente sonoro.

### Del sonido al ruido

El sonido es parte de nuestra vida cotidiana. Nos permite
comunicarnos, reconocer lugares y comprender lo que sucede
a nuestro alrededor.

Pero un sonido también puede ser no deseado, interferir
con actividades importantes como aprender y descansar, o resultar perjudicial.

**No existe un único nivel sonoro a partir del cual
todo sonido se convierte automáticamente en ruido.**
El contexto también importa.

### ¿Qué papel tiene el tránsito cerca de una escuela?


Cada día circulan automóviles, motocicletas, buses y camiones por
las calles de nuestra ciudad. Todos generan sonidos, aunque no
necesariamente suenan igual.

Parte de esos sonidos llega a patios y salas de clases, donde se
mezcla con voces, viento, aves y otras fuentes del entorno.

Cuando esos sonidos resultan no deseados, interfieren con una actividad o pueden ser perjudiciales para la salud de las personas, hablamos de **ruido**. La distinción no depende solamente de la intensidad: también importan el contexto, la duración y las personas que escuchan.

**Nuestra pregunta central es: ¿cómo contribuye el tránsito al
ruido que experimentamos alrededor de nuestra escuela?**

### ¿De dónde proviene el sonido de los vehículos?

Entre sus mecanismos de generación encontramos el motor y la
propulsión, la interacción de los neumáticos con el pavimento,
las turbulencias aerodinámicas y eventos como aceleraciones
o bocinas.

Lo que finalmente escuchamos también depende de la distancia que nos separa de los vehículos,
la velocidad con la que se desplazan estos vehículos, las características de la calle y la propagación
del sonido en el entorno urbano.

| Factor | Pregunta para investigar |
| --- | --- |
| Cantidad de vehículos | ¿Qué sucede cuando circulan más vehículos? |
| Tipo de vehículo | ¿Suena igual un automóvil que un bus? |
| Velocidad | ¿Cómo cambia el sonido al cambiar la velocidad? |
| Distancia | ¿Qué ocurre cuando un vehículo se acerca? |
| Entorno | ¿Qué influencia tienen edificios y otras superficies? |
| Horario | ¿Cambia el ambiente sonoro durante el día? |

**Contar vehículos nos permite caracterizar el tránsito, pero no
equivale a medir el ruido ambiental.**

### ¿Cómo caracterizamos el ruido?

Una magnitud acústica utilizada para describir el ambiente sonoro
es el nivel sonoro continuo equivalente ponderado A,
{math}`L_{\mathrm{Aeq},T}`, correspondiente a un intervalo de tiempo
{math}`T`.

Imagina que observamos el tránsito frente a una escuela durante cinco minutos y contamos diez vehículos.

En una ocasión pasan principalmente automóviles; en otra, circulan varios buses y camiones.

Aunque el número de vehículos sea el mismo, **el nivel sonoro que registramos en un mismo punto de observación puede ser diferente**, porque también influyen el tipo de vehículo, su velocidad, la distancia a la que circula y los demás sonidos presentes en el entorno.

Nuestros registros audiovisuales permiten explorar sonidos y
comparar patrones, pero **no constituyen mediciones calibradas
de ruido ambiental**.

## Descubrimos nuestra ciudad

Comenzamos con
[Valdivia en OpenStreetMap](https://www.openstreetmap.org/#map=12/-39.82/-73.24).

OpenStreetMap es un mapa colaborativo que permite explorar calles,
avenidas, plazas, ríos y otros elementos del territorio.

**Actividad:** Busca un lugar conocido e imagina qué sonidos
podrías escuchar allí.

¿Escucharíamos lo mismo cerca de una avenida que en un parque?

La vista del mapa es general. No asignamos coordenadas precisas
a las cámaras de nuestras grabaciones sin verificarlas.

## Miramos y escuchamos el tránsito

### ¿Dónde aparece la inteligencia artificial?

Además de observar y escuchar por nosotros mismos, utilizaremos herramientas de **inteligencia artificial (IA)**. Con este nombre nos referimos a un conjunto de métodos computacionales que permiten realizar tareas como reconocer patrones, clasificar información o generar predicciones.

En esta experiencia nos interesan especialmente los **modelos de aprendizaje automático (*machine learning*)**, que aprenden patrones a partir de ejemplos durante su entrenamiento y posteriormente utilizan lo aprendido para analizar datos nuevos. Por ejemplo, YOLO es un modelo entrenado para identificar y localizar objetos en imágenes, entre ellos distintos tipos de vehículos.

Pero **YOLO no cuenta vehículos por sí solo**. Combinamos sus
detecciones con **ByteTrack**, un algoritmo de seguimiento, y con
una regla geométrica que registra cuándo las trayectorias cruzan
una línea virtual.

Los resultados son **estimaciones automáticas que debemos contrastar
con nuestras propias observaciones**.


### Primero observa y escucha

Reproduce este fragmento nocturno de Avenida Alemania.
Presta atención a los vehículos que circulan y a los sonidos
que producen.

**Demostración en clase:** observaremos y escucharemos el registro nocturno de tránsito en Avenida Alemania.
*El video con sonido se presentará durante la clase.*

**Pregunta:** ¿Cuántos vehículos crees que pasan durante
estos 30 segundos?

### Ahora escucha sin mirar

Reproduce solamente la pista sonora:

*La pista de audio se reproducirá durante la clase.*

¿Reconoces los mismos eventos que observaste en el video?

¿Podrías contar los vehículos utilizando solamente el sonido?

El enlace abre el reproductor de audio del navegador. No
interpretamos el archivo WAV como una figura.

## Exploramos el sonido

### Forma de onda y espectrograma

La forma de onda muestra cómo cambia la amplitud de la señal del audio que grabamos.
El espectrograma permite observar su contenido frecuencial
a lo largo del tiempo.

**Visualización en clase:** compararemos la forma de onda y el espectrograma del registro de tránsito.
**Para explorar:** vuelve a escuchar el audio. ¿Qué sucede
alrededor de los segundos 11 y 27? ¿Qué cambios encuentras
en el espectrograma?

### Energía y potencia espectral

Podemos estudiar características acústicas como la energía
de corta duración (STE) y la potencia en altas frecuencias (HFP).

**Visualización en clase:** examinaremos las características acústicas STE y HFP.
### ¿Qué ocurre cuando agrupamos la actividad?

**Visualización en clase:** estudiaremos los episodios acústicos y su comparación exploratoria con el video.
En nuestros experimentos encontramos tres máximos HFP
con el umbral exploratorio de prominencia 0,05, agrupados
en dos episodios de actividad.

**Dos episodios acústicos no significan necesariamente
dos vehículos.**

## Contamos vehículos con inteligencia artificial

### ¿Qué hacen YOLO y ByteTrack?

YOLO11n detecta vehículos en los fotogramas. ByteTrack
intenta mantener sus identificadores a lo largo del tiempo.

Posteriormente, un algoritmo identifica cuándo sus
trayectorias cruzan líneas definidas sobre la calle.

**Demostración en clase:** observaremos las detecciones y el seguimiento automático de vehículos.
En este experimento nocturno registramos dos eventos de
cruce. Eso no constituye por sí solo un conteo manual validado.

### ¿La inteligencia artificial también se equivoca?

¡Sí! En nuestras pruebas encontramos ejemplos concretos:

- Una motocicleta fue identificada como `car`.
- En otro video, una camioneta roja produjo probablemente
  dos registros de cruce sobre un mismo vehículo.
- La ubicación de las líneas y las pérdidas de seguimiento
  pueden producir omisiones y otras discrepancias.

Por eso debemos distinguir entre **detectar, clasificar,
seguir y contar**.

En otro experimento diurno registramos automáticamente
25 cruces en la calzada cercana y ocho en la opuesta.
Estos valores también requieren validación manual.

**Pregunta:** ¿qué deberíamos hacer antes de confiar en
los resultados de un modelo de inteligencia artificial?

## ¿Podemos contar vehículos escuchándolos?

El trabajo de Slobodan Djukanović, Jiří Matas y Tuomas
Virtanen, 2020, [*Robust Audio-Based Vehicle Counting in Low-to-Moderate Traffic Flow*](https://arxiv.org/abs/2010.11716)

**[Leer el artículo completo en PDF](https://cmp.felk.cvut.cz/data/audio_vc/paper.pdf)**, investiga el conteo
vehicular a partir de audio.

Su propuesta utiliza una función de distancia temporal
asociada a los instantes de paso de vehículos (CVMD)
y un modelo de regresión SVR.

Los mínimos locales de la función estimada permiten
proponer instantes de paso.

Nuestro análisis STE–HFP es una introducción exploratoria:
**no reproduce todavía el procedimiento CVMD–SVR
del artículo**.

Esto nos permite plantear otra pregunta:

**¿Qué información del tránsito podemos recuperar
escuchando la ciudad sin observar las imágenes?**

## Nuestro desafío escolar

### Volvamos a nuestra pregunta inicial

Al comenzar esta clase conocimos una preocupación que UNICEF ha
destacado: la importancia de proteger a niñas y niños frente a la
exposición excesiva al ruido, porque el ambiente sonoro puede
influir en las condiciones en que descansan, se comunican y aprenden.

Pero ¿qué relación tiene esa preocupación con todo lo que hemos
hecho en esta experiencia?

Observamos calles de nuestra ciudad, escuchamos el tránsito,
exploramos grabaciones mediante espectrogramas y utilizamos
modelos de aprendizaje automático para identificar vehículos.
También descubrimos que estos modelos pueden equivocarse y que
**contar vehículos no equivale a medir el ruido ambiental**.

Todavía no sabemos cuál es la exposición al ruido de una escuela
determinada. Para responder esa pregunta necesitamos observaciones
y mediciones apropiadas.

Sin embargo, hemos aprendido algo esencial: **cómo comenzar a
transformar una preocupación de nuestra vida cotidiana en preguntas
que podemos investigar científicamente**.

### Del aprendizaje a nuestra comunidad escolar

Imaginemos ahora que una comunidad escolar quiere conocer mejor
su ambiente sonoro.

Podríamos comenzar escuchando qué ocurre en sus patios y salas
de clases, reconociendo los sonidos que caracterizan esos espacios
y preguntándonos cuáles pueden interferir con actividades como
conversar, escuchar una explicación o descansar.

Después podríamos estudiar las fuentes de sonido, observar el
tránsito cercano, comparar distintos horarios y realizar
mediciones acústicas cuando contemos con los instrumentos adecuados.

Los datos, las grabaciones y los modelos computacionales nos
ayudarían a investigar. Pero comprender los resultados también
requeriría escuchar a las personas que utilizan esos espacios.

**No se trata de eliminar todos los sonidos ni de buscar una
escuela completamente silenciosa. Se trata de comprender su
ambiente sonoro y contribuir a que sea adecuado para aprender,
convivir y desarrollarse.**

### ¿Qué nos llevamos de esta experiencia?

Para quienes estudiamos acústica computacional, esta clase
muestra que las herramientas tecnológicas adquieren sentido
cuando se utilizan para investigar problemas reales, con
rigor y responsabilidad.

Para las comunidades escolares, abre una posibilidad igualmente
importante: que niñas, niños y jóvenes participen en el
conocimiento de su propio entorno, formulen preguntas,
interpreten evidencias y compartan sus descubrimientos.

Así regresamos al punto de partida de nuestra clase:
el bienestar de las personas y la importancia de la educación.

**Aprender a escuchar nuestra ciudad es también aprender
a comprenderla y cuidarla.**

---
*Actividad exploratoria de ACUS220. Los materiales
audiovisuales se utilizan en la demostración local
mientras se verifican sus permisos de difusión pública.*
