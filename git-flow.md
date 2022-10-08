# WORK to GitFlow

Para trabajar con el metodo GitFlow tendremos las siguientes ramas:
- Master: En esta rama estara una version estable de nuestro repositorio.

- HotFix: En esta rama arreglaremos errores que pueden surgir de la rama Master, sin pasar por el proceso de produccion o develop, para no entorpecer con las nuevas caracteristicas.

- Release: En esta rama se guardaran las versiones "estables" de nuestro repositorio, subidas desde develop cuando las Features esten listas.

- Develop: Esta rama es como un "puzzle" se iran subiendo Features acabadas o en versiones que son estables, cuando tenga suficientes caracteristicas para ser una version como por ejemplo "1.1" se pasara a release.

- Feature: En esta rama trabajaremos una sola caracteristica del repositorio, la cual cuando este lista se subira a la rama Develop, para poder hacer todo el procedimiento de produccion y sacar una nueva Release.


Ejemplo Grafico

![GraphicExample](media/ejemplo%20grafico%20branches.svg)