# Caos
#### Visualización de una conexión de la teoría del caos, fractales y mapas lógicos.
###### Código escrito originalmente por [Jonny Hyman](https://www.jonnyhyman.com), 2020

Este codigo fue desarrollado para [Este video de Youtube de Veritasium](https://www.youtube.com/watch?v=ovJcsL7vyrk)

Esto no es una librería, esto es una traducción y algunas mejoras dentro de la aplicación.

# MiniTutorial

#### Requerimientos de instalación
- [Python 3.6+](https://www.anaconda.com/distribution/) (testeado en Python 3.6 y Python 3.7, macOS Catalina y Windows 10)
- [Numpy](https://numpy.org) package : `pip install numpy`
- [Numba](https://numba.pydata.org) package : `pip install numba`
- PyQt5 : `pip install pyqt5`
- PyQtGraph : `pip install pyqtgraph` (Python 3.6, 3.7) o `pip install pyqtgraph==0.11.0rc0` (Python 3.8)
- [Vispy](http://vispy.org) : `pip install vispy`
- [Matplotlib](https://matplotlib.org) : `pip install matplotlib`
- [PyOpenGL](https://pypi.org/project/PyOpenGL/) : `pip install pyopengl`
- [ffmpeg](https://www.ffmpeg.org) Si quieres renderizar los frames a .movs
  - macOS: [Install homebrew](https://brew.sh) then `brew install ffmpeg`
  - Windows: [Install chocolatey](https://chocolatey.org) then `choco install ffmpeg`
- [Vispy](http://vispy.org) : `pip install vispy`
  - Nota: La versión final de esta repo usa la versión custom de Vispy. Se estará adaptando para nuevas versiones.

#### Tutorial para aquellos que no tienen mucha experiencia con Github.
0. Abrir la "Terminal" en macOS o Linux, y el "CMD" en Windows.
1. Descargar este repositorio y descomprimirlo o desde la terminal escribir `git clone https://github.com/josebenitezg/caos.git`
2. Busca el directorio donde descargaste/descomprimiste o clonaste el repositorio `cd ~/route/to/your/folder`
3. Ejecuta la aplicación que deseas visualizar. Ej.: `python logistic_interactive.py`

#### Si tienes algún probelma
0. Googlea el problema :P
1. Si tienes algún problema con **este** código, postea en "Issues"

----

## Logistic Map - Interactivo
`python logistic_interactive.py`
![Interactive](https://github.com/jonnyhyman/Chaos/blob/master/images/logistic-interactive.png?raw=true)


Aquí podemos apreciar el diagrama de Verhulst en función al tiempo, y el gráfico de difuración del mapa logístico.

#### Shortcuts:
- Barra espaciadora: play/pausa
- Tecla de borrado: resetear vista y animación

----

## El conjunto de Mandelbrot en 3D. (Requiere de mucha acelración gráfica)
`python logistic_mandelbrot.py`
![Mandelbrot Set within Logistic Map GIF](https://github.com/jonnyhyman/Chaos/blob/master/images/logistic-mandelbrot.gif?raw=true)

Aquí podemos ver el conjunto de Mandelbrot en 3D y las iteraciones en el eje Z. Esto nos demuestra que la bifurcación del diagrama de Verhulst es parte del conjunto de Mandelbrot!

La visualización final tiene un render de 1000x1000x1000 voxeles.

Voxel: unidad cúbica que representa una figura tridimensional.
----

## Logistic Map Zoom
`python logistic_zoom.py`
![Logistic Map Zoom GIF](https://github.com/jonnyhyman/Chaos/blob/master/images/logistic-zoom.gif?raw=true)


