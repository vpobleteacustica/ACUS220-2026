# Clase 01 — Python como un entorno de posibilidades

## ¿Qué hay después de aprender la sintaxis de Python?

Probablemente ya has escrito algún programa en Python.

Quizás has utilizado variables, condicionales, ciclos, funciones o listas. Tal vez has resuelto ejercicios numéricos o implementado algún algoritmo.

Pero aprender Python puede significar mucho más que aprender la sintaxis de un lenguaje.

En este curso comenzaremos a descubrir el **ecosistema de herramientas** que permite utilizar Python para desarrollar proyectos científicos y de ingeniería.

La pregunta que guiará esta primera clase será:

> **¿Qué necesitamos, además de saber escribir código, para desarrollar un proyecto computacional reproducible?**

---

## Antes de comenzar

En ACUS220 trabajaremos con estudiantes que pueden provenir de distintas áreas de la ingeniería y, por lo tanto, tener experiencias computacionales muy diferentes.

Algunas personas ya habrán utilizado Git, GitHub, terminales o entornos de Python. Para otras, varios de estos conceptos serán completamente nuevos.

Esa diversidad será parte del curso.

No buscamos que todas las personas comiencen sabiendo lo mismo. Buscamos construir progresivamente un **lenguaje computacional común** que nos permita colaborar, comprender proyectos de otras áreas y desarrollar nuestros propios flujos de trabajo.

Para las actividades prácticas utilizaremos principalmente:

- **Visual Studio Code (VS Code)** como espacio de trabajo;
- la **terminal integrada de VS Code**;
- **Miniconda/Conda** para administrar entornos;
- **Jupyter** para trabajar con notebooks.

La instalación de estas herramientas se encuentra en la página **Preparación — Instalación de VS Code y Miniconda**. En esta clase asumiremos que esa base ya está disponible y nos concentraremos en comprender cómo se relacionan sus componentes.

> **Idea importante**
>
> Lo fundamental no es aprender Conda como una colección de comandos.
> Lo fundamental es comprender **qué es un entorno, por qué aislamos las dependencias de un proyecto y cómo podemos reconstruir ese entorno en otro computador**.

---

## 1. ¿Desde dónde partimos?

Algunas de las siguientes palabras pueden resultarte familiares y otras quizás sean completamente nuevas:

- Python;
- terminal;
- Conda;
- entornos;
- paquetes y librerías;
- NumPy;
- pandas;
- Matplotlib;
- Jupyter;
- kernels;
- Visual Studio Code;
- Git;
- GitHub;
- datasets;
- modelos;
- aprendizaje de máquina.

Esto **no es una prueba**.

Es simplemente nuestro mapa inicial.

Durante el semestre iremos conectando progresivamente estos conceptos y aprendiendo cuándo y por qué utilizar cada herramienta.

### Actividad inicial

Antes de continuar, identifica cada concepto anterior como:

1. lo he utilizado;
2. he escuchado hablar de él;
3. es completamente nuevo para mí.

Compara después tus respuestas con las de otros estudiantes.

¿Qué conocimientos aparecen en común?

¿Qué diferencias existen entre estudiantes provenientes de distintas áreas de la ingeniería?

¿Qué puede aprender cada área de las otras?

---

## 2. Python es más que el lenguaje

Cuando aprendemos programación por primera vez, es natural identificar Python con el código que escribimos:

```python
print("Hola ACUS220")
```

o con estructuras como variables, condicionales, ciclos y funciones.

Todo eso forma parte del **lenguaje Python**.

Sin embargo, cuando comenzamos a desarrollar proyectos científicos o de ingeniería, aparece un ecosistema mucho más amplio.

Un proyecto puede necesitar, por ejemplo:

- una determinada versión de Python;
- librerías desarrolladas por otras personas;
- datos provenientes de mediciones o experimentos;
- notebooks para explorar esos datos;
- scripts para automatizar tareas;
- figuras y resultados;
- documentación;
- un sistema para registrar los cambios realizados;
- una forma de compartir el proyecto con otras personas.

Por eso, saber escribir código es solamente una parte del trabajo.

Podemos pensar en una transición como esta:

```text
sé escribir código en Python
            ↓
sé utilizar Python para desarrollar un proyecto
```

La segunda afirmación requiere nuevas herramientas y nuevas formas de organizar nuestro trabajo.

### Del programa aislado al proyecto

Consideremos dos situaciones.

**Situación A**

Una persona escribe un archivo:

```text
analisis.py
```

lo ejecuta en su computador y obtiene un resultado.

**Situación B**

Otra persona desarrolla un proyecto que contiene:

```text
proyecto/
│
├── datos/
├── notebooks/
├── scripts/
├── figuras/
├── README.md
└── información sobre el entorno computacional
```

Ambas personas pueden estar programando en Python.

Pero en el segundo caso comenzamos a reconocer algo distinto: existe una **estructura de proyecto**.

Esa estructura permite responder preguntas como:

- ¿de dónde vienen los datos?;
- ¿qué código produjo cada resultado?;
- ¿qué librerías fueron necesarias?;
- ¿qué decisiones se tomaron durante el análisis?;
- ¿podría otra persona ejecutar nuevamente el proyecto?;
- ¿podremos nosotros mismos comprenderlo dentro de seis meses?

Estas preguntas serán tan importantes en este curso como aprender nuevos comandos de Python.

### Una idea que nos acompañará durante el semestre

> **Un proyecto computacional no es solamente su código.**
>
> También incluye sus datos, dependencias, organización, decisiones, resultados y documentación.

A esta idea iremos agregando progresivamente conceptos como **entornos, reproducibilidad, Git y GitHub**.

---

## 3. ¿Qué es realmente un entorno computacional?

Supongamos que desarrollamos tres proyectos diferentes.

Uno utiliza una librería reciente; otro depende de una versión anterior; un tercero necesita herramientas completamente distintas.

Si instaláramos todo en un único Python global, con el tiempo podrían aparecer incompatibilidades.

Una forma de evitarlo es utilizar **entornos aislados**.

```text
computador
│
├── proyecto A
│   └── entorno A
│       ├── Python
│       └── librerías del proyecto A
│
├── proyecto B
│   └── entorno B
│       ├── Python
│       └── librerías del proyecto B
│
└── proyecto C
    └── entorno C
        ├── Python
        └── librerías del proyecto C
```

Un entorno permite asociar a un proyecto una determinada versión de Python y un conjunto específico de paquetes.

### ¿Por qué es útil?

Porque dos proyectos distintos pueden necesitar versiones diferentes de una misma librería.

También porque un entorno bien documentado ayuda a responder una pregunta fundamental:

> **¿Qué necesita otra persona para ejecutar este proyecto en su propio computador?**

Durante el curso utilizaremos **Conda** para crear y administrar nuestros entornos.

Conda será nuestra herramienta concreta, pero el concepto que queremos aprender es más general: **aislar y documentar las dependencias de un proyecto**.

---

## 4. ¿Quién es quién en este ecosistema?

Antes de ejecutar comandos, distingamos algunas piezas fundamentales.

### Python

Python es el **lenguaje de programación** que utilizaremos.

También llamamos Python al intérprete que ejecuta nuestro código.

### Librería o paquete

Una librería contiene código desarrollado por otras personas que podemos reutilizar.

Algunos ejemplos que iremos encontrando durante el curso son:

- **NumPy**: computación numérica y trabajo con arreglos;
- **pandas**: datos tabulares;
- **Matplotlib**: visualización;
- **SciPy**: herramientas de computación científica;
- **scikit-learn**: modelos y herramientas de aprendizaje de máquina.

Una parte importante del trabajo profesional consiste en aprender a **buscar, comprender y utilizar herramientas existentes**, en lugar de programarlo todo desde cero.

### Miniconda y Conda

**Miniconda** es una distribución mínima que utilizaremos para disponer de Python y Conda sin instalar desde el comienzo una gran colección de paquetes.

**Conda** es la herramienta que utilizaremos para:

- crear entornos;
- activar y desactivar entornos;
- instalar paquetes;
- mantener separados los requisitos de distintos proyectos.

### Jupyter Notebook

Un notebook permite combinar en un mismo documento:

- texto;
- ecuaciones;
- código;
- resultados;
- figuras;
- explicaciones.

Resulta especialmente útil para **explorar**, **documentar** y **comunicar** un análisis.

### Kernel

El kernel es el proceso que ejecuta el código de un notebook.

Un archivo `.ipynb` puede existir en nuestro computador, pero necesitamos decidir **qué Python** y **qué entorno** ejecutarán sus celdas.

### Visual Studio Code

Visual Studio Code, o VS Code, será uno de nuestros principales espacios de trabajo.

Desde una misma aplicación podremos trabajar con:

- archivos de Python;
- notebooks;
- Markdown;
- carpetas de proyectos;
- terminal;
- Git y otras herramientas.

### Git

Git es un **sistema de control de versiones**.

Nos permitirá registrar cómo cambia un proyecto a lo largo del tiempo.

### GitHub

GitHub es una plataforma que permite alojar repositorios Git y facilita compartir, documentar y colaborar en proyectos.

Git y GitHub están relacionados, pero **no son lo mismo**.

---

## 5. La terminal: conversar con nuestro computador

Muchos flujos de trabajo científicos utilizan una terminal.

La terminal puede parecer extraña al principio, pero no necesitamos aprender cientos de comandos.

Además, utilizaremos la **terminal integrada de VS Code** para que estudiantes de Windows, macOS y Linux trabajemos, en lo posible, desde un mismo espacio.

Según el sistema operativo, es habitual encontrar:

- **PowerShell** en Windows;
- **zsh** en macOS;
- **bash** en Linux.

Los intérpretes son diferentes, pero buena parte del flujo de trabajo que utilizaremos con Python y Conda será común.

### ¿Dónde estoy?

En macOS y Linux:

```bash
pwd
```

En PowerShell, `pwd` también está disponible como alias.

### ¿Qué hay aquí?

```bash
ls
```

En PowerShell, `ls` también puede utilizarse como alias.

### Moverse entre carpetas

```bash
cd nombre_carpeta
```

Para regresar al directorio superior:

```bash
cd ..
```

### ¿Qué versión de Python estoy utilizando?

```bash
python --version
```

### Una comprobación común a Windows, macOS y Linux

Para conocer exactamente qué ejecutable de Python estamos utilizando podemos escribir:

```bash
python -c "import sys; print(sys.executable)"
```

Este comando será especialmente útil cuando comencemos a cambiar entre distintos entornos.

No es necesario memorizar todos estos comandos ahora.

Lo importante es comprender que la terminal nos permite **observar y controlar nuestro entorno de trabajo**.

---

## 6. Construimos nuestro primer entorno

Hasta este punto hemos hablado del problema antes de hablar del comando: un proyecto necesita una forma de declarar y aislar las herramientas de las que depende.

Ahora llevaremos esa idea a la práctica y construiremos nuestro primer entorno.

**Paso 1. Revisar los entornos disponibles**

```bash
conda env list
```

Este comando muestra los entornos que Conda conoce en nuestro computador.

**Paso 2. Crear el entorno del curso**

```bash
conda create -n acus220_2026 -c conda-forge python=3.12
```

Aquí estamos indicando:

- `conda create`: queremos crear un entorno;
- `-n acus220_2026`: el entorno se llamará `acus220_2026`;
- `-c conda-forge`: utilizaremos el canal `conda-forge`;
- `python=3.12`: queremos una versión concreta de Python.

**Paso 3. Activar el entorno**

```bash
conda activate acus220_2026
```

Cuando el entorno está activo, el comienzo de la terminal debería mostrar algo parecido a:

```text
(acus220_2026)
```

**Paso 4. Verificar Python**

```bash
python --version
```

y luego utilizaremos una comprobación que funciona de la misma forma en los principales sistemas operativos:

```bash
python -c "import sys; print(sys.executable)"
```

La ruta mostrada debería apuntar al Python instalado dentro de `acus220_2026`.

### Pregunta

¿Qué cambiaría si ejecutáramos:

```bash
conda deactivate
```

y volviéramos a consultar:

```bash
python -c "import sys; print(sys.executable)"
```

La respuesta nos ayuda a comprender que **activar un entorno modifica qué instalación de Python estamos utilizando**.

---

## 7. Incorporamos herramientas al entorno

Un entorno recién creado contiene muy pocas cosas.

Eso es deliberado.

No queremos comenzar el curso con cientos de paquetes instalados sin saber para qué sirven. Iremos incorporando herramientas cuando aparezca una necesidad concreta.

Para preparar el trabajo inicial podemos instalar:

```bash
conda install -c conda-forge numpy pandas matplotlib jupyterlab ipykernel
```

Estas librerías se instalan **dentro del entorno que tenemos activo**.

Podemos comprobarlo desde Python:

```python
import numpy
import pandas
import matplotlib

print("Las librerías están disponibles.")
```

### Una idea importante

Nuestro proyecto comienza a tener no solamente código, sino también un conjunto de **dependencias**.

Una dependencia es una herramienta externa que nuestro proyecto necesita para funcionar.

Más adelante aprenderemos a registrar estas dependencias para que otras personas puedan reconstruir nuestro entorno.

---

## 8. Jupyter, notebooks y kernels

Para utilizar el entorno `acus220_2026` desde Jupyter podemos registrarlo como kernel.

```bash
python -m ipykernel install --user --name acus220_2026 --display-name "Python (ACUS220 2026)"
```

Después, al abrir un notebook, podremos seleccionar:

```text
Python (ACUS220 2026)
```

Esto significa que las celdas serán ejecutadas utilizando el Python y las librerías de nuestro entorno.

### Notebook y kernel no son lo mismo

Podemos pensar así:

```text
archivo notebook (.ipynb)
          │
          │ selecciona
          ↓
        kernel
          │
          │ ejecuta usando
          ↓
entorno de Python
```

Esta distinción será importante durante todo el curso.

---

## 9. Nuestro primer pequeño experimento

Creemos un notebook nuevo en VS Code y seleccionemos como kernel:

```text
Python (ACUS220 2026)
```

En la primera celda podemos escribir:

```python
import sys

print("Hola ACUS220")
print()
print("Python:", sys.version)
print("Ejecutable:", sys.executable)
```

La información mostrada por `sys.executable` debería apuntar al Python de nuestro entorno.

Ahora probemos algunas de las herramientas instaladas:

```python
import numpy as np
import pandas as pd
import matplotlib

print("NumPy:", np.__version__)
print("pandas:", pd.__version__)
print("Matplotlib:", matplotlib.__version__)
```

Este pequeño ejercicio no pretende enseñarnos todavía NumPy, pandas ni Matplotlib.

Su objetivo es comprobar una idea más fundamental:

> **Nuestro notebook está ejecutándose dentro del entorno que nosotros construimos.**

---

## 10. ¿Qué construimos realmente?

Hasta ahora podría parecer que solamente instalamos algunos programas.

Pero conceptualmente hicimos algo más interesante.

Construimos una relación entre:

```text
proyecto
   │
   ├── Python
   ├── entorno aislado
   ├── librerías
   ├── Jupyter
   ├── kernel
   └── herramientas de trabajo
   │
   ↓
base para un trabajo computacional reproducible
```

Durante el semestre iremos agregando progresivamente:

```text
datos
visualizaciones
audio
modelos
Git
GitHub
documentación
resultados
```

Hasta convertir esta estructura inicial en un proyecto computacional más completo.

---

## 11. Reproducibilidad: “en mi computador funcionaba”

Imagina que una persona te entrega un proyecto desarrollado hace dos años y te dice:

> “El código funcionaba perfectamente en mi computador.”

¿Qué necesitarías saber para intentar reproducir sus resultados?

Probablemente comenzaríamos a preguntar:

- ¿qué versión de Python utilizó?;
- ¿qué librerías instaló?;
- ¿qué versiones de esas librerías?;
- ¿dónde están los datos?;
- ¿cómo se ejecuta el análisis?;
- ¿qué archivo debe ejecutarse primero?;
- ¿qué decisiones fueron tomadas?;
- ¿qué resultados deberían obtenerse?

Ese conjunto de preguntas nos introduce en una idea central del curso:

> **Reproducibilidad significa que un análisis no dependa únicamente de la memoria, el computador o las configuraciones personales de quien lo creó.**

No lograremos reproducibilidad perfecta de inmediato.

La iremos construyendo progresivamente.

---

## 12. Para cerrar esta primera clase

Intenta explicar con tus propias palabras la diferencia entre:

- Python;
- una librería;
- un entorno;
- Miniconda;
- Conda;
- Jupyter;
- un notebook;
- un kernel;
- VS Code;
- Git;
- GitHub.

No importa que las definiciones todavía no sean perfectas.

Lo importante es comenzar a construir un **modelo mental del ecosistema**.

### Preguntas de cierre

1. ¿Por qué podría ser problemático instalar todas las librerías de todos nuestros proyectos en un único Python?
2. ¿Qué diferencia existe entre un notebook y el kernel que lo ejecuta?
3. ¿Qué información necesitarías para reproducir un proyecto desarrollado por otra persona?
4. ¿Qué herramientas de esta clase ya conocías?
5. ¿Qué herramientas aparecieron hoy por primera vez?
6. ¿Qué diferencias observaste entre las experiencias computacionales de estudiantes provenientes de distintas áreas?

---

## Para llevarse de esta clase

Python no será solamente el lenguaje con el cual escribiremos código.

Durante el semestre lo utilizaremos como puerta de entrada hacia un ecosistema que incluye:

```text
Python
   ↓
computación científica
   ↓
datos
   ↓
visualización
   ↓
audio
   ↓
modelos
   ↓
aprendizaje de máquina
   ↓
Git y GitHub
   ↓
reproducibilidad
   ↓
trabajo interdisciplinario
```

No necesitamos dominar todo esto hoy.

La idea de esta primera clase es simplemente comenzar a reconocer el mapa.

En las próximas clases iremos recorriéndolo paso a paso.
