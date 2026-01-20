Curso GIT and GITHub

Que es GIT?

        Es un Sistema de Control de Versiones. (scv). GIT.

        Nos ayuda a trabajar de forma colaborativa con otros programadores.

        Ej. el lunes escribes codigo, el dia martes modificas el codigo, y con git vas a
        poder comparar el codigo del dia LUNES con el codigo del dia MARTES.

        IMPORTANTE = Git solo sube las diferencias.

        ~Registra los cambios realizados en archivos a lo largo del tiempo.
        ~Recupera versiones especificas.
            ~Regresar a versiones anteriores de tus archivos.
            ~Regresar a versiones anteriores del proyecto completo
            ~Comparar los cambios a lo largo del tiempo.
            ~ver quien modifico un archivo en un momento especifico.
            ~Recuperar archivos perdidos o arruinados.

Como funciona GIT?

        Git maneja sus datos como un conjunto de copias, o fotos instantaneas.

        Version 1(Lunes) = File A , File B, File C
        Version 2(Martes) = A1, B, C1
        Version 3(Miercoles) = A1, B, C2
        Version 4(Jueves) = A2, B1, C2
        Version 5(Viernes) = A2, B2, C3

        Git cada vez que confirmas un cambio, guarda el estado de tu proyecto y basicamente
        le toma una foto. 

        Cada version es un dia de la semana, el lunes comenzamos con 3 archivos, A,B,C, Git
        le toma foto a cada archivo para guardarlo.

        El martes podemos notar que el Archivo A fue modificado, junto con el archivo C,
        dando como resultado Martes = A1, B, C1 (entendiendo que el 1 despues de la letra
        es el sinonimo de archivo modificado), Git toma una nueva foto solo de archivo A y 
        archivo C . Solo hace una referencia del archivo B. (Solo archivos modificados
        van a copiarse en la version del dia 2 martes).
        
        En resumen Git hace una foto instantanea al momento de que estes escribiendo el codigo
        y de esta manera, vas a poder tener un historial con todas las versiones de tu codigo
        y acceso a cada una.

Ventajas de utilizar Git.

        ~Operaciones Locales = Es que git solo necesitas tus archivos y recursos locales para funcionar. Lee la historia del proyecto, casi instantaneamente.
        
        ~No Internet = No necesita conectarse a la red o conectarse a otra computadora. 
        
        ~NO Borra = Solo anade informacion a la base de datos de Git
        
        ~Integridad = Es muy dificil que vayamos a perder las copias instantaneas que git realiza de forma automatizada cuando codeamos.

        En git, todo siempre esta verificado con el HASH: SHA-1: 24b9da6552252987aa493b52f8696cd6d3b00373

        Esto realmente es una cadena de 40 caracteres hexadecimal, de 0 a 9 y de A hasta F. Estos codigos son unicos, y se calcula con base a los contenidos del archivo que estas tratando de modificar o la estructura del directorio de Git.

        Sirve para evitar que se puedan carmbiar los archivos o directorios sin que git lo sepa.


Los 3 Estados de Git.

        en git tenemos 3 areas:

            Working Dyrectory = Directorio de trabajo = MODIFIED
                (es donde se va a crear el codigo y donde se va a trabajar)

                   ~ git add ~: pasamos de Modified a Staged

            Staging Area = El area de preparacion = STAGED
                (es un archivo contenido en tu directorio de git, funciona como una lista o indice, indicando que archivos van a ir para el commit)

                  ~ git commit ~: pasamos de Staged a Committed

            Local Repository = El repositorio local o directorio de git = COMMITED
                (es donde se almacenan los metadatos y la base de datos para tus proyectos)

        Importante aprender los nombres en ingles, estos tres estados ocurren de forma local en nuestra computadora.

COMANDOS =
        git status: con este comando podemos saber cual es el estado de nuestro archivo.

        git commit -m "comentario al respecto del commit": sirve para dar finalizado la modificacion de los archivos y cargarlos al repositorio Local.

        git log: te muestra las modificaciones que se realizaron a lo ultimo, con la informacion de el usuario que realizo las modificaciones.

        git add . = envia todas las modificaciones que realizaste al staging area, no agrega los eliminados ni los que tienen seguimiento.

        git add NOMBREARCHIVO.EXTENSION = ahi solo agrega el archivo que seleccionamos al staging area.

        git push = para que otros programadores puedan ver el archivo, mas adelante lo vemos en profundidad.

        pull request = pedir solicitud para modificar algo
        
        
        

