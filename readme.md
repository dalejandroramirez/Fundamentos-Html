## Fundamentos de html

    - < meta name="robots",conten="indexm follow" > : Permite que los robots de ubiquen la página web
    
    - < meta name="viewport" content="width=device-width, initial-scale=1.0"> : el "viewport" es el movimiento de izquierda a derecha, y mejora la experiencia del usuario
    
    - < meta name="description" content="pequeño resumen" > 

## Anatomia de una pagina web

![Image text](imagenes/Anatomia.webp)

## HTML: hypertext Markup Languege

    Existen etiquetas de contenido y etiquetas contenedoras.

    ### Etiquetas contenedoras:
    Son las encargadas para encapsular contenido


![Image text](imagenes/Etiquetascontenedoras.png)

### Tamaño máximo recomendado para una imágen: 70 kb
    Herramientas para optimizar imágenes:

    - Tiny PNG: Comprime el tamaño de una imagen, para hacerla más ligera.

    - Verefix: Elimina los metadatos de una imagen, para reducir su tamaño.

### Tipo de imagenes
![Image text](imagenes/Lossless.png)
![Image text](imagenes/Lossy.png)

![Image text](imagenes/Tabladifererencias.webp)

## Atributos de la etiqueta img

    La etiqueta img cuenta con dos atributos, el atributo “src” y el segundo atributo es “alt”. Ambos son importantes.

El atributo de “src” es para mostrar en dónde se encuentra la imagen que vamos a incrustar. Las imágenes se pueden obtener de alguna carpeta o una URL que obtengamos de internet.
<ul>
    <li>En caso de que el nombre de tu imagen lleve algún espacio, deberás sustituir ese espacio con un guion o guion medio. Caso contrario, el navegador no podrá reconocer la ubicación.
    </li>
</ul>

alt sirve para agregar una descripción a nuestra imagen. Esto es útil por cuestiones de SEO y también para accesibilidad (por ejemplo para personas con visión reducida).
<ul>
    <li>
        < img/>, a diferencia de la gran mayoría de las demás etiquetas de HMTL, no necesita una etiqueta de cierre.
     </li>
</ul>

- https://tinypng.com/ : convierte las imagenes en imagenes menos pesadas

## ¿Como agregar videos?

![Image text](imagenes/video1.png)

![Image text ](imagenes/video2.png)

![Image text ](imagenes/video3.png)


<h1>         source<h1/>

![Image text ](imagenes/video4.png)


## ¿Como generar un formularios?


![Image text](imagenes/formularios1.webp)

## Autocompletado y Requerimientos
![Image text ](imagenes/autocompletado1.webp)

 ## Select y list
<center><img src="imagenes/select.png" width="375" height=300px ><img src="imagenes/list.png" width="375" height=300px>
</center>

<img src="imagenes/submitButton.png">

# CSS 
Css es lo que le da el style a la pagina, cada objeto en html se puede llamar por su class, id , tipo

<img src="imagenes/etiquetas1.webp" width=450px height=300px><img src="imagenes/reglascss.png" width = 450px height=300px>


<center><h2>Metodo BEM</h2></center>
La metodología Bloque, Elemento, Modificador (comúnmente conocida como BEM) es una convención de nomenclatura popular para clases en HTML y CSS. Desarrollado por el equipo de Yandex, su objetivo es ayudar a los desarrolladores a comprender mejor la relación entre HTML y CSS.

-Solo usa clases. Las nombra siguiendo el siguiente patrón: BLOQUE__ELEMENTO--MODIFICADOR (son 2 guiones, se usa 1 guión para separar palabras).

- Bloque: sección que puede funcionar por sí sola.
- Elemento: forma una de las partes del bloque.
- Modificador: variaciones de un mismo bloque/elemento.

<center>
<img src="imagenes/bem1.png" width=550px height=450px>
</center>

# PseudoClases y PseudoElementos
<center>
<img src="imagenes/pseudoclases1.png" scale=1.5px>

<img src="imagenes/pseudoclases.png" width=300px height=200px>
</center>

<center> <h2>Anatonia de una linea en CSS</h2></center>
<center>
<img src="imagenes/reglacss.webp">
</center>

## Modelo de cajas
En la web los elementos se piensan en forma de rectángulos. A esto se le conoce como Modelo de caja.
Las cajas tienen parámetros que podemos editar en nuestro CSS
<center>
<img src="imagenes/modelodecaja2.png" width =300px height=200px>
</center>


- Margin
    Espacio que hay del borde de la caja hacia afuera. Visualmente, permite separar a la caja de elementos externos.

- Padding

    Espacio que hay del borde de la caja hacia adentro. Visualmente, permite separar a la caja de elementos internos.

- Border

    Es el borde de la caja. Por defecto, a partir de ahí medimos las distancias de nuestra caja con elementos internos o externos.


## ojo !!!! con el modelo de caja

<center>
<img src="imagenes/modelocaja1.png">
</center>

Por defecto en el modelo de caja de CSS, el ancho y alto asignado a un elemento es aplicado solo al contenido de la caja del elemento. Si el elemento tiene algún borde (border) o relleno (padding), este es entonces añadido al ancho y alto a alcanzar el tamaño de la caja que es desplegada en pantalla. Esto significa que cuando se definen el ancho y alto, se tiene que ajustar el valor definido para permitir cualquier borde o relleno que se pueda añadir.
*
*
La propiedad box-sizing puede ser usada para ajustar el siguiente comportamiento:

- content-box es el comportamiento CSS por defecto para el tamaño de la caja (box-sizing). Si se define el ancho de un elemento en 100 pixeles, la caja del contenido del elemento tendrá 100 pixeles de ancho, y el ancho de cualquier borde o relleno ser añadirá al ancho final desplegado.

- border-box le dice al navegador tomar en cuenta para cualquier valor que se especifique de borde o de relleno para el ancho o alto de un elemento. Es decir, si se define un elemento con un ancho de 100 pixeles. Esos 100 pixeles incluíran cualquier borde o relleno que se añadan, y la caja de contenido se encogerá para absorber ese ancho extra. Esto típicamente hace mucho más fácil dimensionar elementos.

## Herencias
Herencia y sus valores:
<ul>
<li> Inherit. Este es un valor por medio de una keyword que especifica que, a la propiedad que se la apliquemos debe de heredar los valores de su elemento padre. Podemos decir que la palabra Inherit significa “Usa el valor de mi padre”, si el elemento padre no tiene definido dicho valor el navegador seguirá el DOM hasta que encuentre un elemento superior que lo contenga, y en ultima instancia de no tenerlo ningún elemento superior se aplicara el valor por defecto.
</li>


<li>Initial. Este valor pertenece a la especificación CSS3 y cuando aplicamos a una propiedad el valor initial estamos dando el valor inicial y predefinido por el navegador en cuestión.
</li>


<li>Upset. Este valor unset es una combinación entre inherit y initial, cuando utilizamos este valor en una propiedad esta tratara de heredar el valor de su elemento padre si este esta disponible, de no ser así este valor colocará el valor de la propiedad en su valor inicial, como si usáramos inherit e initial juntos
</li>
</ul>

<img src="imagenes/herencia1.png" width=800px heigth= 300px>
<img src="imagenes/herencia2.png" width= 800px heigth= 300px>

## ¿Cómo se controla el orden de las declaraciones de CSS?

<ul>
<li>importancia</li>
<li>Especificidad</li>
<li>Orden en la fuente</li>

</ul>

<h3>Orden al declarar CSS</h3>

1. Importancia
    a) Hoja de estilo de agente de usuario (estilos del navegador).
    b)Declaraciones normales en hojas de estilo de autor (CSSDocument.css)
    c)Declaraciones importantes en hojas de estilos de autor (utiliza el import !import) Evitarlo

2. Especificidad 


<img src="imagenes/herencia3.png">

Nota: Entre más cerca esté el 1 a la izquierda mayor preferencia le dará el navegador

          Nota 2: Tratar de evitar el uso de important e inline style

          Nota 3: Cuando se usa dos o más selectores la especificidad que le dará el navegador web será dada por la suma de los selectores que se usaron (Son valores binarios entre mayor sea este valor mayor especificidad tendrá)
 
3. Orden en las fuentes: Los estilos que se llamen al final sobrescribirán los estilos ya establecidos, es como pintar una casa la última capa de pintura quitará el color de la primera

# Buenas y malas practicas
<img src="imagenes/herencia4.png" width= 800px heigth= 300px>

<img src="imagenes/herencia5.png" width= 800px heigth= 300px>

## nota: NO USAR ID AL MOMENTO DE DAR ESTILOS