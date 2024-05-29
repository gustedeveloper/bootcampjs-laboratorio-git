# Bootcamp JavaScript 2 - Lemoncode

## Laboratorio Git

Este laboratorio tiene como objetivo practicar los comandos básicos de Git:

1. Crear un repositorio en local.
2. Subir el repositorio a GitHub.
3. Hacer commit y push.
4. Crear una rama.
5. Hacer un merge y resolver los conflictos que se presenten si fuera el caso.

A continuación, me dispongo a explicar todo el proceso que he seguido para crear este laboratorio.

### Crear e inicializar un repositorio en local

Localizo, a través del terminal, el directorio en el que deseo crear el repositorio; creo una carpeta con el nombre del repositorio, ingreso en ella e inicializo el repositorio de Git

<img src="./capturas/img1.png" />

### Subir el repositorio a GitHub

<img src="./capturas/img2.png"/>

Toca elegir un nombre que esté disponible para el repositorio y crearlo

<img src="./capturas/img2.1.png"/>

Copio el link del repositorio

<img src="./capturas/img2.2.png"/>

Conecto el repositorio local con el repositorio en GitHub

<img src="./capturas/img2.3.png"/>

### Hacer _commit_ y _push_

Creo los primeros archivos

<img src="./capturas/img3.png"/>

Los añado al staging y creo un commit con un mensaje descriptivo

<img src="./capturas/img3.1.png"/>

Toca subir los cambios al repositorio en GitHub

<img src="./capturas/img3.2.png"/>

Refresco la página para ver que todo se ha subido correctamente

<img src="./capturas/img3.3.png"/>

### Crear una rama

A continuación, creo una nueva rama llamada **_development_**

<img src="./capturas/img4.png"/>

Cambio a la nueva rama

<img src="./capturas/img4.1.png"/>

Realizo cambios en uno de los archivos en la rama **_development_**. En este caso, he añadido un párrafo al archivo **_html_**

<img src="./capturas/img4.2.png"/>

Reflejo los cambios añadiéndolos y realizando un **_commit_**

<img src="./capturas/img4.3.png"/>

Subo los cambios a GitHub

<img src="./capturas/img4.4.png"/>

### Hacer un _merge_ y resolver los conflictos que se presenten si fuera el caso

Toca combinar ambas ramas. Para ello, vuelvo a la rama **_main_**

<img src="./capturas/img5.png"/>
<img src="./capturas/img5.1.png"/>

Hago **_merge_**. Si no hay conflictos, los cambios realizados en la rama **_development_** se incorporarán directamente a la rama **_main_**

<img src="./capturas/img5.2.png"/>

Si hubiese conflictos (en el escenario de que estoy trabajando en un equipo y alguien elimina un archivo en la rama **_main_**, añade y hace commit de los cambios, y yo por mi parte, he realizado cambios en ese archivo en la rama **_development_**, los he añadido y realizado commit) ocurriría lo siguiente a la hora de hacer **_merge_**:

Git nos avisaría del conflicto

<img src="./capturas/img6.png"/>

Para solucionarlo, vamos al apartado de **_Source control_** y nos mostraría lo siguiente:

<img src="./capturas/img6.1.png"/>

Clicando sobre el + aparecería la siguiente pestaña que explica claramente el origen del conflicto y las posibles soluciones

<img src="./capturas/img6.2.png"/>

> Otra alternativa sería dar marcha atrás al **_merge_**, si todavía no hemos commiteado, con el siguiente comando

```
git merge --abort
```

En este caso, decido mantener la versión de la rama **_development_** que sería recuperar el archivo borrado. Una vez solucionado el conflicto, commiteo los cambios

<img src="./capturas/img6.3.png"/>

Y hago **_push_** al repositorio de GitHub

<img src="./capturas/img7.png"/>
