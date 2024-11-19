# **Mis apuntes de 0373 - ASIX1**

1. [GITHUB](#1-github "Enlace a los apuntes de GitHub")
2. [MARKDOWN](#2-markdown "Enlace a los apuntes de MarkDown")
3. [HTML](#3-html "Enlace a los apuntes de HTML")


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

![Raphinha](https://github.com/AriamSS/0373_A01_DocumentacionApuntes_SanchezAriam/blob/main/R11.jpg?raw=true "Raphinha")
<br>
Un ejemplo de imagen

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



# 3. HTML

## 3.1 Introducción a HTML
- Lenguaje de marcado estándar para crear páginas web.
- Lenguaje más importante de Internet dado que sin HTML no se veria nada en el navegador.
- Define la estructura y el contenido o describe el contenido.
- Los elementos de HTML (etiquetas) son los bloques de construccion de las páginas HTML.

HTML (HyperText Markup Language): 
- HyperText: significa hipertexto y es un texto que enlaza con otros contenidos. 
- Markup: significa marca o etiqueta, ya que todas las páginas web están construidas en base a etiquetas. 
- Language: significa lenguaje.

HTML no es un lenguaje de programación. 
Fue creado por Tim Berners-Lee.

La estructura y contenido de HTML se define mediante etiquetas. Este es un lenguaje muy facil de interpretar, por eso es tan utilizado. Tambien es capaz de cambiar la apariencia de un texto mediante **CSS**.

## 3.2 Elementos
Las partes principales de un elemento son:
- Etiqueta de apertura
- Etiqueta de cierre
- Contenido
- Elemento

Se pueden colocar elementos dentro de otros elementos, a esto se le llama **anidamiento**.
  
### 3.2.1 ¿Que son las etiquetas?
Las etiquetas se pueden definir como código que tiene como función estructurar HTML. La etiqueta de apertura indica el inicio de un bloque HTML y la etiqueta de cierre indica el final de un bloque HTML, aunque estas no siempre se cierran.

```
Etiqueta de apertura: <p>
Etiqueta de cierre: </p>
```

**NORMAS BÁSICAS DE ETIQUETAS HTML**:
- Las etiquetas HTML suelen venir en pares, con una etiqueta de apertura y una de cierre, como por ejemplo ``<p>`` y ``</p>``. 
- Algunas etiquetas, conocidas como etiquetas vacias, no tienen una etiqueta de cierre. Algunas son: ``<img>``, ``<br>``...
- Las etiquetas HTML deben anidarse correctamente. Por ejemplo, si una etiqueta ``<b>`` se abre dentro de una etiqueta ``<p>``, debe cerrarse la etiqueta ``<b>`` antes de que se cierre la etiqueta ``<p>`` para poder leer el código corréctamente. 
- Los atributos de las etiquetas se especifican en la etiqueta de apertura y suelen tener el formato nombre "valor". Por ejemplo, en ``<img sre imagen.jpg>``, "src" es un atributo que especifica la ubicación de la imagen.
  
### 3.2.2 ¿Que son los atributos?
Los atributos buscan dar información extra a una etiqueta, dando detalles como por ejemplo:

```
<img src="URL">"Texto alternativo para la imagen" </img>
```

En esta etiqueta se puede ver la dirección o ubicación de la imagen y un texto que da información sobre la propia imagen.

- Los atributos siempre se incluyen en la etiqueta de apertura de un elemento. 
- Estos siempre deben contener espacio antes del nombre del elemento. 
- El nombre del atributo irá seguido por un signo igual (=).
- Comillas de apertura y de cierre, encerrando el valor del propio atributo.

# 3.3 Estructura básica de un fichero HTML
Un documento de HTML sigue una estructura básica, la cuál se puede implementar ejecutando **HTML 5** dentro del mismo documento. Una vez ejecutado quedaria de la siguiente manera:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

Cada una de las etiquetas tiene un signficado:
- ``<!DOCTYPE html>``: Define el tipo de documento, que seria HTML 5.
- ``<html></html>``: Contenedor principal del documento HTML.
- ``<head></head>``: Contiene informacion adicional sobre el documento, la cual no se muestra en la página web.
- ``<meta></meta>``: Proporciona metadatos, los cuáles son datos sobre los datos de la página y no son visibles directamente para los usuarios, pero son importantes para los navegadores en los que visualizamos nuestra página web.
- ``<title></title>``: Indica el titulo de la pagina web que aparece al abrir las pestaña en el navegador.
- ``<body></body>``: Muestra el contenido visible en la página web, todo lo que queremos crear y mostrar.

# 3.4 Etiquetas

### 3.4.1 Tipos de etiquetas
Las etiquetas se pueden clasificar en 2 tipos de elemento:
- Elementos de bloque: Elementos que requieren de una linea nueva para poder ejecutarse. También se pueden definir como grandes estructuras que pueden contener otros elementos de bloque.
Ej: `<h1>`-`<h6>`, `<p></p>`, `<ol>`, `<ul>`, `<li>`

- Elementos de línea: Elementos que se ubican en la misma línea, se ejecutan antes de un bloque. También se pueden definir como pequeñas estructuras que describen pequeños trozos de texto o datos, es decir, otros elementos de línea. 
Ej: `<strong>`, `<a>`

### 3.4.2 Etiquetas básicas de HTML

#### Rutas
Las rutas se usan en HTML para referenciar una imagen o una dirección URL. En otras palabras, podemos usar rutas para especificar la ubicación de estos archivos. Existen dos tipos de ruta:

- Ruta absoluta: Como su nombre indica, la ruta absoluta define la ubicación del archivo en la web al completo, comenzando desde el dominio. Un ejemplo seria: 

```
<img src="https.//www.example.com/images/logo.png" alt="Logo de Ejemplo">
```

- Ruta relativa: La ruta relativa especifica la ubicación del archivo en relación con el archivo actual. Por ejemplo:

```
<img src="images/logo.png" alt="Logo de Mi Sitio">
```

#### Enlaces
La etiqueta utilizada en HTML para la creación de enlaces es <a>. Esta etiqueta es una etiqueta de linea, ya que podemos colocar enlaces y escribir texto alrededor de los mismos. Pueden haber dos tipos de enlaces:

- Enlaces a páginas externas: Este sirve para fabricar enlaces que nos dirigan a páginas web externas. La estructura a usar para crear este tipo de enlace seria:
  
```
<a href="URL página web externa">Texto Visible</a>
```

- Enlaces a páginas locales: Estos enlaces nos dirigen a un documento local propio. Un ejemplo:

```
<a href="index.html" title="Volver a la página de inicio">Inicio</a>
```

En estos códigos, el atributo **href** nos indica la dirección del enlace. 

#### Imágenes
Uno de los recursos más utilizados en páginas web. Las imágenes proporcionan informacion de manera visual, lo que da soporte a nuestra página web y mejora la estética de la misma. La etiqueta utilizada para insertar una imagen es ``<img>``, etiqueta que no tiene tiene cierre, es decir, se cierra en sí misma. Un ejemplo de uso:

```
<img src="imagen.png" alt="Imagen principal de la página web" width="120" height="120">
```

Donde:
``<src>`` --> Atributo que especifica la ubicación de la imagen.
``<alt>`` --> Proporciona un texto alternativo para la imagen.
``<width> / <height>`` --> Modifica las medidas de la imagen; altura y anchura.

#### Listas
La listas nos sirven para enumerar ciertos conceptos o desarrollos de texto, como pueden ser unas instrucciones, un indice u otros. Cada elemento de una lista debe colocarse dentro de un elemento ``<li>``. Pueden haber dos tipos de lista:

- Listas ordenadas:Son aquellas en las que el orden si importa. La etiqueta a usar es ``<ol>``, que quiere decir ***ordered list***. Un ejemplo:

```
1. Punto 1
2. Punto 2
3. Punto 3
```

- Listas desordenadas: Son aquellas en las que el orden no es relevante. La etiqueta a usar es ``<ul>``, que quiere decir ***unordered list***. Un ejemplo:

```
- Punto 1
+ Punto 2
* Punto 3
```

### 3.4.3 Otras etiquetas
**Encabezados** (``<h1>, ..., <h6>``): Elementos de bloque. Permiten especificar el tipo de encabezado o subencabezado del contenido. 

**Párrafos** (``<p>``): Elementos de bloque. Se utilizan para encerrar párrafos de texto, entendiendo como párrafo un conjunto de frases relacionadas entre sí. 

**Salto de línea** (``<br>``). Permite agregar un salto de línea (o "intro") entre párrafos. Muy útil para añadir espacio entre lineas, mejorando la legibilidad.

**Separador de línea** (``<hr>``). Permite agregar una línea horizontal divisoria. Útil para separar visualmente párrafos por ejemplo, mejorando la estética del texto.

**Énfasis** (``<em>``, ``<strong>``). Cuando queremos dar énfasis a una parte de texto para destacar su importancia, disponemos de dos etiquetas. La etiqueta ``<em>`` se utiliza para dar énfasis y la etiqueta ``<strong>`` para dar más énfasis aún.

## 3.5 Código HTML
Para conseguir que nuestro código HTML sea correcto en todos los aspectos, hay que tener en cuenta varias facetas que influyen en el mismo código. 

### 3.5.1 Legibilidad y organización del código
La legibilidad del código fuente es la claridad con la que está codificado, la cuál nos permite entenderlo de manera fácil y rápida. Es fundamental que el código fuente HTML que generemos sea legible.

La organización del código fuente es la estructuración de la aplicación web en varios archivos, asi como la clasificación de estos archivos en los directorios que sean necesarios. Es recomendable que el archivo de inicio de las aplicaciones tenga el nombre index.html.

Se debe tener en cuenta que todo el trabajo que hayamos desarrollado sea legible para aquellos que trabajan con nuestro documento, de manera que puedan entender que hemos hecho y por qué lo hemos hecho. 


Hay varias técnicas para que el código sea legible y tenga una correcta organización:

- Los comentarios

- La indentación del código

- La organización de los archivos

#### 3.5.2 Comentarios
Dentro de un documento HTML podemos poner anotaciones o comentarios que nos serviran para guiarnos o entender el código. Estas anotaciones no se visualizaran en nuestra página web. La sintaxis para añadir comentarios es la siguiente:

```
<!-- comentario -->
```

### 3.5.3 Validación del código
La validación del código es el proceso a través del cuál verificamos que nuestro código HTML sea correcto y cumpla con los estandares establecidos por el World Wide Web Consortium, de manera que la validación ayuda a detectar cualquier fallo y nos advierte ante cualquier parte del código que no sea del todo correcta.

El validador --> [W3C: Validador de HTML](https://validator.w3.org "Validador de HTML W3C")

## 3.6 Formularios 
