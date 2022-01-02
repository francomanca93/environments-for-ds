<div align="center">
    <h1>Curso de Entorno de Trabajo para Ciencia de Datos con Jupyter Notebooks y Anaconda</h1>
    <img src="https://imgur.com/jycC8yS.png" width="">
</div>

## Tabla de contenidos

- [Introducción a las notebooks](#introducción-a-las-notebooks)
  - [¿En qué lugares programar para ciencia de datos?](#en-qué-lugares-programar-para-ciencia-de-datos)
    - [Notebooks Vs Scripts](#notebooks-vs-scripts)
  - [Google Colab: primeros pasos](#google-colab-primeros-pasos)
  - [Google Colab: ciencia de datos](#google-colab-ciencia-de-datos)
  - [Utilizar Deepnote](#utilizar-deepnote)
- [Configuración de VSCode](#configuración-de-vscode)
  - [Instalar VSCode](#instalar-vscode)
  - [Instalar WSL: usa Linux dentro de Windows](#instalar-wsl-usa-linux-dentro-de-windows)
    - [Cambio de PASS en WSL (Olvido, perdida, etc)](#cambio-de-pass-en-wsl-olvido-perdida-etc)
  - [Agregar extensiones para VSCode](#agregar-extensiones-para-vscode)
  - [Uso de VSCode notebooks](#uso-de-vscode-notebooks)
    - [Format Document](#format-document)
- [Entorno de desarrollo con Anaconda](#entorno-de-desarrollo-con-anaconda)
  - [¿Qué son los ambientes virtuales?](#qué-son-los-ambientes-virtuales)
  - [Instalar Conda a través de la terminal](#instalar-conda-a-través-de-la-terminal)
  - [Conda: crear y actualizar ambientes](#conda-crear-y-actualizar-ambientes)
  - [Conda: abrir VSCode Notebooks con tu ambiente creado](#conda-abrir-vscode-notebooks-con-tu-ambiente-creado)
  - [Conda: eliminar ambientes y librerías](#conda-eliminar-ambientes-y-librerías)
  - [Conda: comandos avanzados](#conda-comandos-avanzados)
  - [Acelerar la creación de ambientes virtuales con Mamba](#acelerar-la-creación-de-ambientes-virtuales-con-mamba)
  - [Bonus: divide y vencerás](#bonus-divide-y-vencerás)
- [¿Qué sigue con estas herramientas?](#qué-sigue-con-estas-herramientas)
  - [Cómo seguir tu camino en ciencia de datos](#cómo-seguir-tu-camino-en-ciencia-de-datos)

# Introducción a las notebooks

## ¿En qué lugares programar para ciencia de datos?

Existen muchas plataformas para trabajar en Data Science, se recomiendo usar algún Sistema Operativo basado en UNIX usando Linux, MacOS o WSL en Windows, en editores estan VSCode, PyCharm, Deepnote, Google Colab, y el que usaremos Jupyter, todo basado en Notebooks que te permiten ir ejecutando trozos de código, en el cual puedes escribir pocas lineas de código probarlas, asegurarse de que estén bien y seguir adelante con otro trozo, allí también se pueden añadir código, ecuaciones, gráficas, texto enriquecido, etc.

### Notebooks Vs Scripts

Ambos son útiles, aunque los Scripts son mas directos, los Notebooks te permiten ver lo que haces, a medida de que lo haces, en estos puedes encargarte de experimentar y hacer el prototipado de tu script y finalmente pasarlo a un Script cuando ya este listo y estés seguro de que todo funciona como es esperado.

## Google Colab: primeros pasos

Es una herramienta basada en la nube que te permite trabajar en notebooks, y se guardan en tu cuenta de Google Drive 😃.

**Nube vs local**: Ambas son útiles, pero se diferencian en la configuración de entornos, ya que en la nube ya están precargadas, y de local tienes que configurarlo manualmente. También es diferente el tiempo de ejecución y la escalabilidad: la nube tiene más poder porque puedes rentarlo!. 💸

**Google Colab**: Servicio en la nube basado en Jupyter Notebooks, no requiere configuración y tiene un trabajo a nivel de archivo (el notebook es la base). Tiene uso de gratuito de GPUs y TPUs para correr modelos grandes. ☁️

Puedes acceder a Google Colab desde tu drive o desde el navegador.

Para aprender Markdown --> [Markdown Guide](https://www.markdownguide.org/)

Las variables son persistentes (se conservan) entre celdas de código!. 🔥

Para llamar a la línea de comandos, debemos usar primero un signo de admiración `!` y luego un comando válido, por ejemplo `!pwd` o `!pip install session-info`.

## Google Colab: ciencia de datos

Podemos subir archivos a Colab para trabajar con ellos (también tienen datos de muestra) 🔢. Dándole click podemos previsualizar e incluso filtrar la tabla que hayamos subido.

Podemos montar nuestro Google Drive en nuestro Notebook, con lo que podremos trabajar con datos que estén en nuestro Drive. 🤓 Es lo más recomendable ya que los archivos no se eliminan al terminar la sesión.

Colab está enfocado a trabajar con Python (también puede usar otros lenguajes) y ya trae librerías de ciencia de datos precargadas como:

- matplotlib: Generación de gráficos a partir de listas o arrays.
- numpy: Cómputo científico para la manipulación de vectores.
- pandas: Manipulación y análisis de datos de tablas y series temporales.
- scipy: Herramientas y algoritmos matemáticos.
- seaborn: Visualización de datos estadísticos.

Google **Colaboratory** tiene code snipets, para que puedas utilizarlo y agilizar tu trabajo 🤯.

Con `ctrl + shift + p` abres la paleta de comandos, si escribes **shortcuts** o atajos de teclado te mostrará una lista de todos los atajos que puedes ejecutar en Colab.

## Utilizar Deepnote

[Deepnote](https://deepnote.com/) es un servicio en la nube basado en Jupyter Notebooks. No requiere configuración y tiene un trabajo a nivel de proyecto. Tiene colaboración en tiempo real, integración con múltiples Apps y tiene acceso a una terminal o línea de comandos integrada 😎.

Tiene también variables de entorno y permite publicar proyectos (para construir portafolio). 🎉

Podemos correr y agregar lo mismo que en Colab, pero además podemos subir archivos que se quedan siempre en el proyecto.

Permite previsualizar los archivos CSV de manera muy elegante 😄.

Parte de lo poderoso de Deepnote es que podemos **integrar** muchas cosas 🔥.

No solo podemos agregar celdas de código y de texto, si no que en la opción de **Bloque** vienen muchos más tipos, como `input, chart, dataframe sql`, etc 🤯. Puede crear gráficas de manera automática sin código!

Para acceder a los atajos de teclado usamos `Ctrl + i`.

También es importante resaltar que tenemos una **terminal integrada** 🤖.

# Configuración de VSCode

## Instalar VSCode

- **Editores de código**: Enfocados a multiples lenguajes. Se pueden potencial con extensiones o plugins. Por lo general son gratuitos. Mejor este 😄. Tenemos VSCode, Atom, etc.
- **IDE (entornos de desarrollo integrado)**: Enfocado a un solo lenguaje y seguimiento a un solo proyecto. Por lo general son de pago 💸. Tenemos Pycharm, Visual Studio, etc

![editores-ide](https://imgur.com/PbMyQlK.png)

[Instalacion de Visual Studio Code](https://code.visualstudio.com/download)

## Instalar WSL: usa Linux dentro de Windows

[Instalar WSL](https://docs.microsoft.com/es-mx/windows/wsl/install)

### Cambio de PASS en WSL (Olvido, perdida, etc)

- Abrir el `cmd.exe`
- Ejecutar el comando para entrar como root: `wsl -u root`
- Cambian la password del usuario con `passwd <user>` (se los va a pedir dos veces)
- Entran de vuelva a ubuntu y realizar alguna acción que requiera la pass, ejemplo actualizar los paquetes `sudo apt update`.

## Agregar extensiones para VSCode

- Hay muchas extensiones para VSCode que hacen trabajar con datos más cómodo. ☁️
- Se pueden instalar todas las [extensiones](https://marketplace.visualstudio.com/VSCode) directamente desde VSCode 😄.
- Es recomendable activar la **sincronización automática** en la nube, para que siempre puedas tener tu entorno de trabajo en cualquier lugar. Lo puedes contectar con tu cuenta de GitHub 🤖
- Hay extension para [**Python**](https://marketplace.visualstudio.com/items?itemName=ms-python.python) que incluye muchas funcionalidades 🔥.
- [**MagicPython**](https://marketplace.visualstudio.com/items?itemName=magicstack.MagicPython) sirve mucho para darle formato a Python y que sea más legible.
- Con [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode) tendremos un asistente de desarrollo con AI
- Las extensiones de [**Icon**](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) sirven para diferenciar tipos de archivos. 📁
- [**Rainbow Brackets**](https://marketplace.visualstudio.com/items?itemName=2gua.rainbow-brackets) sirve para cambiar los colores de los paréntesis y no tener errores 🌈.
- [**Remote Development**](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl) te descarga múltiples extensiones que te sirven trabajar de manera remota. 🌎

Con el comando `code --list-extensions` podremos ver un lista de las extensiones instaladas.

## Uso de VSCode notebooks

- [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks) son un nuevo estilo de Notebook, integrado dentro de VSCode 🤯.
- Puedes abrir VSCode en una carpeta específica para ver todos los archivos dentro (y solo esos). Menos distracción que tener todo abierto con WSL. 😆
- Podemos correr los archivos .py directamente en la terminal dando click en ▶️.
- Con las extensiones que instalamos, podemos darle formato de manera automática a nuestro código 🐍.
- Dentro de los Jupyter Notebook en VSCode podemos usar todas estas extensiones 💕. La extensión de los Notebooks es .ipynb. Podemos exportar los notebooks a texto plano!.

### Format Document

0. Seleccionamos el texto a formatear
1. `CTRL + SHIFT + P` se nos abre el **Command Palette**.
2. Buscamos **Format Document**
3. Con la extension `autopep8` si la tenemos instalada, si no, la instalamos, podremos ordenar el código.
4. Si tenemos librerias en orden distinto, podemos ordenarla alfabeticamente con **Sort Imports**, mejorando la legibilidad, codigo organizado y limpio.

# Entorno de desarrollo con Anaconda

## ¿Qué son los ambientes virtuales?

## Instalar Conda a través de la terminal

## Conda: crear y actualizar ambientes

## Conda: abrir VSCode Notebooks con tu ambiente creado

## Conda: eliminar ambientes y librerías

## Conda: comandos avanzados

## Acelerar la creación de ambientes virtuales con Mamba

## Bonus: divide y vencerás

# ¿Qué sigue con estas herramientas?

## Cómo seguir tu camino en ciencia de datos
