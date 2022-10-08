# WORK to GitFlow

Para trabajar con el metodo GitFlow tendremos las siguientes ramas:
- Master: En esta rama estara una version estable de nuestro repositorio.

- HotFix: En esta rama arreglaremos errores que pueden surgir de la rama Master, sin pasar por el proceso de produccion o develop, para no entorpecer con las nuevas caracteristicas.

- Release: En esta rama se guardaran las versiones "estables" de nuestro repositorio, subidas desde develop cuando las Features esten listas.

- Develop: Esta rama es como un "puzzle" se iran subiendo Features acabadas o en versiones que son estables, cuando tenga suficientes caracteristicas para ser una version como por ejemplo "1.1" se pasara a release.

- Feature: En esta rama trabajaremos una sola caracteristica del repositorio, la cual cuando este lista se subira a la rama Develop, para poder hacer todo el procedimiento de produccion y sacar una nueva Release.


Ejemplo Grafico

![GraphicExample](media/ejemplo%20grafico%20branches.svg)


### Comandos para subir de una rama a otra
##### (ej: Feature -> develop)

- Lo primero que debemos tener en cuenta es tener nuestra rama actual con un commit hecho de lo que queremos subir

- Una vez hecho esto cojeremos la version mas actual de develop -> ```$ git pull origin develop```
    - En caso que esto nos de error o diga que no es la misma version -> ```$ git rebase```
    - Ahora desde nuestro editor de codigo arreglaremos los errores entre versiones que nos salgan.
    - Añadiremos los cambios al branch pero **IMPORTANTE NO HACER UN COMMIT SOLO EL ADD** -> ```$ git add -A```
    - Finalmente seguiremos con el git rebase -> ```$ git rebase --continue```

- Como llegados a este punto, o nuestro repositorio estaba al dia o no nos ha dado errores haremos los siguientes pasos
    - Cambiaremos a la rama develop -> ```$ git checkout develop```
    - Haremos un merge con nuestra rama feature que hemos preparado anteriormente -> ```$ git merge --no-f <feature>```
    - Y finalmente subiremos los cambios de la rama "Develop" -> ```$ git push origin develop```