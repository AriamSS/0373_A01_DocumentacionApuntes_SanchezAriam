# **Mis apuntes de 0373 - ASIX1**

1. [GITHUB](#1.Github "Enlace a los apuntes de GitHub")
2. [MARKDOWN](#2.MarkDown "Enlace a los apuntes de MarkDown")
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
  


