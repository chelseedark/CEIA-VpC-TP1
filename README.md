# TP1 - Visión por Computadora I

Esta carpeta contiene la resolución del TP1 de la materia Visión por Computadora I (CEIA / FIUBA). El trabajo consiste en dos partes: implementar el algoritmo White Patch para corregir diferencias de color por iluminación, y analizar los histogramas de dos imágenes en escala de grises.

## Contenido

- `TP1.ipynb`: resolución del trabajo práctico.
- `img1_tp.png` e `img2_tp.png`: imágenes de entrada para la parte de histogramas.
- `white_patch/`: imágenes de entrada para la parte de White Patch.
- `requirements.txt`: dependencias necesarias para correr el notebook.
- `README.md`: este archivo.

## Entorno

Para correr el notebook se usa un entorno conda llamado `vision_cv`. Fue creado a partir del entorno `ia_env` agregando la librería de OpenCV, que es la única que faltaba para este trabajo.

Características del entorno:

- Python 3.12.13
- opencv-python 5.0.0
- numpy 2.5.0
- matplotlib 3.11.0
- jupyter (IPython 9.15.0, notebook)

## Creación del entorno en esta computadora

El entorno local se creó con estos comandos:

```
conda create -n vision_cv --clone ia_env
conda activate vision_cv
pip install opencv-python
```

## Creación del entorno en otra computadora

Para reproducir el entorno desde cero en otra máquina alcanza con:

```
conda create -n vision_cv python=3.12
conda activate vision_cv
pip install -r requirements.txt
```

El archivo `requirements.txt` reúne los paquetes que se necesitan para resolver este trabajo.

## Cómo ejecutar el notebook

Con el entorno activado, abrir Jupyter y lanzar el notebook:

```
conda activate vision_cv
jupyter notebook TP1.ipynb
```

La carpeta de trabajo debe ser esta misma carpeta, porque el notebook lee las imágenes con rutas relativas.
