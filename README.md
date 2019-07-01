# Interconectar-Choreographe-y-Webots (En windows)

Este repositorio tiene como objetivo realizar la conexión virtual entre el software choreographe y Webots con la finalidad de poder simular trayectorias y movimientos con el robot Nao.

# Introducción
El simular los movimientos del robot NAO antes de probarlos en el robot real es de suma importancia, ya que así podemos preveer eventos que podráin dañar al robot real. Uno de los mas importantes y competos entornos de simulación para robots es Webots, el cual nos permite simular una amplia gama de robots. Estas simulaciones pueden programarse en C, Python, Java o como en este proyecto que se programo el comportamiento del Robot NAO con la ayuda del software Choreographe.

# Instalación
En primer lugar se debe descargar e instalar los programas Webots y choreographe.
En el caso del programa Choreographe, se descarga en el link: https://www.robotlab.com/choregraphe-download .En ese sitio deberan poner algunos datos para que les muestre los botones de descarga y un código de activación.

Para descargar Webots, se tiene la siguiente página: https://cyberbotics.com/download

# Descarga de archivos necesarios
Los archivos que necesitamos para que el programa Webots pueda conectarse a Choreographe se pueden descargar de la siguiente liga:

http://www.mediafire.com/file/qgj10ju5b9s5ab4/aldebaran.rar/file

Una vez que se haya descomprimido la carpeta, la copiamos a la ruta: C:\Program Files\Webots\projects\robots

# Instalación de Visual Studio 
 Para poder compilar algunos archivos será necesario instalar Microsoft Visual Studio C++ 2010 Express, la cual es una terminal.
 
# Instalación de terminal MSYS2
Para poder compilar otros archivos archivos será necesario instalar MSYS2, la cual es una plataforma de desarrollo y distribución de software para Windows. Este programa se puede descargar de: https://www.msys2.org/ En esta página vienen todas las instrucciones para instalarlo y actualizarlo. Nota: Es importante actualizarlo.

# Construcción del proyecto

Además se actualizar MSYS2 se deben instalar algunas aplicaciones desde esa termianl. Así que para realizar esto se debe teclear:
pacman -S make

Cuando termine de instalar make, instalamos unzip, con el comando:
pacman -S unzip

Despues tecleamos:
pacman -S gcc

A continuación accederemos ala ruta: c/Archivos de programa/Webots/projects/robots/aldebaran/controllers/naoqisim mediante la terminal que acabamos de instalar. Para esto debemos teclear:
$ cd c:

$ cd Archivos\ de\ programa

$ cd Webots/

$ cd projects/

$ cd robots/

$ cd aldebaran/

$ cd controllers/

$ cd naoqisim

Estando en esa ruta tecleamos:
make
(Si apareciera la alerta: make: *** [Makefile:19: release] Error 1, solo se debe ingnorar)

Despues nos regresamos a la carpeta "aldebaran", esto tecleando:
cd ..
cd ..

Estando en esa carpeta volvemos a teclear:
make
(Si apareciera algún error volver a teclear: make)

Despues de esto volvemos ala carpeta "naoquisim" con los comandos:
$ cd controllers/

$ cd naoqisim

Y finalmente teclemaos el comando: 
make


Hecho eso se compila el programa y está listo para Probar.

# Prueba de la conexión entre Webots y Choreographe

Para realizar la conexión se realizó un video en youtube el cual esta en el sigiente link:

https://youtu.be/9J6-B0g9f1A




