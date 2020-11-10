---
title: "Flujo de trabajo"
date: 2020-11-10T08:22:03-03:00
author: odelaf
draft: false
categories:
    - blog
tags:
    - "texto plano"
slug: workflow
authorbox: true # Enable authorbox for specific page
toc: true # Enable Table of Contents for specific page
sidebar: false 
---

Ya sea por una tendencia irresistible a procrastinar o simplemente porque nos interesa ser más eficientes en nuestro trabajo, muchas veces usamos parte de nuestro tiempo buscando información sobre cómo organizar de manera eficiente nuestro trabajo. Quizás generalizo mi propia experiencia y mucha gente no lo ve necesario. He dedicado tiempo a estos asuntos y llegué a un punto donde me pareció necesario escribirlo para poder volver a mis hallazgos en caso de que sea necesario (mi memoria es frágil). Lo hago público por si es de utilidad o interés para alguien más.

Con flujo de trabajo me refiero a una organización de los distintos momentos que componen el trabajo académico, que clasifico para estos propósitos así:

* Notas personales y notas de lectura
* Escritura
* Compartir

En lo que sigue explico la manera en que he organizado mi trabajo, presentado algunas ideas generales sobre las notas personales y de lectura, los beneficios de escribir en texto plano, cómo los sistemas de referencia facilitan muchísimo el trabajo, y de qué manera es posible utilizar algunas herramientas tecnológicas muy sencillas que ayudan en la elaboración del manuscrito que será compartido o publicado.

Antes de empezar, una prevención: trabajar con Microsoft Word es cómodo y no requiere de la instalación de nada más. Mi flujo de trabajo considera el uso de los siguientes software:

* [Obsidian](https://obsidian.md/) (para las notas, pero se puede usar una libreta y lápiz, no es imprescindible)
* [VS Code](https://code.visualstudio.com/) y algunas extensiones (para escribir en texto plano)
* [Zotero](https://www.zotero.org/) y la extensión [Better BibTeX](https://retorque.re/zotero-better-bibtex/) (para las referencias)
* [Pandoc](https://pandoc.org/) (para convertir el archivo en texto plano en docx)

No estoy en condiciones de hacer una estimación de cuánto tiempo toma rehabilitarse de Microsoft Word y trabajar en texto plano. Para mí es sencillo explicarlo porque ya lo hago así desde hace un tiempo. Creo que puede llegar a ser frustrante embarcarse en otra forma de trabajar, distinta a la que uno está acostumbrado. Y mi explicación no cubre en detalle todo lo que esto implica, lo que obligará en algunos casos a buscar en internet la respuesta (mi propia rehabilitación de Microsoft Word fue así). En cualquier caso, para mí este cambio valió completamente la pena y se ha vuelto mucho más fácil mi trabajo. Pero al final dependerá de cada persona, sus hábitos y gustos.

## Notas personales y notas de lectura

Previo a cualquier trabajo existe una etapa que podemos llamar «exploratoria», en la cual nos informamos en términos gruesos de algún tema según la literatura que tengamos a mano. De esta lectura, en algún momento asumimos una posición que queremos desarrollar más latamente.

Para familiarizarse con las ideas que se discuten sobre un tema e ir delineando una posición frente a ellas, tomar notas de lo que leemos es fundamental. Esto es algo que intuitivamente vamos desarrollando y cada persona tendrá su manera de hacerlo. En mi caso, fui probando distintas opciones que se me iban ocurriendo, buscando alguna que me resulte más cómoda, hasta que di con el libro _How to take smart notes_ de Sönke Ahrens, que explica el sistema que diseñó Luhmann para su trabajo y que es conocido como _Zettelkasten_.

A grandes rasgos, él distingue entre notas de lectura, que corresponde a aquello de que trata el texto dicho en nuestras palabras, y notas personales, que refiere en general a ideas que nos surgen cuando reflexionamos sobre los asuntos que nos ocupan. Resumiendo, creo que hay tres ideas principales en este método:

* Tomar notas con lápiz y papel durante la lectura, intentando establecer un dialogo con la autora o autor del texto, colocando las ideas que nos interesen en nuestras palabras y, si lo estimamos pertinente, agregando comentarios personales. Lo importante de usar lápiz y papel es que nos invita a pensar lo que vamos a escribir por la sencilla razón de que nos toma más tiempo escribir a mano que escribir en un teclado. En otras palabras, usar lápiz y papel nos conduce a una lectura atenta y pausada.
* En cada lectura, en lugar de resumir todo lo que se dice, enfocarse en el trabajo que realizamos. Es decir, fijarse principalmente en qué medida lo que se dice en el texto contribuye a nuestro trabajo.
* Lo más importante de todo esto es encontrar alguna manera de poder relacionar todas estas notas. Aquí la sugerencia es etiquetarlas, pero pensando en qué contexto sería útil rescatar esa idea (que inevitablemente olvidaremos), pero que podemos recuperar gracias a este sistema.

En este video, Ahrens explica en qué consiste este método:

{{< vimeo 275530205 >}}

Finalmente, es útil trabajar con algún software que ayude a organizar las notas y vincularlas por medio de las etiquetas. Yo he estado usando [Obsidian](https://obsidian.md/) con resultados bastante satisfactorios, aunque toma un poco de tiempo entender cómo usarlo.

## Sistema de referencia

Todo trabajo académico descansa en publicaciones anteriores. La referencia a ellas cumple diversos propósitos, tales como situar el trabajo propio en algún marco de discusión que se encuentra dibujado por investigaciones anteriores, referir a trabajos ajenos que sirven como contrapunto a las ideas que uno desarrolla, hacer una remisión a un desarrollo más profundo de alguna idea que nuestro trabajo menciona, etc. En la academia existen ciertas prácticas para ello, que pueden organizarse por medio de dos grandes tipos de cita: en el texto o al pie de página. Adicionalmente, puede tratarse de una referencia breve (que se desarrolla al final del texto en la sección dedicada a ello) o una referencia completa que luego se usa en una versión más breve.

La diversidad de maneras que existen para hacer referencia a otros trabajos es muchas veces abrumadora. Cada revista académica o editorial maneja su propia manera de hacerlo. Para poder lidiar con ello, un sistema de referencia es fundamental. Este se compone de dos archivos que sirven para automatizar el proceso: un archivo con la base de datos (extensión .bib) y un archivo con el sistema de citas (extensión .cls).

### Una base de datos bibliográfica (bib)

Una herramienta fundamental son las bases de datos bibliográficas. La idea es simple: en un solo archivo se encuentran registrado todo el material bibliográfico que vamos reuniendo, consignando la información relevante para su referencia posterior. Este registro se estructura de manera estándar para que pueda ser procesado por distintos software al momento de generar una referencia.

Yo uso [Zotero](https://www.zotero.org/) con estos fines. Este software tiene dos características que me han sido muy útiles. La primera es que automáticamente genera una «cite key». Se trata de un código único establecido para cada publicación que se encuentra en el registro, que se puede usar luego en el texto de manera sencilla mientras uno escribe. Posteriormente, un software se encarga de convertir ese código en la cita correspondiente conforme al sistema de cita deseado (tomado desde el archivo cls).

La segunda característica es la creación de un archivo único (extensión .bib) donde se encuentran todas las publicaciones del registro, que se va actualizando automáticamente cada vez que se actualiza la base de datos (para ello, es necesario instalar la extensión [Better BibTeX](https://retorque.re/zotero-better-bibtex/)).

### Un sistema de citas

En general, toda publicación cuenta con una manera de hacer referencias a otros trabajos que se establece como un conjunto de reglas. Los sistemas más comunes son los establecidos por la American Psychological Association (APA) y la Chicago University Press. El proceso aquí creo que es conocido: primero es necesario familiarizarse a grandes rasgos con el sistema (si el título de un artículo de revista va entre comillas o no, si el año va al inicio o al final, si se escribe el nombre completo o solo las iniciales, etc.). Y en caso de dudas, se pueden consultar las reglas y seguirlas.

Como estas reglas son sencillas, es posible automatizar el proceso. El archivo cls contiene las reglas del sistema elegido en lenguaje de programación, las cuales son aplicadas al manuscrito en texto plano (el input) y dan como resultado un manuscrito con todas las referencias completadas (el output). Este sencillo proceso puede realizarse tantas veces como sea necesario y cambiando el archivo cls entregará el manuscrito bajo las reglas que allí se encuentren.

Por cierto, no es necesario aprender programación para traducir las reglas para las referencias y crear un archivo csl. Estos archivos son [públicos](https://citationstyles.org/).

## Texto plano

Para que sea posible esta automatización de las referencias, es extraordinariamente útil trabajar en texto plano. Lo contrario a texto plano es el texto enriquecido, una de las características de procesadores de texto como Microsoft Word. En estos, la pantalla nos muestra el resultado final del texto que estamos trabajando con los distintos formatos que le damos (el tipo de letra, interlineado, títulos, negritas, cursivas, etc.).

Trabajar con texto enriquecido tiene algunos inconvenientes. Uno de ellos es que te hace perder tiempo en el formato del texto, lo que distrae de la escritura (que al final es lo importante). Además, consume mucho recursos del equipo en el que trabajamos y eso hace que el desempeño del software no sea óptimo e incluso falle.

Como alternativa, es posible escribir en texto plano. En esta modalidad solo existen caracteres que deben respetar las reglas de composición establecidas en el lenguaje informático que utilicemos. Esto que pareciera sonar a aprender alemán o chino, en realidad es bastante sencillo (más sencillo que saber dónde está el botón para negritas en Word). Yo uso el lenguaje Markdown (extensión .md) y el documento se ve algo así:

```markdown
    # Esto es un título
    ## Esto es una sección
    ### Esto es una subsección
    #### Esto es una subsub...se entiende la idea creo

    Si queremos destacar alguna palabra o frase, se puede marcar en **Negritas** o en _cursivas_

    Podemos también hacer listas numeradas o no numeradas

    1. uno
    2. dos
    3. tres

    * item
    * item
    * item

    > Esto es una cita.
```

En el siguiente video se explica Markdown con un poco más de detalle. Solo quisiera destacar lo ágil que se vuelve la escritura cuando se usa texto plano.

{{< youtube hpAJMSS8pvs >}}

## Compartir

He dicho que el uso de texto plano agiliza muchísimo el trabajo. Sin embargo, habitualmente nuestros borradores y trabajos los compartimos en otros formatos, como docx o pdf. Aquí entra otro software llamado Pandoc. Básicamente, lo que hace es convertir nuestro archivo en texto plano en el formato requerido. Para ello, hay que hacer algo poco habitual pero que en realidad es muy sencillo, similar a escribir la dirección de una página web en un navegador pero, en este caso, es una línea de comandos que se escribe en una interfaz (Terminal, en Mac):

``pandoc manuscrito.md -s --reference-doc custom-reference.docx -o manuscrito.docx``

En este ejemplo el input es un manuscrito escrito en texto plano (manuscrito.md) y el output es un archivo docx (manuscrito.docx), que en su elaboración sigue el formato de otro archivo docx que fue previamente creado para estos efectos (custom-reference.docx).

Al principio, por estar habituados a trabajar en Office puede parecer escalofriante. Toma un poco de tiempo preparar todo lo necesario para poder trabajar con texto plano y eso requiere aprender algunas cosas nuevas. Pero el poco tiempo que requiere este pequeño aprendizaje se compensa significativamente con la agilidad que se gana al trabajar en texto plano.

En este video se explican en más detalle y de manera práctica los preparativos para trabajar en texto plano, usando como editor el software VS Code, el lenguaje Markdown y el conversor de documentos Pandoc.

{{< youtube J86Pm62XM_Q >}}
