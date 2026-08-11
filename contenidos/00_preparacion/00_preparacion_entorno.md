# Preparación — Instalación de VS Code y Miniconda

Antes de comenzar la Clase 01 queremos disponer de una base de trabajo común.

Durante ACUS220 utilizaremos principalmente:

- **Visual Studio Code (VS Code)** como espacio de trabajo;
- la **terminal integrada de VS Code**;
- **Miniconda** para disponer de Python y Conda;
- **Conda** para crear y administrar entornos;
- las extensiones **Python** y **Jupyter** de VS Code.

> **Idea central**
>
> Lo importante no es memorizar comandos de Conda.
> Lo importante es comprender por qué cada proyecto puede necesitar su propio entorno,
> con una versión de Python y un conjunto de dependencias bien definidos.

---

## 1. Instalar Visual Studio Code

Descarga VS Code desde:

<https://code.visualstudio.com/>

Instala la versión correspondiente a tu sistema operativo.

Después de instalarlo:

1. abre VS Code;
2. selecciona el panel **Extensions**;
3. instala la extensión **Python** publicada por Microsoft;
4. instala la extensión **Jupyter** publicada por Microsoft.

---

## 2. Instalar Miniconda

Miniconda es una distribución pequeña que incluye Python, Conda y las dependencias básicas necesarias para comenzar.

No instalaremos todas las librerías científicas de una vez. Las iremos agregando progresivamente cuando aparezca una necesidad concreta en el curso.

La instalación depende del sistema operativo.

---

### 2.1 Windows

**Paso 1. Descargar Miniconda**

Ve al sitio oficial:

<https://www.anaconda.com/download>

Busca la sección **Miniconda** y selecciona:

**Windows 64-bit Graphical Installer**

El instalador quedará normalmente en la carpeta `Downloads`.

**Paso 2. Ejecutar el instalador**

Haz doble clic sobre el archivo descargado.

Durante la instalación:

1. acepta la licencia;
2. selecciona **Just Me**;
3. continúa con la carpeta de instalación propuesta;
4. completa la instalación.

Para un curso como ACUS220, la instalación para el usuario local es la opción más sencilla y evita requerir privilegios de administrador.

**Paso 3. Verificar la instalación**

Abre el menú Inicio de Windows y busca:

```text
Anaconda Prompt
```

Ábrelo.

Deberías observar algo parecido a:

```text
(base) C:\Users\tu_usuario>
```

Ejecuta:

```bash
conda --version
```

Luego:

```bash
python --version
```

Y finalmente:

```bash
conda list
```

Si estos comandos producen resultados sin errores, Miniconda está funcionando.

---

### 2.2 macOS — Apple silicon

Esta sección corresponde a los Mac recientes con procesadores Apple silicon (M1, M2, M3, M4, etc.).

**Paso 1. Descargar Miniconda**

Ve al sitio oficial:

<https://www.anaconda.com/download>

Busca **Miniconda** y selecciona:

```text
64-bit (Apple silicon) Graphical Installer
```

Se descargará un archivo `.pkg`.

**Paso 2. Ejecutar el instalador**

Haz doble clic sobre el archivo `.pkg`.

Sigue el asistente:

1. selecciona **Continue**;
2. acepta la licencia;
3. continúa con las opciones propuestas;
4. selecciona **Install**.

**Paso 3. Abrir una nueva terminal**

Cuando termine la instalación, abre una nueva ventana de Terminal.

Deberías observar algo parecido a:

```text
(base)
```

**Paso 4. Verificar**

Ejecuta:

```bash
conda --version
```

Luego:

```bash
python --version
```

Y:

```bash
conda list
```

Si `conda` no aparece inmediatamente, cierra completamente Terminal y vuelve a abrirla.

---

### 2.3 macOS — computadores Intel

Las versiones recientes de Miniconda ya no se distribuyen de la misma forma para computadores Mac con procesador Intel.

Si tu Mac es Intel:

1. no utilices el instalador actual para Apple silicon;
2. revisa los instaladores históricos disponibles en el archivo oficial de Miniconda;
3. si tienes dudas, consúltalo antes de instalar.

Archivo oficial:

<https://repo.anaconda.com/miniconda/>

Para saber qué procesador utiliza tu Mac puedes abrir:

```text
 → About This Mac / Acerca de este Mac
```

---

### 2.4 Linux — x86-64

En Linux utilizaremos normalmente la terminal.

**Paso 1. Abrir una terminal**

Abre tu terminal habitual.

**Paso 2. Descargar Miniconda**

Para computadores Linux x86-64:

```bash
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

Si no tienes `curl`, puedes utilizar:

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

**Paso 3. Ejecutar el instalador**

```bash
bash ~/Miniconda3-latest-Linux-x86_64.sh
```

Lee las instrucciones del instalador.

Cuando se solicite aceptar la licencia, responde:

```text
yes
```

Puedes aceptar la ruta de instalación propuesta presionando `Enter`.

Cuando el instalador pregunte si deseas inicializar Conda, responde:

```text
yes
```

**Paso 4. Reiniciar la terminal**

Cierra y vuelve a abrir la terminal.

Alternativamente, si utilizas bash:

```bash
source ~/.bashrc
```

Si utilizas zsh:

```bash
source ~/.zshrc
```

**Paso 5. Verificar**

Ejecuta:

```bash
conda --version
```

Luego:

```bash
python --version
```

Y:

```bash
conda list
```

---

## 3. Abrir la terminal integrada de VS Code

Una vez instalados VS Code y Miniconda, abre VS Code.

Selecciona:

```text
Terminal → New Terminal
```

Dependiendo del sistema operativo, probablemente aparecerá:

- **PowerShell** en Windows;
- **zsh** en macOS;
- **bash** en Linux.

Comprueba:

```bash
conda --version
```

y:

```bash
python --version
```

---

## 4. Una comprobación común para Windows, macOS y Linux

Para saber exactamente qué instalación de Python estamos utilizando, ejecuta:

```bash
python -c "import sys; print(sys.executable)"
```

Este comando funciona de la misma forma en Windows, macOS y Linux.

Más adelante lo utilizaremos para comprobar que realmente estamos ejecutando Python desde el entorno correcto.

---

## 5. Checklist

Antes de continuar con la Clase 01, comprueba:

- [ ] Tengo VS Code instalado.
- [ ] Tengo instalada la extensión Python de VS Code.
- [ ] Tengo instalada la extensión Jupyter de VS Code.
- [ ] Tengo Miniconda instalado.
- [ ] Puedo ejecutar `conda --version`.
- [ ] Puedo ejecutar `python --version`.
- [ ] Puedo abrir la terminal integrada de VS Code.
- [ ] Puedo ejecutar `python -c "import sys; print(sys.executable)"`.

Si alguna respuesta es **no**, no continúes instalando paquetes al azar.

Revisaremos primero qué parte de la instalación falta.

---

## 6. ¿Qué viene después?

Con esta base preparada podremos comenzar la Clase 01.

Allí no partiremos memorizando comandos. Primero discutiremos **qué es un entorno computacional**, por qué conviene aislar las dependencias de cada proyecto y qué problema intenta resolver esta forma de trabajo.

Después construiremos conscientemente nuestro primer entorno de ACUS220:

```text
computador
   ↓
proyecto
   ↓
entorno aislado
   ↓
Python
   ↓
librerías
   ↓
Jupyter / kernel
```

La instalación termina aquí.

El siguiente paso será comenzar a comprender y recorrer el **ecosistema computacional** de ACUS220.
