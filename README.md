INTEGRANTES:
David Felipe Velasquez Contreras (Collaborator)
Santiago Diaz Rojas (Owner)

PASO A PASO:

Parte 1:

Creacion de repositorio localmete

![alt text](image.png) 

Comando git add y git commit para tener los ultimos cambios generados localmente y subirlos al repositorio remoto
![alt text](image-1.png)

Conexxion con el repositorio remoto, y subida de los cambios al mismo
![alt text](image-2.png)

Configuracion de correo

![alt text](image-3.png)

Subida de cambios nuevos

![alt text](image-4.png)

Parte 2:

Inicio aceptando la solicitud de colaboracion de Santiago
Ahora hicimos un push al mismo tiempo haciendo un cambio previamente en el archivo README, como se puede ver aqui yo gane por lo que es Santiago quien debe resolver los conflictos manualmente:

![alt text](image-6.png)
A David (Collaborator) le dejo subir los cambios de primero por lo tanto me toca hacer un pull para bajar los cambios realizados y solucionar los conflictos que hay entre versiones
![alt text](image-7.png)

el archivo se visualiza con los simbolos <<< === >>> como se muestra a contuniacion, se procede a arreglalos manualmente
![alt text](image-5.png)

Luego de que se hayan resuelto los conflictos manualmente volvemos a hacer push al mismo tiempo para esta ves utilizar visual studio code.
Se vuelve hacer el mismo proceso para ahora solucionarlos con el editor
![alt text](image-8.png)

de nuevo David(Collaborator) gana y me toca hacer la correccion ahora usando el editor
![alt text](image-9.png)

Al hacer el pull nos salen los mismo simbolos <<< === >>>, como se muestra a contuniacion, se procede a arreglalos desde Visual Studio Code
![alt text](image-10.png)
![alt text](image-11.png)

Parte 3:
Ya David habiendo realizado este fork, va a clonarlo en el computador, para hacer cambios y posteriormente hacer un pull request.

Primero va a crear la nueva rama dentro de este:

![alt text](imageD-12.png)

Ahora dentro de esta rama hago un add, commit y push para que de esta manera los cambios queden guardados en el fork:

![alt text](imageD-13.png)

Ya los cambios se ven reflejados en github, por lo tanto voy a proceder a hacer el pull request, con esto Santiago debera decidir si aceptar o no los cambios propuestos desde el fork:

![alt text](imageD-14.png)
![alt text](imageD-15.png)

Esto es lo que se ve al aceptar el pull request

![alt text](imageD-16.png)

Se procede hacer la creacion de la rama "features/santiago" para poder hacer un pull request de mis cambios con los de David
![alt text](image-12.png)


RESPUESTAS: 
--Santiago Diaz Rojas

Parte 1:
git add
¿Para que sirve?
El comando git add añade una modificación presente en el directorio de trabajo al area de preparacion. Es la forma de decirle a Git qué cambios particulares se realizarán en la próxima confirmación.

¿Como se usa?
Se utiliza ejecutando el comando "git add . (para subir todos los cambios encontardos dentro del directorio de trbabajo o se puede utilizar comandos internos de git si se requiere, para subir cambios de un directiorio de en especifico, particular, etc.)"

git commit
¿Para que sirve?
El comando git commit captura una instancia que se esta realizando en los archivos que se agregaron con el comando git add

¿Como se usa?
Se utiliza ejecutando el comando "git commit -m (este ultimo para dejar un mensaje de los cambios realizados o se puede utilizar otros comandos internos de git si se requieren)"

Parte 2: 
¿Que sucedio?
Como se inteta hacer una modificacion del repositorio remoto en donde la version del repositorio local no es la misma, este bloquea el push, con el fin de no permitir la 
la modificacion de una version correcta dentro del repositorio remoto. Por eso nos toca actualizar el repositorio local con un pull y solucionar los problemas de los archivos ya sea manualmente o con ayuda de algun IDE.

Parte 3:

¿Hay una mejor forma de trabajar con Git para no tener conflictos?
Sí, hay varias maneras de trabajar con Git para minimizar los conflictos, especialmente cuando varias personas trabajan en la misma rama, como master.

Crear una rama de trabajo: En lugar de trabajar directamente en la rama master, siempre crear una propia rama. Esto aísla cambios y evita que interfieran con los de otros hasta que estés listo para integrarlos.

Hacer pulls frecuentemente: Antes de empezar a trabajar, hay que asegurarce de hacer un pull de la última versión de master para que la rama esté actualizada. Esto reduce la probabilidad de conflictos más adelante.

¿Qué es y como funciona el Pull Request?
Un Pull Request (PR) es una herramienta que permite proponer cambios en la rama master de un proyecto, pero de una manera que otros puedan revisar antes de integrarlos. 
para que funcione corectamente se debe hacer los siguientes pasos:

1. Crea una rama

2. Trabaja en la rama

3. Actualiza tu rama

4. Envía un PR

6. Resuelve conflictos(Si Git detecta conflictos al intentar fusionar el PR, habra que resolverlos manualmente. El proceso es sencillo: Git indicará los archivos en conflicto, y se determina cómo combinar los cambios.)

7. Merge en master: Una vez que el PR sea aprobado y los conflictos se hayan resuelto, los cambios se pueden fusionar en master, manteniendo el código estable y sin conflictos.


-- David Velasquez

Parte 1:

3. Git add sirve para decirle a git que archivos queremos incluir en el seguimiento de git sobre el proyecto actual, si se hace git add . se toman todos los archivos actuales pero tambien se puede solo incluir el nombre de un archivo o una carpeta para solo tomar estos en cuenta.

Git commit con el mensaje nos ayuda a guardar los cambios localmente "como tomarle una foto" al codigo en el momento que se hace, con un mensaje para referenciar los cambios hechos, usualmente utilizando una fecha

Parte 2:

¿Que sucedio?

Desde mi punto de vista se realizaron los cambios correctamente, sin embargo para Santiago no fue asi por lo que debemos resolver los conflictos.

Ahora hicimos un push al mismo tiempo haciendo un cambio previamente en el archivo README, como se puede ver yo gane por lo que es Santiago quien debe resolver los conflictos manualmente, esto es especialmente util en equipos grandes ya que no permite la superposicion de elementos que luego pueden dar muchos problemas

Parte 3:

1. Encontramos que una mejor manera de trabajar esto es realizando un fork ya que asi se trabaja una copia del proyecto, esto en proyectos grandes ayuda mucho ya que no se corre peligro de hacer cambios importantes, y cualquiera de estos es posteriormente revisado en un pull request.

2. Un pull request es una solicitud al repositorio original para que se tomen en cuenta los cambios realizados en una copia del proyecto o en una rama alternativa, con ello el administrador decide que cambios se realizan y que cambios no.

