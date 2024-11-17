# **Mis apuntes de 0373 - ASIX1**

1. [GITHUB](#1.GITHUB "Enlace a los apuntes de GitHub")
2. [MARKDOWN](#2.MARKDOWN "Enlace a los apuntes de MarkDown")
3. [HTML](#3.HTML "Enlace a los apuntes de HTML")

# 1. GITHUB

## 1.1 ¿Que es GitHub?
GitHub se define como una plataforma que se utiliza para el control de versiones y que permite la colaboración en proyectos software, es decir, se puede almacenar, compartir y trabajar junto a otros usuarios para escribir código. Esta plataforma nos ayudará a llevar un historial de modificaciones/cambios que se hayan realizado en un proyecto de manera ordenada.

## 1.2 Características de GitHub
1. Permite trabajar de forma colaborativa
2. Permite realizar un seguimiento de los diferentes cambios realizados en el código con Git.
3. Ofrece un almacenamiento organizado de código gracias a los repositorios.
4. Ofrece soporte para diferentes páginas de documentación.
5. La comunidad ofrece soporte para proyectos de código abierto y también hay foros de discusión.

## 1.3 Creación de una cuenta en GitHub
Para crear una cuenta en GitHub y comenzar a trabajar debemos seguir los siguientes pasos:
1. Visitar la página web de GitHub.
2. Registrarse y crear una nueva cuenta.
3. Introducir un nombre de usuario junto a un correo electrónico y una contraseña segura.
4. Completar el proceso de verificación y la configuración inicial de la cuenta.
Una vez tengamos nuestra cuenta en GitHub, podremos crear un repositorio en el que trabajar.

## 1.4 Repositorios: Funcionamiento

### 1.4.1. Creación de un repositorio
Dentro de GithHub con nuestra sesión iniciada:
1. Hacemos click en la opción "Nuevo" en la pagina principal para crear un repositorio. También le podemos dar a la opción "Crear repositorio" si nos aparece.
2. Introducimos el nombre de nuestro repositorio.
3. Podemos agregar una descripción, escoger si mostrar el repositorio como público o privado e incluso añadir un archivo README una vez inicialicemos por primera vez el repositorio, entre algunas otras opciones más.
   
### 1.4.2. Clonación de un repositorio
1. Copiamos la URL de nuestro repositorio en GitHub.
2. En la terminal (CMD), dentro de nuestra carpeta local de repositorios, escribiremos el siguiente comando: ``git clone "URL del Repositorio"``. Este creará una carpeta local sincronizada al repositorio del cual hemos copiado la URL en GitHub. Con esto, podremos trabajar de manera local para, posteriormente, transferir todo el trabajo al repositorio de GitHub.

## 1.5 Comandos para GitHub
Estos son algunos de los comandos a utilizar en el terminal para tranferir archivos entre nuestra carpeta local y el repositorio de GitHub:
 - ``git init`` --> Inicializa un repositorio de GitHub en la carpeta local.
 - ``git branch -M "rama"`` --> Permite cambiar a otras ramas (ej: git branch -M main).
 - ``git branch`` --> Muestra la rama en la que se está trabajando.
 - ``git add "archivo.txt"`` --> Agrega los archivos al area intermedia antes de hacer el commit y el push. Podemos escribir el nombre de los archivos que queremos agregar o usar "." para añadir todos los archivos de la carpeta local en la que estamos trabajando.
 - ``git commit -m "Descripción del commit realizado"`` --> Guarda los cambios del area intermedia en el commit para posteriormente subirlo. También da información acerca de las modificaciones realizadas en el commit.
 - ``git push origin main`` --> Envia el commit y sube los archivos a github (desde la rama "main", en la que tenemos nuestra carpeta local, hasta la rama "origin", donde se encuentra el repositorio.)
 - ``git remote add origin "URL del repositorio"`` --> Se usa para clonar un repositorio remoto a nuestra carpeta local.
  


# 2. MARKDOWN

## 2.1 Títulos
Para repartir diferentes apartados podemos aplicar los encabezados. Para crear encabezados, utilizaremos el símbolo "#" antes del texto que queramos utilizar como título. Dependiendo de la cantidad de "#" que se escriban, los niveles del título variaran.

```
# Primer nivel de encabezado
## Segundo nivel de encabezado 
### Tercero nivel de encabezado 
#### Cuarto nivel de encabezado 
##### Quinto nivel de encabezado 
###### Sexto nivel de encabezado 
```

## 2.2 Listas
Para enumerar diferentes apartados o listar diferentes elementos crearemos indices o listas. Para crearlos, deberemos seguir el proceso a realizar en cualquier procesador de texto, colocando el numero o el símbolo y, a continuación, el texto que queramos. Ejemplos:

```
1. Primer punto del indice/lista
    1.1 Primer elemento de la primera sublista
    1.2 Segundo elemento de la primera sublista
2. Segundo punto de la lista
    2.1 Primer elemento de la segunda sublista
    2.2 Segundo elemento de la segunda sublista

* Primer punto de la lista desordenada
- Segundo punto de la lista desordenada
+ Tercer punto de la lista desordenada
```

## 2.3 Texto
Se puede mostrar texto de diferentes formas. Estas ayudan a distinguir las palabras o conceptos clave o para mostrar diferentes tipos de texto.

### 2.3.1 Mostrar código en un repositorio
Para mostrar codigo se debe empezar y finalizar el mismo con el siguiente simbolo escrito tres veces "`" (Es decir, "```"). Un ejemplo podria ser:

```
</body>
</html>
```

### 2.3.2 Negrita y cursiva
Para resaltar palabras en **negrita**, rodearemos una palabra o un conjunto de palabras con un símbolo, ya sea "_" o "*", aplicando uno de los símbolos dos veces, al principio y al final de lo que queremos __destacar__. Un ejemplo:

```
__palabradestacada__

**palabradestacada**
``` 

Para cambiar el tipo de letra a _cursiva_ de cualquier *texto*, debemos rodear este utilizando únicamente uno de los siguientes símbolos al principio y al final del mismo texto. Estos símbolos son "_" y "*", y quedarian de la siguiente manera:

```
_palabracursiva_
*palabracursiva*
```

Es posible poner un texto en ***negrita y cursiva*** si se suman los operadores, es decir, si para cambiar el tipo de letra a cursiva es necesario poner el símbolo una vez y para resaltar las palabras en negrita hace falta poner el símbolo dos veces, para poner el texto de las dos formas habria que ponerlo tres veces en total al inicio y al final, de la siguiente manera:

```
***palabramezcla***
___palabramezcla___
```

## 2.4 Enlaces 
Para aplicar un enlace, se tendrá que seguir el siguiente operador:

```
[TextoAltClicable](URL "Titulo opcional")
```

Donde el "TextoAltClicable" sera un texto alternativo visible y que se podrá clicar para dirigirnos al enlace, y URL el enlace previamente copiado de la dirección a la que queremos ir a traves del texto clicable.

Ej: [Página web Jesuites Bellvitge](https://www.fje.edu/ca/jesuites-bellvitge "Jesuites Bellvitge")

## 2.5 Imágenes
Para colocar una imagen el proceso será similar al de los enlaces, pero el enlace de la imagen tendrá que provenir de nuestro repositorio, es decir, previamente habrá que descargar la imagen a colocar y subirla a nuestro repositorio para asi poder usarla. El operador quedaria de la siguiente manera:

```
![TextoAlt](URL "Titulo Opcional")
```

Un ejemplo de imagen:
![Raphinha](https://github.com/AriamSS/0373_A01_DocumentacionApuntes_SanchezAriam/blob/main/R11.jpg?raw=true "Raphinha")

## 2.6 Tablas
Para comenzar a crear la tabla, debemos empezar por los respectivos títulos de cada columna. Cada columna de la tabla se dividirá por el siguiente símbolo "|", de manera que la primera fila quedará asi:

```
|Titulo 1 | Titulo 2 | Titulo 3|
```

A continuación de los títulos, crearemos una fila en la que se definan los caracteres de una columna, de la siguiente manera:

```
|Titulo 1 | Titulo 2 | Titulo 3|
|----------|:---------------:|------------------:|
```

El símbolo ":" indica la alineacion o posición que tiene el texto en la columna, ya sea a la izquierda, a la derecha o centrado.

Por último, escribiremos los datos a insertar en las tablas utilizando las celdas necesarias:

```
|Titulo 1 | Titulo 2 | Titulo 3|
|----------|:---------------:|------------------:|
|ASIX1 | Curso 24-25 | 33|
|DAW2 | Curso 24-25 | 32|
|ASIX2 | Curso 24-25 | 30|
```
La tabla quedaria de la siguiente manera:

|Titulo 1 | Titulo 2 | Titulo 3|
|----------|:---------------:|------------------:|
|ASIX1 | Curso 24-25 | 33|
|DAW2 | Curso 24-25 | 32|
|ASIX2 | Curso 24-25 | 30|

