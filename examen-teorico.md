# **Examen Final Periodismo de Datos: María Magdalena de la Barrera**

# Primera parte: preguntas cortas

## **Preguntas comunes a ambos bloques**

### **1. ¿Quién es Philip Meyer?**

Philip Meyer es un periodista, profesor y escritor estadounidense, cuyas ideas –basadas en la intención de **“convertir el periodismo en una ciencia”**– han cambiado la manera en que se ejerce el periodismo, sobre todo a partir de los 60 y llegando hasta la actualidad. 

Meyer fue designado para la cobertura de los disturbios de Detroit en 1967, como parte de la plantilla del Detroit Free Press. Para ofrecer un relato detallado, **Meyer propuso una investigación científica para identificar las causas de las revueltas, en la que hizo uso del ordenador para las pruebas estadísticas de la muestra**, demostrando que las tesis asumidas por la prensa del momento sobre las razones de disturbios raciales eran falsas.

Este trabajo fue decisivo para la profesión periodística, **sentando las bases del “periodismo de precisión”** (así tituló su obra publicada en 1973, que supone el primer tratado sobre la nueva forma de hacer información). También le sirvió para que, en 1968, el personal del Detroit Free Press ganara el Premio Pulitzer de Reportaje Local General. 


### **2. ¿Quién fue Florence Nightingale?**

**Florence Nightingale (1820-1910) fue una enfermera inglesa, pionera de la enfermería profesional moderna y creadora del primer modelo conceptual de enfermería**. Tras la Guerra de Crimea, trabajando en los hospitales se dio cuenta de que las altas tasas de mortalidad de los soldados se debían sobre todo a las malas condiciones sanitarias de los hospitales. Nightingale recabó información y reunió estadísticas sobre mortalidad, introduciendo a su labor la estadística: hacía gráficas, formularios sobre las causas de enfermedad y de muerte... 

**Nightingale fue completamente innovadora en la recolección, interpretación y presentación gráfica de las estadísticas descriptivas**. Buscaba facilitar la comprensión de los datos a quienes pudieran tener dificultades con los informes estadísticos tradicionales. **Creó el *Diagrama de la Rosa* que, desde el punto de vista estadístico, fue muy novedoso para la época**. En este diagrama se representan tres variables –el tiempo (cada sector es un mes), el número de muertes (el área del sector) y la causa de la muerte (color)– en un momento en que los gráficos más habituales representaban solo una o dos variables.


## **Preguntas Bloque B**

### **1. ¿Cuál fue el comienzo del CAR (Computer Assisted Reporting)?**

Las siglas *CAR* se refieren al concepto de **periodismo asistido por ordenador** y describen el uso de ordenadores para recopilar y analizar datos necesarios para la redacción de noticias, y está **estrechamente ligado al “periodismo de precisión"**.

Comenzó en los años 50, cuando la cadena de televisión estadounidense CBS utilizó un ordenador UNIVAC I (*UNIVersal Automatic Computer I*) para analizar los resultados de las elecciones presidenciales del país. 

Una de las primeras aplicaciones fue la de Philip Meyer tras los disturbios en Detroit (utilizó un ordenador central para demostrar que las personas que habían asistido a la universidad tenían la misma probabilidad de haberse alzado que las que habían abandonado la escuela secundaria). Años más tarde, en su libro *Precision Journalism*, Meyer sostiene que un buen periodista debe utilizar bases de datos y encuestas, ambas asistidas por ordenador. 


### **2. ¿Qué es nano?**

`nano` es un programa de edición de textos (o editor de textos). Permite escribir desde la terminal empleando el lenguaje Markdown y crear archivos `.md`, entre otros. 


### **3. ¿Cuál es la estructura de las sentencias/instrucciones en la línea de comandos?**

Existen varias estructuras posibles, dependiendo de lo que busquemos hacer. 
En algunos casos, se pone exclusivamente el comando, es decir, solo se ejecuta una orden en la terminal (por ejemplo `ls`, que muestra un listado). En otros, los comandos se siguen de opciones que lo modifican o añaden funciones, que vienen a menudo precedidas por un guion (ejemplo: `ls -a`, que lista archivos y directorios ocultos; o `ls -la`, que hace la función anterior, pero con detalle). También se pueden añadir argumentos que indican sobre qué archivos o directorios queremos que se aplique la orden (por ejemplo, `ls practicas-periodismo-datos`, que listará los archivos estén dentro de esta carpeta).


### **4. ¿Cuál es la versión de Shell qué utilizas?**

La `Shell` tiene varios dialectos posibles. El más común es `bash`, pero, en mi caso, utilizo la versión `zsh`, que es la versión de shell predeterminada actualmente para Mac.
Se puede comprobar qué shell utilizas usando el comando `echo $SHELL`. Al ponerlo me sale: `/bin/zsh`, por lo tanto introduzco otro comando para que me de la versión que tengo en mi ordenador: `$SHELL --version`

### **5. ¿Cómo verías las variables de entorno de tu shell "PATH"? Escribe su valor también.**

Utilizo el comando `env`, que sirve para visualizar en pantalla todas las variables de entorno. También podemos utilizar el comando `env | less`, para ver menos, porque son demasiadas variables y a menudo no caben en la pantalla. 

__CFBundleIdentifier=com.apple.Terminal
TMPDIR=/var/folders/tg/945dj5pd4r9769ghzpgm48f00000gn/T/
XPC_FLAGS=0x0
LaunchInstanceID=A281362F-32CD-47D7-8E43-D3D5424E3853
TERM=xterm-256color
SSH_AUTH_SOCK=/private/tmp/com.apple.launchd.BJzqtNQ3Rk/Listeners
SECURITYSESSIONID=186b2
XPC_SERVICE_NAME=0
TERM_PROGRAM=Apple_Terminal
TERM_PROGRAM_VERSION=443
TERM_SESSION_ID=3AFDFA2B-6B46-4603-8A99-AFAE5A4B31C1
SHELL=/bin/zsh
HOME=/Users/magdalenadelabm
LOGNAME=magdalenadelabm
USER=magdalenadelabm
PATH=/opt/homebrew/bin:/opt/homebrew/sbin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
SHLVL=1
PWD=/Users/magdalenadelabm
OLDPWD=/Users/magdalenadelabm
HOMEBREW_PREFIX=/opt/homebrew
HOMEBREW_CELLAR=/opt/homebrew/Cellar
HOMEBREW_REPOSITORY=/opt/homebrew
MANPATH=/opt/homebrew/share/man::
INFOPATH=/opt/homebrew/share/info:
LANG=es_ES.UTF-8
_=/usr/bin/env

### **6. Cuál es el primer comando que deberías usar en la terminal. Explica tu respuesta.**

Antes de empezar a trazar la ruta hacia el fichero con el que deseamos trabajar, primero debemos usar el comando `pwd`, que viene del inglés *print work directory* (imprimir directorio de trabajo). Sirve para que la terminal nos diga en qué parte del árbol de directorios nos encontramos; de qué directorio partimos. 


### **7. ¿Qué se puede hacer para ver el contenido de un archivo de texto?**
Habría que introducir el comando `TYPE`, que sirve para visualizar el contenido de archivos de texto planos (como los .md). Esto nos permitirá ver el contenido del archivo de texto, pero no editarlo (para lo que tendríamos que recurrir a un editor de texto como nano, por ejemplo). 


# **Segunda parte: pregunta de desarrollo**

## **Qué es el periodismo de datos. Cómo se relaciona con la visualización de datos.**

**El periodismo de datos es el resultado de la propia evolución de la sociedad de la información** –en la que vivimos desde la década de los 60’ y en la que comienzan a darse las primeras manifestaciones del uso de esta nueva manera de hacer periodismo. Su antecedente directo está en el periodismo de precisión, que se define como el uso de métodos de análisis de las ciencias sociales unido al software estadístico y ordenadores, con el fin de construir una historia periodística. En resumen, **se trata de un compendio de elementos fundamentales: periodismo, investigación, datos, aplicaciones informáticas y visualización.**

No obstante, **el periodismo de datos moderno, del que nos nutrimos en la actualidad, nace ya en el siglo XXI** (entre 2006-200), como resultado de una combinación de factores (entre los que están la abundancia de software de código abierto, HTML5 y Open Data). En un contexto en que la industria predominante es la del conocimiento, en la que disponemos de acceso a cantidades ingentes de datos, **el *periodismo guiado por datos* los incorpora como una parte más del trabajo periodístico, sin por ello menospreciar la parte periodística de la profesión**. De hecho, Philip Meyer, en su libro *Precision Journalism* (1973), sostiene que un periodista debe utilizar bases de datos y encuestas, ambas asistidas por ordenador. 

Esta definición está más en sintonía con el término *computer-assisted reporter* (reportero asistido por ordenador). En la edición de 2002, Meyer va un paso más allá y afirma:

> "Un periodista tiene que ser un gestor de bases de datos"

De estas palabras deducimos que, en un mismo profesional, deben implicarse distintos saberes o capacidades: competencias informáticas, desarrollo de aplicaciones de noticias y conocimientos en visualización de datos. 

No obstante, además de la gestión de los datos como tal (también los datos en abierto), una parte fundamental es la inclusión de la visualización de datos, para facilitar la comprensión de estos. Sin embargo, este elemento no solo debe entenderse como un producto final; **en la etapa de visualización, el periodista también realiza análisis, aplica técnicas estadísticas y programas informáticos**. De este modo, el periodista de datos –*data journalist*, término más utilizado actualmente– consigue que, de un gran volumen de datos, pueda sacar hipótesis o conclusiones a lo largo del proceso. Estos se materializarían posteriormente en una historia, que llegaría finalmente al público.

