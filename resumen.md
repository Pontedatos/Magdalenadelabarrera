# Resumen de lo aprendido en el curso

## **A continuación incluyo las nociones elementales adquiridas a lo largo del cuatrimestre en la asignatura de Periodismo de Datos, siguiendo el esquema/índice proporcionado por el profesor en Aula Global**

> Nota: mi aprendizaje en esta asignatura ha variado con respecto al del resto de mis compañeras debido a que estoy trabajando desde un portátil de Apple. No obstante, he buscado adaptar la explicación del proceso de aprendizaje al uso de un Mac.

## **Instalación de un programa de emulación de la terminal**

Mis compañeras tuvieron tuvieron que descargarse Cygwin y/o Ubuntu. En el caso de Mac, la terminal está presente por defecto, de modo que no hace falta instalar un programa de emulación de la terminal –que simula el funcionamiento de una terminal de ordenador. 

Los pasos s seguir en mi caso fueron la descarga y activación de XCode. Sin embargo, antes de descargarlo, actualicé en sistema operativo de mi portátil. Después ejecuté el comando `xcode-select –install` en la terminal. 

## **Configuración del programa**

Dado que haríamos un uso recurrente de la Terminal, el profesor nos introdujo en el lenguaje propio y nos presentó algunas operaciones que facilitarían y agilizarían el trabajo en la Terminal. De nuevo, al ser usuaria de Mac no tuve que llevar a cabo alguna de las configuraciones que sí realizaron las otras compañeras.

Por ejemplo, un paso importante en la configuración del programa consiste en establecer el alias, que nos conduce directamente a la carpeta sin necesidad de rastrear todo el árbol de directorios. De este modo te puedes “ahorrarte” el `cd`. Sin embargo, yo no lo necesité, porque solo se estableció para las usuarias de Windows.

### Algunas nociones básicas de la terminal

- `whoami`:  imprime el nombre del usuario actual en el momento en que se invoca
- `pwd`: devuelve la ruta en la que estamos situados

*Otro instrumento que puede ser muy útil a la hora de empelar la Terminal es la tecla tabuladora*

### Github

La intención era vincular el repositorio creado online en Github con una carpeta de mi ordenador a través de la terminal. 

En primer lugar, una vez dentro de la carpeta seleccionada (a la que vamos usando el comando `cd`), copiamos el enlace de nuestro repositorio (botón verde ‘Code’), y copiamos el enlace https que nos muestra. 

Volvemos a la terminal, y escribimos `git clone "enlacerepositorio"`. En mi caso, `git clone https://github.com/magdibmassieu/practicas-periodismo-datos` 

Antes de nada, tenemos que configurar nuestro usuario de GitHub en la terminal para vincular los cambios. Para ello, tenemos que escribir `git config --global user.name nuestrousuario`, y luego `git config --global user.email correogithub`. En mi caso: `git config --global user.name magdibmassieu` y `git config --global user.email 10038175@alumnos.uc3m.es`, con el correo de la universidad.

Una vez terminado el proceso de configuración, ya podemos empezar a trabajar desde la terminal empleando una serie de comandos propios de git. 

- `git status`: muestra el estado del directorio de trabajo y permite ver los cambios realizados (por ejemplo al hacer un cambio a través de `nano README.md`), los que no, y los archivos en los que Git no va a realizar el seguimiento
- `git add nombre-archivo` o `git add .`para añadir un archivo
- `git commit -m “mensaje del commit”` o `git commit .` para “commitear”, o lo que es igual, hacer un cambio; registrar el cambio, con el que puedes reflejar y explicar las modificaciones. 
- `git push` para que se suba a nuestro repositorio de GitHub. En este punto a veces nos es útil hacer previamente `git pull`, empleado para extraer y descargar contenido desde un repositorio remoto

*Nos pedirá nuestro usuario y contraseña, pero esta contraseña no es con la que accedemos sino un token, que podemos sacar de los ajustes de GitHub > Developer settings > Personal access token*


## Configuración de un programa de edición de texto

El programa de edición de texto que he instalado es nano. Para ello, reiterándome en que trabajo con Mac, lo hago ejecutando en la terminal `brew install nano`

*A continuación se explicará qué es “brew”, con relación al gestor de paquetes*

### Configuración y funcionamiento de un gestor de paquetes/programas del emulador de la terminal

En el caso de Mac, hemos hecho uso de Homebrew, el gestor o administrador de paquetes más popular para Mac OS X, que simplifica la instalación, actualización y eliminación de programas en los sistemas operativos Mac OS de Apple. 

Para su instalación se copió lo siguiente en la terminal (sacado la página web de Homebrew): 
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`


## Versión del lenguaje de SHELL utilizado

El Shell también se conoce como intérprete de órdenes o intérprete de comandos. De forma predeterminada, el Mac usa zsh o bash como intérprete de la línea de comandos para el Shell. En mi caso, utilicé el dialecto de la Shell zsh (Z shell), que es el shell predeterminado en Mac para todas las cuentas de usuario nuevas, a partir de la versión de macOS Catalina.

Al empezar la asignatura yo tenía como shell bash, pero como el shell predeterminado actualmente para Mac es zsh, desde la terminal se me recomendaba que lo actualizara. Para ello ejecuté `chsh -s /bin/zsh`

Para averiguar qué shell estaba utilizando ejecuté `echo $SHELL`; para saber la versión, `$SHELL –versión`, que da zsh 5.8 (x86_64-apple-darwin21.0)

## Valor de la variable de entorno PATH

PATH es una de las variables de entorno más importantes para ejecutar comandos. Todas las variables empiezan con el símbolo `$`. Para obtener el valor de la variable de entorno PATH ejecuto el comando `echo $PATH`. El resultado que me da es:
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin


## Comandos utilizados y ejemplos.

A lo largo de este documento ya se han ido introduciendo varios comandos –como, por ejemplo, los propios de git–, pero a continuación incluyo algunos de los que no han aparecido, y que hemos ido aprendiendo a lo largo de las clases.
- `echo`: sirve para que la terminal nos devuelva un texto. Por ejemplo, si queremos que la terminal nos diga “Hola mundo” escribimos `echo Hola mundo`.
- `cd`: nos permite acceder a un directorio en específico. Si escribimos solo `cd` vamos al directorio raíz. Con `cd -`nos lleva al último sitio en el que estábamos.
- `cat` para concatenar archivos. Necesita argumentos, hay que explicarle qué queremos que haga
- `ls` lista los archivos o directorios que hay en el espacio de trabajo en el que nos encontramos. Por ejemplo, si ejecuto este comando en mi carpeta se imprimirían en pantalla todos los archivos relativos a las prácticas de la asignatura de Periodismo de Datos
- `-l` similar al anterior, pero con información más extendida
- `cp`, seguido de origen y del destino, para copiar
- `mv` para mover o renombrar
- `man` seguido de un comando cualquier sirve para abrir el manual de dicho comando; es decir, explica en qué consiste y cómo funciona. Por ejemplo, `man ls` nos muestra todas las opciones disponibles para el comando `ls`. 
- `>` envía la salida del comando que le precede a donde nosotros le indiquemos
- `>>` lo envía al final, si existe; y si no existe, lo crea
- `env` para ver todas las variables de entorno
- `mkdir` para crear un repositorio. Por ejemplo, si quisiéramos crear una carpeta en la que almacenar todos los repositorios de GitHub, haríamos `mkdir github`. Si queremos crear el directorio y entrar en la carpeta de una vez, ponemos las órdenes seguidas pero separadas por `&&` (que permite ejecutar dos comandos en una misma línea). En este caso: `mkdir github && cd github`.
- `wget [enlace]` para descargarnos un archivo/contenido de una web. Nos es útil también para adjuntar imágenes (escribes `wget’ y a continuación añades el link de la imagen y la renombras con mv)

