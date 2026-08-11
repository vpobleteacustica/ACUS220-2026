# ACUS220 — Acústica Computacional con Python

Material docente del curso **ACUS220 — Acústica Computacional con Python**, Universidad Austral de Chile.

El curso propone una idea central:

> aprender Python no termina cuando aprendemos su sintaxis.

A lo largo del semestre utilizaremos Python como puerta de entrada a un ecosistema de herramientas para desarrollar proyectos científicos y de ingeniería: entornos reproducibles, Jupyter, manejo y visualización de datos, procesamiento de audio, modelos, aprendizaje de máquina, Git y GitHub.

## Jupyter Book

La versión publicada del curso está disponible en:

**https://vpobleteacustica.github.io/ACUS220-2026/**

## Propósito del curso

ACUS220 es un curso optativo orientado a estudiantes provenientes de Acústica y otras áreas de la ingeniería.

El objetivo no es memorizar una colección de comandos ni dominar todas las herramientas disponibles. Buscamos desarrollar progresivamente **autonomía computacional**: aprender a explorar herramientas nuevas, organizar proyectos, comprender datos, probar metodologías, evaluar resultados, documentar decisiones y construir procesos de trabajo que puedan ser comprendidos y reproducidos por otras personas.

Los problemas vinculados con la acústica serán nuestro punto de partida, pero el curso busca también construir un **lenguaje computacional común** que facilite el trabajo interdisciplinario.

## Contenidos iniciales

El Book comienza con:

- preparación del entorno de trabajo;
- instalación de Visual Studio Code y Miniconda;
- introducción a entornos de Python;
- Jupyter Notebooks y kernels;
- organización de proyectos computacionales;
- reproducibilidad;
- referencias y documentación fundamental.

Durante el semestre se incorporarán progresivamente nuevos contenidos y actividades.

## Estructura del repositorio

```text
ACUS220-2026/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── assets/
│   ├── images/
│   └── site.css
├── contenidos/
│   ├── 00_preparacion/
│   ├── 01_entorno_computacional/
│   └── referencias.md
├── footer.md
├── index.md
├── myst.yml
├── references.bib
└── README.md
```

## Construcción local

El Book está desarrollado con **Jupyter Book / MyST**.

Para trabajar localmente, con el entorno correspondiente activado:

```bash
jupyter book start
```

El sitio local estará disponible normalmente en:

```text
http://localhost:3000
```

## Publicación

El repositorio utiliza **GitHub Actions** para construir y publicar automáticamente el Book mediante GitHub Pages.

Cada `push` a la rama `main` ejecuta el workflow de despliegue definido en:

```text
.github/workflows/deploy.yml
```

## Autores

**Víctor Poblete**  
Instituto de Acústica  
Universidad Austral de Chile

**Carlos Duarte**  
Escuela de Ingeniería Civil en Informática  
Universidad Austral de Chile

## Referencias

El Book incluye documentación oficial de Python, Conda, Visual Studio Code, Jupyter, Git y GitHub, junto con lecturas fundamentales sobre reproducibilidad, organización de proyectos computacionales, Jupyter Notebooks y control de versiones.

---

© 2026 · ACUS220 · Universidad Austral de Chile
