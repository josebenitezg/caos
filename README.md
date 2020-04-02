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

#### Tutorial para aquellos que no tienen mucha experiencia con Github.
0. Abrir la "Terminal" en macOS o Linux, y el "CMD" en Windows.
1. Descargar este repositorio y descomprimirlo o desde la terminal escribir `git clone https://github.com/josebenitezg/caos.git`
2. Busca el directorio donde descargaste/descomprimiste o clonaste el repositorio `cd ~/route/to/your/folder`
3. Ejecuta la aplicación que deseas visualizar. Ej.: `python logistic_interactive.py`

#### Si tienes algún probelma
0. Google the problem you're running into
1. If it seems to be a problem with **this** code, post in "Issues"

----

## Logistic Map - Interactive
`python logistic_interactive.py`
![Interactive](https://github.com/jonnyhyman/Chaos/blob/master/images/logistic-interactive.png?raw=true)


Aquí podemos apreciar el diagrama de Verhulst en función al tiempo, y el gráfico de difuración del mapa logístico.

#### Shortcuts:
- Barra espaciadora: play/pausa
- Tecla de borrado: resetear vista y animación

----

## 3D Mandelbrot Set
`python logistic_mandelbrot.py`
![Mandelbrot Set within Logistic Map GIF](https://github.com/jonnyhyman/Chaos/blob/master/images/logistic-mandelbrot.gif?raw=true)

Here we see the Mandelbrot set on the x-y plane, and iterations of the Mandelbrot set in the z axis. This reveals the bifurcation plot beneath the Mandelbrot set!

Final visualization is accomplished by a volume rendering of 1000x1000x1000 voxels, oversampled by 16 to reduce aliasing.

#### Additional Requirements


----

## Logistic Map Zoom
`python logistic_zoom.py`
![Logistic Map Zoom GIF](https://github.com/jonnyhyman/Chaos/blob/master/images/logistic-zoom.gif?raw=true)

- [Vispy](http://vispy.org) : `pip install vispy`
  - Note: The final version of the visualization used a custom version of Vispy, modified to improve the appearance of axes. I have not released this and don't plan to, but if you really need it please post in Issues a feature request.
