# **Metodología de la Práctica Final**

## **Crear el repositorio**

Para realizar la práctica final debíamos agrupar todos los trabajos realizados a lo largo del curso en un mismo repositorio. Este nuevo repositorio tenía que estar dentro de la organización de Github Pontedatos, a la que fuimos añadida por el profesor. En ella tuve que crear el repositorio Magdalenadelabarrera a través de la pestaña “New repository” en la que puse mi nombre. En la pestaña “owner” seleccioné “Pontedatos” (pues es el profesor el “dueño” del repositorio, y debe darnos permiso para acceder a él).

Una vez creado mi repositorio, los siguientes pasos los llevé a cabo no desde Github, sino a través de la terminal de mi ordenador. Ahí debía conectar mi repositorio de Pontedatos con la terminal; es decir, copiar el repositorio Git en mi directorio local, a través de la función `git.clone`, añadiendo a continuación la URL del código de mi repositorio Git. Para comprobar que está acción se había realizado de manera correcta lo hice con el comando `ls -a`, que permite ver que se había clonado el Git creando un nuevo directorio local para el repositorio.

Para copiar el contenido del directorio con todas mis prácticas utilizo el comando `cp` –que tiene la estructura: cp [opciones] [origen] [destino]. En “opciones” puse el nombre de todos los archivos, el origen la carpeta en la que los tenía y en destino puse la nueva carpeta Magdalenadelabarrera. De nuevo, para comprobar que los archivos se habían copiado correctamente utilicé el comando de listar archivos dentro de este directorio, `ls -a`.

Ya con todos los archivos subidos en la carpeta Magdalenadelabarrera, me dispuse a subirlos a mi repositorio en Pontedatos. Aunque previamente había realizado con la nueva url el comando `git clone`, para comprobar que el repositorio remoto es correcto ejecuté el comando` git remote -v`, que me mostraba la url de donde lo extraigo (fetch) y donde lo vuelca (push). 

## **Subir los archivos a GitHub**

El siguiente paso consistía en subir todos los archivos desde la terminal a mi repositorio de Github. Para ello llevé a cabo los siguientes pasos:

- Ejecutar el comando `git status` que nos muestra el estado del directorio y nos permite ver los cambios realizados.
- Ejecutar el comando `git add .` con la que se añaden los archivos
- Ejecutar el comando `git commit .` con el que se “comitean” (llevan a cabo) los cambios
- Ejecutar el comando `git push` con el que se carga el contenido del repositorio local al remoto, en este caso el de Github.
- En mi caso, me daba error, pues decía que no había sido posible subir algunas “refs” (Git References) al repositorio remoto. La opción `git pull` –que permite actualizar los contenidos de los repositorios y generalmente me es útil como paso previo al `git push`– en esta ocasión no me servía. Por tanto, para solventar el problema ejecuté el comando `git push -f’
*Aclaración: `git push -f`es la abreviatura de `git push --force`. Este comando sirve para forzar un push cuando de otro modo git rechazaría tu `git push` porque has cambiado el historial de tu repositorio en tu repositorio de empuje* (Fuente: [Stack Overflow](https://stackoverflow.com/questions/44678942/difference-between-git-push-and-git-push-f))
- Para ver que los pasos se han realizado correctamente o conocer el estado del git volvemos a usar el comando `git status`.

## **README.md**

Una vez con todos los archivos de las prácticas previas dentro de la carpeta, he procedido a editar el "README.md" que explica todos los archivos que guarda este repositorio. Lo he realizado a través de nano, el editor de texto de la terminal. También a través de nano he creado los archivos "metodología.md" y "resumen.md" en los que se explica la metodología empleada para realizar esta práctica y lo aprendido durante el curso. 

## **Creación de una página web a través de Github**

Para crear una página web a través de Github se utiliza la funcionalidad "Pages", con la que se puede crear una web con el contenido de nuestro repositorio. 

Para activar esta opción de "Pages", debemos hacerlo a través de la siguiente url:  https://github.com/Pontedatos/nombre-repositorio/settings/pages. 

Elegimos que la fuente en la rama "main" en la carpeta "/root". Asimismo, como GitHub emplea como index.html el archivo README.md, al acceder a la dirección web lo que visualizamos es el contenido del README. 

