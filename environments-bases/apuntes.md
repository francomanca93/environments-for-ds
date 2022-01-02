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
  - [Agregar extensiones para VSCode](#agregar-extensiones-para-vscode)
  - [Uso de VSCode notebooks](#uso-de-vscode-notebooks)
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

# Configuración de VSCode

## Instalar VSCode

## Instalar WSL: usa Linux dentro de Windows

## Agregar extensiones para VSCode

## Uso de VSCode notebooks

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
