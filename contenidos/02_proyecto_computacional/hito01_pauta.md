# Hito 1 — Pauta de presentación y evaluación

## Propósito

El **Hito 1** corresponde a la primera presentación evaluada del proyecto del semestre.

Su propósito no es mostrar un proyecto terminado, sino evidenciar que la idea inicial ya comenzó a transformarse en un **proyecto computacional organizado, comprensible, documentado y desarrollable**.

En esta etapa esperamos que cada estudiante o equipo pueda explicar profesionalmente:

```text
qué problema queremos abordar
        ↓
qué queremos investigar o explorar
        ↓
con qué datos trabajaremos
        ↓
cómo estamos organizando el proyecto
        ↓
qué hemos realizado hasta ahora
        ↓
cómo pensamos continuar
```

No es necesario haber entrenado modelos, completado análisis ni obtenido resultados definitivos.

> **En este hito se evaluará la calidad con que el proyecto ha comenzado a formularse, organizarse, documentarse y desarrollarse desde su propio punto de partida.**

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

---

## 2. Requisito fundamental — Repositorio GitHub

Cada proyecto debe contar con un **repositorio en GitHub**.

El repositorio puede ser público o privado, pero debe estar compartido con:

- **Víctor Poblete**, profesor del curso;
- **Carlos Duarte**, ayudante del curso.

Este requisito es fundamental porque el repositorio será uno de los principales medios para **acompañar, revisar y retroalimentar el desarrollo del proyecto durante el semestre**.

> **El repositorio GitHub compartido con el profesor y el ayudante es un requisito obligatorio del Hito 1.**

Si el repositorio es privado, ambos deben haber sido incorporados como colaboradores antes de la presentación.

---

## 3. Organización esperada del repositorio

No todos los proyectos necesitarán exactamente la misma estructura.

Sin embargo, al momento del Hito 1 debería ser posible reconocer una organización comprensible.

Por ejemplo:

```text
mi_proyecto/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
├── figures/
├── results/
└── references/
```

Es posible que algunas de estas carpetas todavía no sean necesarias.

Lo importante es que la estructura tenga sentido para el proyecto y permita comprender:

- dónde se encuentran los datos;
- dónde se desarrollan los análisis;
- dónde se guardan scripts o funciones;
- dónde se almacenan figuras o resultados;
- y cómo se documenta el trabajo realizado.

El repositorio debería mostrar señales de evolución mediante commits y documentación progresiva.

---

## 4. Contenido recomendado de la presentación

##4.1 Portada

La primera diapositiva debe tener una apariencia formal e incluir:

- título provisional del proyecto;
- nombres de los integrantes;
- asignatura **ACUS220 — Acústica Computacional con Python**;
- Universidad Austral de Chile;
- fecha;
- escudo institucional.

##4.2 Problema y motivación

Explicar con lenguaje técnico, profesional y comprensible:

- ¿qué fenómeno queremos estudiar?;
- ¿en qué contexto aparece?;
- ¿por qué es interesante?;
- ¿por qué tiene sentido abordarlo computacionalmente?

La presentación debería avanzar desde una idea general hacia una formulación más precisa.

Por ejemplo:

```text
“queremos trabajar con música”
```

debería evolucionar hacia algo como:

```text
“nos interesa estudiar...”
```

y luego explicar específicamente qué aspecto será investigado.

##4.3 Pregunta, objetivo o exploración principal

Explicar con claridad:

> **¿Qué queremos investigar, caracterizar, comparar, detectar, modelar o explorar?**

La pregunta puede ser todavía provisional.

Es completamente válido que cambie durante el semestre como consecuencia de lo que aprendamos de los datos, de las herramientas o del propio problema.

##4.4 Datos

Presentar qué datos utilizarán o están considerando utilizar.

Según el proyecto, puede ser relevante informar:

- fuente de los datos;
- cantidad aproximada;
- formato de los archivos;
- variables disponibles;
- etiquetas;
- duración de las señales;
- frecuencia de muestreo;
- metadatos;
- forma en que están organizados;
- restricciones;
- limitaciones conocidas;
- incertidumbres que todavía deben resolver.

Si aún están buscando datos, deberán explicar:

- qué necesitan encontrar;
- qué alternativas han identificado;
- y qué criterios utilizarán para escoger entre ellas.

> **Primero conocemos los datos. Después elegimos las herramientas.**

##4.5 Organización computacional del proyecto

Mostrar brevemente el repositorio GitHub.

La presentación debería permitir reconocer:

- estructura de carpetas;
- `README.md`;
- datos o estrategia de organización de datos;
- notebooks;
- scripts, si existen;
- figuras o resultados iniciales;
- documentación;
- historial de commits.

No se espera una estructura perfecta ni definitiva.

Se espera que el proyecto ya muestre un **criterio de organización**.

##4.6 Estado actual y primeras evidencias

Mostrar qué se ha realizado realmente hasta el momento.

La evidencia puede ser muy diferente entre proyectos.

Por ejemplo:

- búsqueda y selección de un dataset;
- revisión de repositorios;
- escucha o inspección de audios;
- auditoría de archivos;
- organización de datos;
- lectura de metadatos;
- primeras formas de onda;
- espectrogramas;
- visualizaciones;
- notebooks iniciales;
- pruebas de bibliotecas;
- revisión bibliográfica;
- adquisición de datos;
- primeros análisis;
- pruebas de modelos, si el proyecto ya alcanzó esa etapa.

No es necesario presentar resultados sofisticados.

Lo importante es mostrar **evidencia concreta del proceso realizado**.

##4.7 Pipeline provisional

Cada proyecto debería intentar representar su trabajo mediante un pipeline.

Una estructura genérica podría ser:

```text
datos
  ↓
organización / auditoría
  ↓
preprocesamiento
  ↓
exploración
  ↓
representación / características
  ↓
análisis o modelo
  ↓
evaluación
  ↓
interpretación
```

Este pipeline debe adaptarse al proyecto.

No todos los proyectos necesitarán todas estas etapas y algunas podrán aparecer, desaparecer o cambiar durante el semestre.

---

## 5. Planificación de los tres hitos

El proyecto se desarrollará progresivamente durante el semestre.

##Hito 1 — fines de septiembre

```text
Estado inicial organizado del proyecto
```

Esperamos observar:

- problema definido;
- pregunta provisional;
- datos identificados o en proceso de selección;
- repositorio GitHub organizado;
- primeras evidencias de trabajo;
- pipeline inicial;
- próximos pasos.

##Hito 2 — fines de octubre

```text
Desarrollo
+
primeras evidencias
+
decisiones metodológicas
```

Esperamos observar una evolución del proyecto:

- datos mejor comprendidos;
- análisis o procesamiento en desarrollo;
- decisiones justificadas;
- resultados o evidencias intermedias;
- dificultades encontradas;
- posibles reformulaciones.

##Hito 3 — fines de noviembre

```text
Estado final alcanzado
+
resultados
+
limitaciones
+
próximos pasos
```

El Hito 3 corresponde al cierre del semestre, pero no implica necesariamente haber completado toda la idea inicial.

Será importante explicar:

- hasta dónde llegó realmente el proyecto;
- qué aprendimos;
- qué resultados se obtuvieron;
- qué limitaciones permanecen;
- y cuál sería el siguiente paso si el proyecto continuara.

> **Esta planificación no constituye un contrato rígido. El proyecto puede cambiar a medida que conocemos mejor los datos y el problema.**

---

## 6. Próximos pasos y dificultades

La presentación debería cerrar identificando:

- principales dificultades;
- preguntas todavía abiertas;
- herramientas que aún necesitan aprender;
- decisiones que todavía no pueden tomar;
- y el siguiente paso concreto del proyecto.

Una pregunta importante será:

> **¿Cuál es la próxima acción concreta que realizaremos después de este hito?**

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

Las referencias deben presentarse de forma clara y suficiente para poder identificar la fuente utilizada.

---

## 8. Declaración de uso de inteligencia artificial

Cada presentación debe incluir una **declaración explícita de uso de herramientas de inteligencia artificial**.

La declaración debe indicar:

- si se utilizaron herramientas de IA;
- cuáles se utilizaron;
- y para qué fueron utilizadas.

Por ejemplo:

> *Se utilizaron herramientas de IA generativa como apoyo para discutir la organización inicial del proyecto y revisar redacción. Las decisiones metodológicas, la revisión de datos y la interpretación del trabajo fueron realizadas por el equipo.*

Este texto es solamente un ejemplo.

Cada equipo debe declarar **su uso real** de estas herramientas.

---

## 9. Pauta de evaluación

| Criterio | Qué observaremos | Ponderación |
| --- | --- | ---: |
| **1. Definición del problema y motivación** | Claridad, contexto, pertinencia y capacidad para explicar profesionalmente qué se quiere estudiar. | **15%** |
| **2. Pregunta, objetivo y alcance inicial** | Especificidad de lo que se desea investigar o explorar y coherencia con el tiempo disponible. | **15%** |
| **3. Datos y comprensión inicial del material de trabajo** | Fuente, organización, características, limitaciones y comprensión de qué representan los datos. | **15%** |
| **4. Repositorio GitHub y organización computacional** | Repositorio accesible, `README.md`, estructura de carpetas, orden, documentación inicial y trazabilidad del trabajo. | **20%** |
| **5. Estado actual y evidencia de avance** | Evidencia concreta de exploración, preparación, pruebas o análisis realizados hasta el momento. | **10%** |
| **6. Pipeline y planificación Hitos 1–2–3** | Coherencia del camino propuesto, próximos pasos y capacidad de reconocer que el plan puede evolucionar. | **10%** |
| **7. Comunicación profesional y manejo del tiempo** | Claridad oral, terminología apropiada, calidad visual, organización de la presentación y ajuste a 10 minutos. | **10%** |
| **8. Referencias y declaración de uso de IA** | Fuentes identificadas correctamente y declaración transparente del uso de IA. | **5%** |
|  | **Total** | **100%** |

---

## 10. ¿Qué se valorará especialmente?

No se evaluará el proyecto solamente por cuánto de la idea inicial haya sido completado.

Tampoco se premiará automáticamente:

- utilizar más algoritmos;
- utilizar un modelo más complejo;
- escribir más código;
- tener más resultados;
- o encontrarse en una etapa más avanzada que otro grupo.

Nos interesará especialmente:

- comprender el problema;
- comprender los datos;
- organizar el proyecto;
- documentar el proceso;
- justificar decisiones;
- mostrar evidencia del trabajo realizado;
- reconocer dificultades y limitaciones;
- y saber cómo continuar.

> **No todos los proyectos partirán desde el mismo lugar ni llegarán al mismo punto.**

> **Un proyecto bien organizado y documentado, que muestra comprensión del problema y evidencia de un proceso serio, puede constituir un excelente Hito 1 aunque todavía se encuentre en una etapa inicial.**

---

## 11. Preguntas posteriores a la presentación

Después de los 10 minutos de presentación tendremos aproximadamente **5 minutos de preguntas**.

Las preguntas pueden abordar aspectos como:

- ¿por qué eligieron esos datos?;
- ¿qué representa exactamente esa etiqueta?;
- ¿qué dificultad consideran más importante?;
- ¿qué harían si no consiguen suficientes datos?;
- ¿por qué están considerando esa metodología?;
- ¿qué parte todavía no saben resolver?;
- ¿qué aprendieron al revisar sus primeros datos?;
- ¿qué cambiarían de su idea inicial?;
- ¿cuál será su próximo experimento, notebook, análisis o commit?

El propósito de estas preguntas no es buscar una respuesta perfecta.

Buscamos comprobar que el equipo **comprende el proyecto que está construyendo y puede razonar sobre sus propias decisiones**.

---

## 12. Para llevarse de este hito

El Hito 1 representa una primera fotografía organizada del proyecto.

Queremos poder decir:

```text
tenemos una idea
      ↓
la transformamos en una pregunta
      ↓
identificamos datos
      ↓
organizamos un repositorio
      ↓
comenzamos a explorar
      ↓
documentamos lo realizado
      ↓
sabemos cuál es nuestro próximo paso
```

Ese será el punto de partida para continuar desarrollando el proyecto durante octubre y noviembre.
