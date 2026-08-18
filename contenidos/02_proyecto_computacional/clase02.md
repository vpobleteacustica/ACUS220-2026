# Clase 02 — De una idea a un proyecto computacional

## Idea central

En las primeras clases hemos comenzado a construir nuestro entorno de trabajo. También hemos conversado sobre posibles proyectos para desarrollar durante el semestre.

Hoy daremos un paso diferente:

> **pasar de una idea que nos interesa a un proyecto computacional que podamos organizar, desarrollar, documentar y continuar.**

Una idea puede comenzar de manera muy abierta:

- analizar el llanto de bebés;
- estudiar un paisaje sonoro;
- explorar características de personas a partir de la voz;
- reconocer eventos acústicos;
- analizar vibraciones;
- comparar sonidos producidos por diferentes fuentes;
- estudiar cualquier otro fenómeno que **suene, se escuche o vibre**.

No necesitamos que la idea esté completamente resuelta hoy. Lo importante es comenzar a transformarla en una pregunta abordable y en un proceso de trabajo.

---

## 1. El proyecto como proceso

En ACUS220 el proyecto no se entiende solamente como un resultado final.

Durante el semestre aprenderemos a construir un **proceso computacional**:

```text
idea
  ↓
pregunta
  ↓
datos
  ↓
exploración
  ↓
decisiones metodológicas
  ↓
análisis
  ↓
resultados
  ↓
interpretación
  ↓
nuevas preguntas
```

Este proceso rara vez ocurre de manera perfectamente lineal.

Muchas veces tendremos que volver atrás:

```text
pregunta
   ↓
datos
   ↓
descubrimos una limitación
   ↓
reformulamos la pregunta
   ↓
ajustamos el alcance
```

Eso no significa que el proyecto haya fallado.

Significa que estamos aprendiendo de los datos y del problema.

---

## 2. ¿Qué esperamos lograr durante el semestre?

El proyecto se desarrollará durante aproximadamente tres meses. Durante ese período cada estudiante tendrá también otras asignaturas, actividades e intereses, y además partimos con experiencias computacionales diferentes.

Por eso, **no esperamos necesariamente completar toda la idea que imaginamos al comienzo del semestre**.

La idea inicial nos dará una dirección, pero el alcance real del proyecto irá apareciendo a medida que conozcamos mejor los datos, las herramientas y las dificultades del problema.

Por ejemplo, un grupo podría recorrer:

```text
dataset
→ auditoría
→ visualización
→ características acústicas
→ modelo
→ evaluación
```

Mientras que otro podría recorrer:

```text
dataset
→ auditoría
→ descubrir problemas en las etiquetas
→ reformular la pregunta
→ caracterización acústica
```

Y otro podría llegar hasta:

```text
búsqueda de datos
→ comparación de posibles corpus
→ selección
→ organización
→ primeras visualizaciones
```

Estos recorridos no representan necesariamente proyectos mejores o peores.

Lo que nos interesará observar es **cómo evoluciona cada proyecto desde su propio punto de partida**.

> **El objetivo principal no es llegar lo más lejos posible ni utilizar las herramientas más complejas, sino aprender a desarrollar un proyecto de manera organizada, crítica, documentada y reproducible.**

Durante el semestre será completamente válido modificar una pregunta, reducir el alcance, cambiar una metodología o incluso abandonar una estrategia que inicialmente parecía apropiada.

Lo importante será poder explicar **por qué** se tomó esa decisión y qué aprendimos durante el proceso.

Al presentar los avances deberíamos ser capaces de contar una historia como esta:

```text
queríamos estudiar...
        ↓
encontramos estos datos...
        ↓
observamos...
        ↓
decidimos...
        ↓
probamos...
        ↓
descubrimos...
        ↓
por eso modificamos...
        ↓
ahora estamos aquí...
        ↓
el próximo paso sería...
```

Al finalizar el semestre queremos poder responder con claridad:

- ¿qué queríamos estudiar?;
- ¿qué datos encontramos o construimos?;
- ¿qué aprendimos acerca de esos datos?;
- ¿qué decisiones metodológicas tomamos y por qué?;
- ¿qué herramientas aprendimos a utilizar?;
- ¿qué dificultades encontramos?;
- ¿qué logramos desarrollar?;
- ¿qué quedó pendiente?;
- ¿qué cambiaríamos si comenzáramos nuevamente?;
- ¿y cuál sería el siguiente paso si continuáramos el proyecto?

---

## 3. Trabajar solos o en grupo

El proyecto puede desarrollarse:

- individualmente;
- en parejas;
- o en grupos de hasta **tres integrantes**.

Trabajar en grupo no significa simplemente repartir tareas.

Durante el semestre iremos aprendiendo herramientas que permiten que varias personas puedan contribuir a un mismo proyecto, mantener una estructura común y documentar los cambios realizados.

Más adelante utilizaremos **Git y GitHub** para apoyar este trabajo.

---

## 4. De una idea a una pregunta

Supongamos que nuestra idea inicial es:

> *Quiero trabajar con el sonido del llanto de bebés.*

Todavía no tenemos una pregunta.

Podríamos preguntarnos:

- ¿queremos detectar cuándo existe llanto?;
- ¿queremos caracterizar acústicamente diferentes grabaciones?;
- ¿queremos estudiar su contenido espectral?;
- ¿queremos explorar si aparecen agrupamientos?;
- ¿queremos comparar categorías disponibles en un corpus?;
- ¿queremos construir posteriormente un clasificador?

Una primera pregunta provisional podría ser:

> **¿Qué características acústicas permiten describir y explorar diferencias entre grabaciones de llanto infantil?**

La palabra **provisional** es importante.

La pregunta podrá cambiar cuando conozcamos mejor los datos.

---

## 5. Antes del modelo vienen los datos

Es frecuente comenzar un proyecto diciendo:

> *Quiero usar una red neuronal.*

o:

> *Quiero entrenar un Random Forest.*

Pero antes debemos responder preguntas más fundamentales:

> **¿Qué datos tenemos realmente?**

Preguntas iniciales:

- ¿De dónde provienen los datos?
- ¿Cuántos archivos existen?
- ¿Qué contiene cada archivo?
- ¿Qué representa una observación?
- ¿Existen etiquetas?
- ¿Quién creó esas etiquetas?
- ¿Qué tan confiables son?
- ¿Existen clases desbalanceadas?
- ¿Cuál es la duración de las señales?
- ¿Cuál es su frecuencia de muestreo?
- ¿Podemos utilizar esos datos de manera ética y legal?
- ¿Los datos permiten responder la pregunta que queremos estudiar?

Una regla útil para el curso será:

> **Primero conocemos los datos. Después elegimos las herramientas.**

---

## 6. Definir un alcance inicial

Una idea interesante puede crecer rápidamente hasta convertirse en un proyecto demasiado grande.

Por ejemplo:

> *Construiremos un sistema que identifique automáticamente las causas del llanto de un bebé.*

Para un semestre, podría ser mucho más razonable comenzar con:

```text
obtener un corpus
      ↓
comprender su estructura
      ↓
escuchar ejemplos
      ↓
visualizar señales y espectrogramas
      ↓
extraer algunas características
      ↓
explorar diferencias
```

Si luego existe tiempo y los datos lo permiten:

```text
clasificación
      ↓
comparación de modelos
      ↓
evaluación
```

El **alcance inicial** no es una promesa de todo lo que debemos terminar.

Es una primera delimitación de hacia dónde queremos avanzar.

---

## 7. Dibujar el pipeline antes de programar

Antes de escribir código, intentaremos representar el proyecto como una secuencia de etapas.

Una estructura general podría ser:

```text
Datos originales
       ↓
Auditoría
       ↓
Preprocesamiento
       ↓
Representación
       ↓
Características
       ↓
Exploración
       ↓
Modelo
       ↓
Evaluación
       ↓
Interpretación
```

No todos los proyectos necesitarán todas estas etapas.

Por ejemplo, un proyecto exploratorio puede no necesitar un modelo.

Otro proyecto puede requerir una etapa adicional de adquisición o anotación de datos.

El objetivo del diagrama es poder responder:

> **¿Dónde estamos ahora y cuál podría ser nuestro siguiente paso?**

---

## 8. La estructura también es parte del proyecto

Un proyecto computacional no debería convertirse en una carpeta llena de archivos con nombres como:

```text
prueba.py
prueba2.py
prueba_final.py
prueba_final_ahora_si.py
```

Desde el comienzo intentaremos construir una estructura comprensible.

Una estructura inicial muy sencilla puede ser:

```text
mi_proyecto/
├── README.md
├── data/
└── notebooks/
```

Más adelante podría crecer hacia algo como:

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

No necesitamos crear todas estas carpetas hoy.

La estructura debe crecer junto con el proyecto.

---

## 9. El README como memoria viva

El archivo `README.md` será uno de los primeros documentos de cada proyecto.

No será un informe final.

Será una **memoria viva del proyecto**.

Podrá evolucionar durante el semestre:

```text
README v0
idea inicial
     ↓
README v1
pregunta + datos
     ↓
README v2
primer análisis
     ↓
README v3
pipeline actualizado
     ↓
README final
estado del proyecto + resultados + próximos pasos
```

Es completamente válido que el README cambie porque la pregunta, los datos o el alcance también cambiaron.

---

## 10. Actividad de hoy — Organizar nuestro proyecto

Cada estudiante o grupo comenzará a construir una primera descripción organizada de su proyecto.

> **El objetivo de esta actividad no es resolver hoy el proyecto ni definir una metodología definitiva. Al terminar la clase, cada grupo debería contar con una primera versión organizada y documentada de su proyecto, suficientemente clara como para saber qué quiere estudiar, qué necesita investigar y cuál será su próximo paso.**

**10.1 Título provisional**

No tiene que ser definitivo.

Ejemplo:

> **Caracterización acústica exploratoria del llanto infantil**

**10.2 Integrantes**

Indicar los integrantes del proyecto.

Máximo tres personas.

**10.3 Idea inicial**

Explicar en pocas palabras qué fenómeno desean estudiar.

**10.4 Pregunta provisional**

Intentar formular **una pregunta principal**.

No necesitamos que sea perfecta.

**10.5 Motivación**

¿Por qué les interesa este problema?

¿Qué les gustaría aprender al desarrollarlo?

**10.6 Datos**

Describir lo que sabemos hasta ahora:

- ¿ya existen datos?;
- ¿hay algún dataset o repositorio disponible?;
- ¿tendremos que realizar grabaciones?;
- ¿qué tipo de archivos esperamos encontrar?;
- ¿hay etiquetas?;
- ¿qué información todavía necesitamos investigar?

**10.7 Alcance inicial**

¿Qué sería razonable intentar durante este semestre?

Separar, si es útil:

**Objetivo inicial**

```text
lo que pensamos que podríamos alcanzar
```

**Si existe tiempo**

```text
extensiones posibles
```

**10.8 Pipeline provisional**

Dibujar una primera secuencia del proyecto.

Por ejemplo:

```text
audios
  ↓
auditoría
  ↓
espectrogramas
  ↓
características acústicas
  ↓
exploración
  ↓
¿clasificación?
```

El signo `?` está permitido.

No tenemos que conocer todavía todas las respuestas.

**10.9 Posibles dificultades**

¿Qué podría dificultar el proyecto?

Por ejemplo:

- pocos datos;
- datos desbalanceados;
- problemas de calidad;
- etiquetas poco confiables;
- adquisición de grabaciones;
- desconocimiento de alguna metodología;
- capacidad computacional;
- tiempo disponible.

Identificar dificultades tempranamente **forma parte del proyecto**.

**10.10 Próximo paso**

Cada grupo debe terminar la clase pudiendo responder:

> **¿Cuál es la próxima acción concreta que podemos realizar?**

Ejemplos:

- descargar y revisar un dataset;
- buscar un corpus;
- escuchar diez grabaciones;
- estudiar cómo están organizadas las etiquetas;
- investigar una biblioteca de Python;
- definir qué variables contiene un archivo;
- discutir una reformulación de la pregunta.

**Al terminar la clase**

Cada grupo debería contar, al menos, con:

- integrantes definidos;
- un título provisional;
- una idea explicada en pocas palabras;
- una pregunta principal provisional;
- una primera identificación de los datos que necesitará;
- un alcance inicial razonable;
- un pipeline provisional, aunque tenga etapas todavía desconocidas;
- una lista breve de dificultades o preguntas abiertas;
- y **una próxima acción concreta**.

> **No importa que algunas respuestas todavía sean “no sabemos”. Lo importante es identificar qué necesitamos averiguar para poder continuar.**

Lo que construyamos hoy será la base de la primera versión del `README.md` de cada proyecto. No necesitamos que esté terminado: comenzaremos a utilizarlo como registro de cómo evoluciona nuestra idea durante el semestre.

---

## 11. Plantilla inicial del README

Cada proyecto podrá comenzar con una estructura como esta:

```markdown
# Título provisional del proyecto

## Integrantes

- Nombre
- Nombre
- Nombre

## Idea del proyecto

Descripción breve de la idea.

## Pregunta principal

Pregunta provisional que queremos estudiar.

## Motivación

¿Por qué nos interesa este problema?
¿Qué esperamos aprender?

## Datos

- Fuente:
- Tipo de datos:
- Formato:
- Cantidad aproximada:
- Etiquetas disponibles:
- Aspectos que todavía debemos investigar:

## Alcance inicial

¿Qué pensamos que sería razonable desarrollar durante el semestre?

## Pipeline provisional

Datos
→ ...
→ ...
→ ...

## Posibles dificultades

- ...
- ...

## Estado actual

¿Qué hemos realizado hasta ahora?

## Próximos pasos

1. ...
2. ...
3. ...
```

No necesitamos completar todas las secciones perfectamente hoy.

La plantilla existe para **ayudarnos a pensar**.

---

## 12. Hitos del proyecto

Durante el semestre tendremos **hitos de avance**.

Los hitos no buscan premiar solamente a quien haya llegado al algoritmo más complejo ni exigir que todos los grupos se encuentren en la misma etapa.

> **Los hitos no son puntos de llegada. Son momentos para detenernos, organizar la evidencia disponible y explicar cómo está evolucionando el proyecto.**

En cada hito será importante mostrar no solo lo que logramos, sino también las preguntas que aparecieron, las dificultades encontradas, las decisiones tomadas y los cambios realizados respecto de la idea inicial.

Una forma de pensar esta evolución es:

```text
Hito 1
¿qué queremos hacer y cómo pensamos comenzar?
        ↓
trabajo entre hitos
        ↓
Hito 2
¿qué ocurrió realmente cuando comenzamos a trabajar?
        ↓
qué aprendimos
        ↓
qué modificamos
        ↓
qué sigue
```

**Hito 1 — De la idea al proyecto**

Esperaremos poder explicar de manera organizada:

- cuál es la idea;
- cuál es la pregunta provisional;
- quiénes integran el grupo;
- qué datos utilizarán o están buscando;
- cómo están organizando el proyecto;
- cuál es el alcance inicial;
- qué dificultades han identificado;
- cuáles son los siguientes pasos.

También será valioso mostrar alguna primera evidencia de que el proyecto comenzó a tomar forma. Por ejemplo:

- corpus, datasets o fuentes que encontraron;
- algunos archivos que hayan revisado;
- literatura, documentación o repositorios consultados;
- una primera estructura de carpetas;
- una versión inicial del `README.md`;
- preguntas que todavía permanecen abiertas.

No es necesario que en este primer hito exista ya un modelo, un análisis completo o incluso código avanzado.

**Hito 2 — Evolución del proyecto**

Más adelante mostraremos cómo fue cambiando el proyecto cuando comenzamos a trabajar realmente con los datos y las herramientas.

Podremos organizar la presentación mediante una secuencia como esta:

```text
lo que planeamos
      ↓
lo que efectivamente pudimos hacer
      ↓
evidencia obtenida
      ↓
problemas encontrados
      ↓
decisiones tomadas
      ↓
estado actual
      ↓
siguiente paso
```

Será importante poder mostrar:

- cómo cambió la pregunta, si fue necesario;
- qué datos logramos reunir;
- cómo los auditamos y organizamos;
- qué notebooks, scripts o herramientas hemos construido;
- qué primeras evidencias o resultados encontramos;
- qué decisiones metodológicas tomamos y por qué;
- qué dificultades aparecieron;
- qué estrategias funcionaron y cuáles no;
- hasta dónde logramos avanzar;
- qué haríamos a continuación si continuáramos el proyecto.

Las afirmaciones que hagamos deberían apoyarse, cuando corresponda, en evidencia del propio proyecto: datos, notebooks, figuras, tablas, código, documentación o resultados intermedios.

Las fechas y detalles de cada presentación serán informados durante el curso.

---

## 13. ¿Qué se valorará?

Los proyectos pueden partir desde lugares diferentes y avanzar a ritmos distintos. Por eso, no nos interesa comparar solamente quién llegó más lejos o quién utilizó la herramienta más sofisticada.

Nos interesará especialmente **cómo evoluciona cada proyecto desde su propio punto de partida**.

Podemos organizar lo que se valorará en cinco dimensiones.

**Comprender el problema**

- ¿Podemos explicar con claridad qué queremos estudiar?
- ¿Podemos explicar por qué esa pregunta nos interesa?
- ¿El alcance que proponemos es razonable para el tiempo disponible?

**Comprender los datos**

- ¿Sabemos de dónde provienen?
- ¿Comprendemos qué contiene cada observación o archivo?
- ¿Reconocemos posibles limitaciones, sesgos, problemas de calidad o incertidumbres?
- ¿Podemos explicar si los datos realmente permiten estudiar nuestra pregunta?

**Construir un proceso**

- ¿El proyecto está organizado de manera comprensible?
- ¿Podemos seguir cómo se realizaron los análisis?
- ¿Los notebooks, scripts, datos y resultados tienen una estructura clara?
- ¿Estamos documentando el proceso para poder retomarlo y continuar?

**Tomar y justificar decisiones**

- ¿Podemos explicar por qué elegimos una determinada herramienta o metodología?
- ¿Podemos justificar por qué modificamos una pregunta, un alcance o una estrategia?
- ¿Somos capaces de reconocer cuando algo no funcionó y aprender de ello?

**Aprender y continuar**

- ¿Podemos explicar qué aprendimos durante el proceso?
- ¿Reconocemos qué logramos y qué todavía no sabemos?
- ¿Podemos identificar las principales limitaciones?
- ¿Tenemos claridad acerca de cuál sería el siguiente paso?

No se evaluará el proyecto solamente por:

- cuántos algoritmos se utilizaron;
- qué tan complejo fue el modelo;
- cuántas líneas de código se escribieron;
- o si se alcanzó exactamente todo lo imaginado al comienzo.

> **No todos los proyectos partirán desde el mismo lugar ni llegarán al mismo punto. Nos interesará especialmente la evolución de cada proyecto respecto de su propio punto de partida y la capacidad del grupo para documentar y explicar esa evolución.**

> **Un proyecto bien documentado que descubre una limitación importante puede ser mucho más valioso que un modelo complejo que no comprendemos.**

---

## 14. Una idea importante para llevarse de esta clase

Al terminar el curso no esperamos que todos se hayan convertido en especialistas en aprendizaje de máquina, procesamiento de audio o ciencia de datos.

Esperamos algo diferente:

> **que frente a un nuevo problema sepan mucho mejor cómo comenzar, cómo organizarlo, cómo comprender los datos, cómo explorar herramientas, cómo documentar lo que hicieron y cómo continuar avanzando.**

Ese proceso puede seguir creciendo mucho después de terminado ACUS220.

---

## 15. Lo que viene

Hoy estamos construyendo:

```text
idea
  ↓
pregunta
  ↓
datos
  ↓
alcance
  ↓
estructura
  ↓
README
```

En la próxima etapa aprenderemos cómo transformar esa carpeta en un proyecto cuya evolución podamos registrar y compartir:

```text
proyecto local
      ↓
     Git
      ↓
   GitHub
      ↓
historia reproducible del proyecto
```

Git y GitHub aparecerán entonces no como herramientas aisladas, sino como parte del ecosistema que estamos construyendo.
