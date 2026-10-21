# Hito 2 — Pauta de presentación y evaluación

## Propósito

El **Hito 2** corresponde a la segunda presentación evaluada del proyecto del semestre.

A diferencia del Hito 1, esta presentación **no comienza desde cero**.

El Hito 1 permitió construir una primera fotografía organizada del proyecto:

```text
problema
   ↓
pregunta provisional
   ↓
datos
   ↓
organización del repositorio
   ↓
primeras evidencias
   ↓
pipeline inicial
   ↓
próximos pasos
```

El **Hito 2 comienza donde terminó el Hito 1**.

Su propósito es mostrar cómo evolucionó el proyecto durante aproximadamente un mes de trabajo y qué aprendimos al comenzar a desarrollar, probar, analizar y tomar decisiones.

La progresión de los tres hitos puede pensarse así:

```text
Hito 1 — fines de septiembre
¿qué queremos hacer y cómo pensamos comenzar?

        ↓

Hito 2 — fines de octubre
¿qué hicimos desde entonces,
qué evidencia obtuvimos,
qué aprendimos
y qué decisiones tomamos?

        ↓

Hito 3 — fines de noviembre
¿hasta dónde llegamos,
qué resultados obtuvimos,
qué limitaciones quedaron
y qué aprendimos del proyecto?
```

La presentación del Hito 2 debería permitir contar una historia como esta:

```text
en el Hito 1 estábamos aquí
          ↓
durante este mes hicimos...
          ↓
observamos / obtuvimos...
          ↓
encontramos estas dificultades...
          ↓
tomamos estas decisiones...
          ↓
modificamos / mantuvimos...
          ↓
ahora el proyecto está aquí
          ↓
para el Hito 3 haremos...
```

> **El Hito 2 evaluará principalmente la evolución del proyecto desde el Hito 1, la evidencia concreta del trabajo realizado, la capacidad para interpretar lo encontrado y la justificación de las decisiones tomadas.**

No todos los proyectos deberán encontrarse en la misma etapa.

Un proyecto puede haber avanzado hacia modelos o experimentos, mientras otro puede haber descubierto problemas importantes en sus datos, reformulado su pregunta, cambiado una representación o reducido razonablemente su alcance.

> **Avanzar no significa solamente agregar más código o utilizar métodos más complejos. También significa comprender mejor el problema, detectar limitaciones y tomar mejores decisiones.**

---

## 1. Formato de la presentación

Cada proyecto dispondrá de:

```text
10 minutos de presentación
+
5 minutos de preguntas
```

La presentación debe ser clara, profesional y ajustarse al tiempo disponible.

Como referencia, una presentación de aproximadamente **7 a 9 diapositivas** debería ser suficiente.

### Importante

La presentación **no debe repetir extensamente el Hito 1**.

El problema, la pregunta y los datos pueden recordarse brevemente para entregar contexto, pero idealmente esa recapitulación debería ocupar **como máximo una diapositiva**.

El tiempo principal debe utilizarse para mostrar:

- qué trabajo se realizó desde el Hito 1;
- qué evidencia se obtuvo;
- qué dificultades aparecieron;
- qué decisiones se tomaron;
- cómo cambió o se consolidó el proyecto;
- y qué se realizará antes del Hito 3.

---

## 2. Requisito fundamental — Repositorio GitHub

Cada proyecto debe continuar trabajando sobre el **mismo repositorio GitHub** presentado en el Hito 1.

El repositorio puede ser público o privado, pero debe continuar compartido con:

- **Víctor Poblete**, profesor del curso;
- **Carlos Duarte**, ayudante del curso.

Este requisito sigue siendo fundamental porque el repositorio es uno de los principales medios para **acompañar, revisar y retroalimentar la evolución del proyecto durante el semestre**.

> **En el Hito 2 no esperamos un repositorio nuevo. Esperamos observar cómo evolucionó el repositorio que ya existía en el Hito 1.**

---

## 3. Evolución esperada del repositorio

Al momento del Hito 2 debería ser posible reconocer que el repositorio **ha evolucionado desde septiembre**.

Según el proyecto, esta evolución puede reflejarse en:

- nuevos commits;
- actualización del `README.md`;
- notebooks adicionales o revisados;
- scripts o funciones;
- nuevas figuras;
- resultados intermedios;
- documentación de decisiones;
- mejoras en la estructura;
- registro de dependencias;
- instrucciones para reproducir análisis;
- separación clara entre datos originales y derivados.

No se espera que todos los repositorios tengan la misma estructura.

Sí se espera que permitan reconstruir razonablemente:

```text
qué se hizo
   ↓
cómo se hizo
   ↓
con qué datos
   ↓
qué resultado produjo
```

La organización computacional sigue formando parte del proyecto.

### Una fotografía de la trazabilidad de los proyectos

Antes del Hito 2 realizamos una revisión general de los **12 repositorios informados para los proyectos del curso**. El objetivo de esta revisión **no es comparar cuánto ha trabajado cada equipo ni establecer un ranking entre proyectos**, sino observar hasta qué punto GitHub está permitiendo reconstruir el proceso desarrollado entre ambos hitos.

La siguiente tabla corresponde a una **fotografía formativa de la actividad visible en GitHub al 21 de octubre de 2026**. Las observaciones se refieren exclusivamente a la trazabilidad que puede observarse en el repositorio y no al trabajo que eventualmente pueda existir fuera de GitHub.

| Proyecto | Actividad visible entre Hito 1 y Hito 2 | Observación sobre trazabilidad |
| --- | --- | --- |
| **Narración emocional — Generación de audiolibros con análisis de sentimientos** | Se observa una secuencia importante de organización, documentación, dependencias, estructura y resultados alrededor del cierre del Hito 1, seguida por una actualización del `README.md` el 8 de octubre. | Existe una base de trabajo bien organizada, pero la evolución posterior al Hito 1 aparece poco distribuida en el historial visible. Conviene registrar progresivamente el desarrollo de las siguientes fases. |
| **AstroWave** | Se observa actividad reciente el 21 de octubre con generación de audio y modificación del dataset para incorporar nuevos datos astronómicos. | Existe avance reciente y sustantivo. Sería útil continuar registrando las etapas intermedias para que el historial permita reconstruir mejor el proceso. |
| **Proyecto asociado a `Acus220Repo-Tesis` — título no verificable** | Al momento de esta revisión no fue posible acceder al repositorio desde el enlace informado. | **No es posible evaluar su trazabilidad visible.** Antes del Hito 2 debe verificarse que el enlace sea correcto y que profesor y ayudante tengan acceso al repositorio. |
| **Diarización de hablantes** | Al momento de esta revisión no se observan commits posteriores al 29 de septiembre. | El repositorio no refleja todavía qué ocurrió durante octubre. Esto no implica necesariamente ausencia de trabajo, pero sí **falta de trazabilidad visible** entre ambos hitos. |
| **Visuales controladas vía señales de audio** | La actividad visible se concentra entre el 29 de septiembre y el 1 de octubre, incluyendo notebook, datos, correcciones y preparación del Hito 1. | El repositorio documenta el estado alcanzado para el Hito 1, pero no muestra todavía una evolución visible durante las semanas posteriores. |
| **Detector de Características Humanas a través de la Voz** | La actividad visible más reciente corresponde al 24 de septiembre. No se observan commits durante octubre en la revisión realizada. | Conviene que el trabajo desarrollado después del Hito 1 comience a quedar registrado en GitHub para que pueda reconstruirse la evolución del proyecto. |
| **Proyecto Acus — Transcripción y separación de audio con IA** | Se observa un commit reciente el 21 de octubre que integra HT-Demucs y un comparador DSP en Marimo; la actividad anterior se concentra principalmente en septiembre. | Existe avance técnico reciente y significativo. Conviene mantener una secuencia más continua de commits que documente pruebas, decisiones y resultados intermedios. |
| **Cancelación adaptativa de ruido con filtros LMS, NLMS y RLS** | Se observan varios commits diferenciados durante octubre relacionados con experimentos, incorporación de voz real, análisis de sensibilidad, refactorización, notebooks, resultados y documentación. | El historial permite reconstruir con bastante claridad cómo ha evolucionado el proyecto y constituye un buen ejemplo de **trazabilidad del proceso**, más que simplemente de cantidad de commits. |
| **Exploración y Clasificación Acústica de Géneros Musicales** | Se observan commits de organización, notebook exploratorio, pipeline y actualización del `README.md` durante los primeros días de octubre; la actividad visible más reciente es del 6 de octubre. | Existe evidencia de evolución respecto del Hito 1, aunque sería conveniente mantener la documentación del trabajo de manera más continua. |
| **DeMask — Smart Dynamic EQ** | La actividad visible se concentra alrededor de los días previos al Hito 1 y no se observan commits posteriores al 30 de septiembre. | Conviene que los avances desarrollados durante octubre comiencen a quedar registrados progresivamente en el repositorio. |
| **Acoustic Monitoring Indexing System with BirdNET v3** | La actividad visible más reciente corresponde al 29 de septiembre y se concentra en la organización inicial del repositorio, dependencias, `README.md` y scripts. | No se observa todavía trazabilidad visible del trabajo desarrollado durante octubre. |
| **Proyecto asociado a `panxuloo/acustica_python` — título no verificable** | Al momento de esta revisión no fue posible acceder al repositorio desde el enlace informado. | **No es posible evaluar su trazabilidad visible.** Antes del Hito 2 debe verificarse que el enlace sea correcto y que profesor y ayudante tengan acceso al repositorio. |

> **Esta tabla no evalúa la cantidad de trabajo realizado por cada equipo. Resume únicamente la actividad visible en los repositorios al momento de esta revisión y se utiliza como retroalimentación formativa sobre trazabilidad.**

El historial de Git debe ayudar a observar la evolución del proyecto entre el Hito 1 y el Hito 2.

**No existe un número mínimo de commits y la cantidad de commits no será evaluada mecánicamente.** Lo que esperamos es que el repositorio funcione como una memoria del proceso: que los cambios relevantes se registren progresivamente y con mensajes suficientemente informativos para comprender qué se hizo.

Un único commit grande realizado poco antes de la presentación puede contener trabajo técnicamente valioso, pero ofrece menos trazabilidad que un historial que permita reconocer etapas, decisiones, experimentos, correcciones o resultados intermedios.

Del mismo modo, **no tiene sentido crear commits artificiales o dividir cambios solamente para aumentar su número**. Los commits deben corresponder a unidades de trabajo reales y comprensibles.

> **GitHub no es solamente un lugar donde entregar el proyecto antes de cada hito; es parte de la memoria y trazabilidad de cómo el proyecto va evolucionando durante el semestre.**

Esta revisión constituye **retroalimentación formativa**. Todavía existe tiempo para mejorar la documentación y trazabilidad antes del Hito 2. No se espera reconstruir artificialmente actividad pasada; se espera comprender que, desde este momento y especialmente hacia el Hito 3, GitHub debe acompañar progresivamente el desarrollo del proyecto.

---

## 4. Contenido recomendado de la presentación

### 4.1 Portada

La primera diapositiva debe mantener una apariencia formal e incluir:

- título del proyecto;
- nombres de los integrantes;
- asignatura **ACUS220 — Acústica Computacional con Python**;
- Universidad Austral de Chile;
- fecha;
- escudo institucional.

### 4.2 Punto de partida — ¿Dónde terminó el Hito 1?

Al comienzo de la presentación se recomienda incluir una síntesis muy breve del estado anterior.

Por ejemplo:

```text
Hito 1
pregunta inicial
+
datos seleccionados
+
pipeline provisional
+
estado alcanzado
```

No es necesario volver a explicar en detalle toda la motivación ni reconstruir la presentación anterior.

La pregunta que orienta esta parte es:

> **¿Desde qué punto concreto comenzamos a trabajar después del Hito 1?**

Si la pregunta, los datos, el alcance o el pipeline cambiaron desde entonces, debe indicarse claramente.

### 4.3 Trabajo realizado entre el Hito 1 y el Hito 2

Esta es una de las partes centrales de la presentación.

Cada estudiante o equipo debe mostrar **evidencia concreta del trabajo realizado durante el último mes**.

Dependiendo del proyecto, esta evidencia puede incluir:

- descarga, organización o depuración de nuevos datos;
- auditoría del dataset;
- escucha o inspección sistemática de grabaciones;
- análisis exploratorio;
- visualizaciones;
- formas de onda;
- espectrogramas;
- representaciones Mel o log-Mel;
- extracción de características;
- desarrollo de notebooks;
- scripts o funciones;
- automatización de etapas;
- construcción o modificación de un pipeline;
- adquisición o anotación de datos;
- pruebas de bibliotecas;
- implementación de métodos;
- experimentos iniciales;
- entrenamiento de modelos;
- evaluación preliminar;
- comparación de alternativas;
- lectura y uso de bibliografía técnica o científica;
- documentación de problemas encontrados.

No es suficiente afirmar:

> *“trabajamos en los datos”*

o:

> *“probamos un modelo”*.

La presentación debe mostrar **qué se hizo realmente y qué evidencia quedó de ese proceso**.

### 4.4 Comprensión de los datos y desarrollo metodológico

Durante el Hito 2 esperamos una comprensión más profunda del material de trabajo.

Según el proyecto, puede ser relevante explicar:

- qué se aprendió acerca de los datos;
- qué problemas de calidad aparecieron;
- qué limitaciones tienen las etiquetas;
- si existen desbalances;
- qué preprocesamiento fue necesario;
- qué representaciones se escogieron;
- qué variables o características se utilizaron;
- qué método se implementó o se está evaluando;
- qué supuestos se están realizando;
- por qué una alternativa parece más apropiada que otra.

La metodología no necesita estar terminada.

Lo importante es mostrar que las decisiones comienzan a estar respaldadas por **observaciones, pruebas o evidencia**.

> **En el Hito 1 podíamos decir “pensamos hacer esto”. En el Hito 2 deberíamos comenzar a poder decir “hicimos esta prueba y, a partir de lo observado, decidimos esto”.**

### 4.5 Resultados o evidencias intermedias

El Hito 2 no exige resultados finales.

Sí esperamos encontrar **resultados, observaciones o evidencias intermedias** que permitan comprender qué está ocurriendo en el proyecto.

Por ejemplo:

- una distribución de datos;
- una auditoría;
- una tabla;
- una figura;
- una comparación;
- una característica acústica;
- un espectrograma;
- una representación;
- una métrica preliminar;
- una salida de un algoritmo;
- una prueba experimental;
- un ejemplo exitoso;
- un ejemplo problemático;
- un resultado inesperado;
- evidencia de que una estrategia no funcionó.

Una figura por sí sola no constituye interpretación.

Cada resultado debería ayudarnos a responder:

> **¿Qué observamos y qué significa esto para el proyecto?**

### 4.6 Decisiones tomadas

A partir de la evidencia acumulada, cada proyecto debería comenzar a justificar decisiones.

Por ejemplo:

```text
pensábamos utilizar...
       ↓
al probarlo observamos...
       ↓
esto mostró una limitación...
       ↓
por esa razón decidimos...
```

Puede haber decisiones sobre:

- datos;
- preprocesamiento;
- representaciones;
- características;
- bibliotecas;
- modelos;
- métricas;
- organización del trabajo;
- alcance;
- pregunta de investigación.

No se espera que todas las decisiones sean definitivas.

Sí se espera que puedan explicarse a partir de la evidencia disponible.

### 4.7 Pipeline actualizado

El pipeline presentado en el Hito 1 era provisional.

Para el Hito 2 debe revisarse a partir de la experiencia adquirida.

Por ejemplo:

```text
pipeline del Hito 1
        ↓
trabajo realizado
        ↓
dificultades / hallazgos
        ↓
pipeline actualizado
```

La presentación debería mostrar:

- qué etapas ya fueron realizadas;
- cuáles están actualmente en desarrollo;
- qué etapas cambiaron;
- qué etapas fueron descartadas;
- qué queda pendiente.

No existe obligación de conservar el pipeline original.

> **El pipeline debe representar el proyecto real, no el proyecto que imaginábamos hace un mes.**

---

## 5. Planificación hacia el Hito 3

El Hito 3 se realizará a fines de noviembre y corresponderá al cierre del proyecto del semestre.

Por eso, el Hito 2 debe terminar con una planificación **concreta y realista** para las semanas restantes.

Cada equipo debería poder identificar:

- qué aspecto es prioritario;
- qué análisis o experimento falta realizar;
- qué resultado necesita obtener;
- qué problema todavía debe resolver;
- qué parte del alcance inicial probablemente ya no será posible completar;
- qué sería un cierre razonable del proyecto.

Una pregunta central será:

> **¿Qué debemos hacer entre hoy y el Hito 3 para cerrar el proyecto de manera coherente?**

No es necesario intentar completar todo lo imaginado al comienzo del semestre.

Puede ser mejor cerrar bien una pregunta más acotada que dejar muchas líneas abiertas.

---

## 6. Decisiones, dificultades y reformulaciones

Durante un proyecto real es normal encontrar dificultades.

El Hito 2 debe mostrar también qué ocurrió cuando el plan inicial se enfrentó con los datos y con la implementación.

Puede ser necesario explicar:

- qué dificultad apareció;
- cómo fue detectada;
- qué alternativas se consideraron;
- qué decisión se tomó;
- qué parte del plan cambió;
- qué parte se mantuvo;
- si fue necesario reformular la pregunta;
- si se redujo o amplió el alcance;
- si una metodología fue descartada;
- si apareció una nueva pregunta.

Cambiar el plan **no constituye un problema** si existe una razón bien explicada.

> **Una reformulación justificada puede representar más aprendizaje que continuar mecánicamente con un plan que los datos ya demostraron inadecuado.**

---

## 7. Referencias

Toda fuente utilizada debe ser reconocida.

Esto incluye, cuando corresponda:

- artículos científicos;
- libros;
- datasets;
- repositorios GitHub;
- documentación de bibliotecas;
- documentación técnica;
- sitios web;
- software;
- imágenes o figuras provenientes de otras fuentes.

En este hito será especialmente importante poder identificar las fuentes que hayan influido en **decisiones metodológicas**.

---

## 8. Declaración de uso de inteligencia artificial

Cada presentación debe incluir nuevamente una **declaración explícita de uso de herramientas de inteligencia artificial**.

La declaración debe indicar:

- si se utilizaron herramientas de IA;
- cuáles se utilizaron;
- para qué fueron utilizadas;
- y, cuando corresponda, qué aspectos fueron verificados o decididos por el estudiante o equipo.

La declaración debe reflejar el **uso real realizado durante esta etapa del proyecto**.

---

## 9. Pauta de evaluación

| Criterio | Qué observaremos | Ponderación |
| --- | --- | ---: |
| **1. Continuidad y evolución desde el Hito 1** | Capacidad para ubicar brevemente el punto de partida y mostrar qué cambió, se mantuvo o se reformuló desde la presentación anterior. | **10%** |
| **2. Evidencia de trabajo realizado entre hitos** | Evidencia concreta, suficiente y trazable del trabajo desarrollado durante el último mes. | **20%** |
| **3. Comprensión de los datos y desarrollo metodológico** | Mayor comprensión de los datos, procesamiento realizado, metodología utilizada o en desarrollo y coherencia de las decisiones técnicas. | **15%** |
| **4. Resultados o evidencias intermedias e interpretación** | Calidad y pertinencia de resultados, observaciones, pruebas, figuras, experimentos o análisis intermedios, incluyendo su interpretación. | **20%** |
| **5. Decisiones, dificultades, reformulaciones y planificación hacia el Hito 3** | Capacidad para identificar problemas, justificar decisiones, reconocer limitaciones, reformular razonablemente el proyecto y proponer un cierre realista. | **10%** |
| **6. Repositorio GitHub, documentación y reproducibilidad** | Evolución trazable del repositorio **durante el período entre hitos**, commits significativos, `README.md`, organización, documentación y posibilidad de comprender o reproducir el trabajo realizado. | **10%** |
| **7. Comunicación profesional y manejo del tiempo** | Claridad oral, terminología apropiada, calidad visual, organización de la presentación y ajuste a los 10 minutos. | **10%** |
| **8. Referencias y declaración de uso de IA** | Fuentes identificadas correctamente y declaración transparente del uso de IA durante esta etapa. | **5%** |
|  | **Total** | **100%** |

---

## 10. ¿Qué se valorará especialmente?

En este hito se valorará especialmente la capacidad para demostrar:

- **progreso real desde el Hito 1**;
- evidencia concreta del trabajo realizado;
- comprensión creciente de los datos;
- capacidad para transformar observaciones en decisiones;
- documentación del proceso;
- interpretación de resultados intermedios;
- reconocimiento de dificultades;
- reformulación cuando esté justificada;
- planificación realista hacia el cierre del semestre.

No se premiará automáticamente:

- presentar más algoritmos;
- utilizar modelos más complejos;
- mostrar muchas figuras sin interpretarlas;
- escribir más líneas de código;
- mantener intacta la idea original;
- o encontrarse en una etapa aparentemente más avanzada que otro equipo.

> **El Hito 2 no evalúa quién llegó más lejos. Evalúa cómo evolucionó cada proyecto desde su propio Hito 1.**

---

## 11. Preguntas posteriores a la presentación

Después de los 10 minutos de presentación tendremos aproximadamente **5 minutos de preguntas**.

Las preguntas pueden abordar aspectos como:

- ¿qué cambió desde el Hito 1?;
- ¿cuál fue el avance más importante del último mes?;
- ¿qué evidencia respalda esa decisión?;
- ¿qué aprendieron acerca de los datos?;
- ¿qué resultado les sorprendió?;
- ¿qué estrategia no funcionó y por qué?;
- ¿qué parte del pipeline modificaron?;
- ¿qué limitación consideran actualmente más importante?;
- ¿qué pueden concluir y qué todavía no pueden concluir?;
- ¿qué dejarían fuera si tuvieran que reducir el alcance?;
- ¿cuál es el próximo experimento, análisis o commit?;
- ¿qué necesitan completar antes del Hito 3?

El propósito de estas preguntas no es buscar una respuesta perfecta.

Buscamos comprobar que el equipo **comprende lo que ha realizado, puede interpretar su propia evidencia y puede justificar cómo continuará**.

---

## 12. Para llevarse de este hito

El Hito 2 representa una segunda fotografía del proyecto, pero ahora basada en experiencia y evidencia acumulada.

Queremos poder contar:

```text
en septiembre propusimos...
        ↓
durante octubre hicimos...
        ↓
los datos mostraron...
        ↓
aprendimos...
        ↓
por eso decidimos...
        ↓
ahora sabemos mejor qué podemos hacer
        ↓
y tenemos un plan realista para noviembre
```

> **El valor del Hito 2 está en mostrar evolución: pasar de una intención inicial a un proyecto que ya ha producido evidencia, decisiones y aprendizaje.**
