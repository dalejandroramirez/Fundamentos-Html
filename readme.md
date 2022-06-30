

## Fundamentos de html

    - < meta name="robots",conten="indexm follow" > : Permite que los robots de ubiquen la página web
    
    - < meta name="viewport" content="width=device-width, initial-scale=1.0"> : el "viewport" es el movimiento de izquierda a derecha, y mejora la experiencia del usuario
    
    - < meta name="description" content="pequeño resumen" > 

## Anatomia de una pagina web

<center> <img src="imagenes/Anatomia.webp" width=100%></center>

## HTML: hypertext Markup Languege

    Existen etiquetas de contenido y etiquetas contenedoras.

    ### Etiquetas contenedoras:
    Son las encargadas para encapsular contenido

<img src="imagenes/Etiquetascontenedoras.png" width=1200px>


### Tamaño máximo recomendado para una imágen: 70 kb
    Herramientas para optimizar imágenes:

    - Tiny PNG: Comprime el tamaño de una imagen, para hacerla más ligera.

    - Verefix: Elimina los metadatos de una imagen, para reducir su tamaño.

### Tipo de imagenes
<img src="imagenes/Lossless.png" width = 50% height=450px><img src="imagenes/Lossy.png" width = 50% height=450px><img src="imagenes/Tabladifererencias.webp" width=100% >


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


<img src="imagenes/video1.png" width=100%>
<img src="imagenes/video2.png" width=100%>]
<img src="imagenes/video3.png" width=100%>]


<h1>         source<h1/>



<img src="imagenes/video4.png" width=100%>


## ¿Como generar un formularios?


![Image text](imagenes/formularios1.webp)

## Autocompletado y Requerimientos
![Image text ](imagenes/autocompletado1.webp)

 ## Select y list
<center><img src="imagenes/select.png" width=100% height=500px ><img src="imagenes/list.png" width=100% height=500px>
</center>

<img src="imagenes/submitButton.png" width=100% height=100%>

# CSS 
Css es lo que le da el style a la pagina, cada objeto en html se puede llamar por su class, id , tipo

<img src="imagenes/etiquetas1.webp" width=100% height=100%><img src="imagenes/reglascss.png" width = 100% height=100%>


<center><h2>Metodo BEM</h2></center>
La metodología Bloque, Elemento, Modificador (comúnmente conocida como BEM) es una convención de nomenclatura popular para clases en HTML y CSS. Desarrollado por el equipo de Yandex, su objetivo es ayudar a los desarrolladores a comprender mejor la relación entre HTML y CSS.

-Solo usa clases. Las nombra siguiendo el siguiente patrón: BLOQUE__ELEMENTO--MODIFICADOR (son 2 guiones, se usa 1 guión para separar palabras).

- Bloque: sección que puede funcionar por sí sola.
- Elemento: forma una de las partes del bloque.
- Modificador: variaciones de un mismo bloque/elemento.

<center>
<img src="imagenes/bem1.png" width=100% height=100%>
</center>

# PseudoClases y PseudoElementos
<center>
<img src="imagenes/pseudoclases1.png" width=100%>

<img src="imagenes/pseudoclases.png" width=100% height=100%>
</center>

<center> <h1>Anatonia de una linea en CSS</h1></center>
<center>
<img src="imagenes/reglacss.webp" width=100%>
</center>

## Modelo de cajas
En la web los elementos se piensan en forma de rectángulos. A esto se le conoce como Modelo de caja.
Las cajas tienen parámetros que podemos editar en nuestro CSS
<center>
<img src="imagenes/modelodecaja2.png" width =50% height=50% >
</center>


- Margin
    Espacio que hay del borde de la caja hacia afuera. Visualmente, permite separar a la caja de elementos externos.

- Padding

    Espacio que hay del borde de la caja hacia adentro. Visualmente, permite separar a la caja de elementos internos.

- Border

    Es el borde de la caja. Por defecto, a partir de ahí medimos las distancias de nuestra caja con elementos internos o externos.


## ojo !!!! con el modelo de caja

<center>
<img src="imagenes/modelocaja1.png" width=100%>
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

<img src="imagenes/herencia1.png" width= 100% heigth= 100%>
<img src="imagenes/herencia2.png" width= 100% heigth= 100%>

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


<img src="imagenes/herencia3.png" width=100%>

Nota: Entre más cerca esté el 1 a la izquierda mayor preferencia le dará el navegador

          Nota 2: Tratar de evitar el uso de important e inline style

          Nota 3: Cuando se usa dos o más selectores la especificidad que le dará el navegador web será dada por la suma de los selectores que se usaron (Son valores binarios entre mayor sea este valor mayor especificidad tendrá)
 
3. Orden en las fuentes: Los estilos que se llamen al final sobrescribirán los estilos ya establecidos, es como pintar una casa la última capa de pintura quitará el color de la primera

# Buenas y malas practicas
<img src="imagenes/herencia4.png" width= 100% heigth= 100%>

<img src="imagenes/herencia5.png" width= 100% heigth= 100%>

## nota: NO USAR ID AL MOMENTO DE DAR ESTILOS.


# Combinadores


<img src="imagenes/combinado2.webp"
width= 100% heigth= 100%>


<img src="imagenes/combinadores2.png"
width= 100% heigth= 100%>

<img src="imagenes/combinado1.webp"
width= 100% heigth= 100%>

## Jugar------------> https://flukeout.github.io/


## Medidas relativas y Medidas absolutas

medida absoluta: el valor de este no cambia y siempre sera el mismo asi la pagina cambie su tamaño, las medidas absolutas son:
.
mm = milimetros
cm = centimetros
in = pulgada
pc = picas
px = pixel
.

las medidas relativas: estas medidas heredan el tamaño o se basan en algun tamaño que se alla seleccionado y el valor ira cambiando segun si la pagina cambia de tamaño, las medidas relativas son :
.
%
em 
rem

<center><img src="imagenes/medidas1.png" width= 100% heigth= 100%> </center>

## Medida relativa EM y REM

* MEDIDA EM: va a tomar el tamaño de fuente que tenga el padre directo, o en su defecto, a su ancestro más próximo que tenga un tamaño declarado.

* MEDIDA REM
    rem es una unidad de medida dentro de css, que nos permite utilizar a nuestro html como guía en cuanto a los tamaños.

* ¿Cómo funciona  rem?
lo primero que debes entender es que, por ejemplo, si sabemos que siempre por defecto nuestro tamaño de fuente es de 16px(proveniente del documento html), pues entonces 1rem es igual a 16 pixeles, ¿fácil no?
UN TRUCO QUE TE VA A SALVAR LA VIDA


<center><img src="imagenes/medidas2.png" width= 100% heigth= 100%>
 </center>



## min width and max width

* Min-height: se utiliza para definir la altura mínima de un elemento dado. Impide que el valor de la propiedad height llegue a ser más pequeña que la especificada en la altura mínima ( min-height ). Se refiere a la altura del bloque contenedor.

* Max-height: se utiliza para definir la altura máxima de un elemento dado. Impide que el valor de la altura pueda llegar a ser más grande que la de max-height . Porcentajes: se refiere a la altura del bloque contenedor.

* Min-width: se usa para determinar la anchura mínima de un elemento. Previene que la propiedad width pueda ser inferior que min-width . Aplicable a: elementos de tipo bloque. Porcentajes: se refieren a la anchura del bloque contenedor.

* Max-width: define el ancho máximo que un elemento puede tener, max-width cambia el tamaño del elemento si el valor de width es mayor que el de max-width.

## Resolver problema de la clase 37

## Display

<img src="imagenes/display1.png">

# resolver el problema de la clase 39 sin usar flex

# Flex

Flex es un tipo de display que permite que el contenedor padre sea flexible a los cambios que puedan tener los elementos hijos en su alineación.

Una vez tengamos el elemento padre con display flex tenemos otras propiedades que podremos usar para nuestro beneficio.

<center><img src="imagenes/flex1.webp" width= 100% heigth= 100%></center>

juego de flex : https://flexboxfroggy.com/#es

<center><img src="imagenes/flex2.png" width= 100% heigth= 100%></center>

## hacer el problema de la clase 37 con flex


## Variables en css

<center><img src="imagenes/variables1.png" width= 100% heigth= 100%></center>


## web-font

Los import de google fonts no son tan buenas prácticas porque pegan en el performance, a pesar del display=swap que agregó google para mitigar el daño aún así es mejor hacerlo en el head de html usando el link que nos proporciona.

Es una buena práctica cargar solo una fuente por proyecto.

# Responsive Design

¿Qué es Responsive Design?
Son todas esas técnicas que usamos para adaptar nuestras aplicaciones web a la mayor cantidad de pantallas

* Break points: hay que entenderlos como las distintas medidas(en el width) que podamos encontrar en los dispositivos donde se vera nuestra aplicación para poder reposicionar de mejor manera los elementos de nuestra aplicación.

* Media quieries: son líneas de códigos que se escriben en el archivo css que sirven para condicionar ciertas características de nuestra aplicación web dependiendo del tamaño del dispositivo de donde se este renderizando.
Ejemplo:

<center> <img src="imagenes/webFont1.png" width= 100% heigth= 100%></center>

- Ojo: la medida que va después de min-width es un break point, o sea la medida del width un dispositivo

Buenas Practicas
Desarrollar nuestras aplicaciones web con las metodología de Mobile first. Empezando a diseñar primero para los dispositos mas pequeños y luego ir aumentando el tamaña del dispositivo

<h3> Se puede aplicar directamente en el HTML, lo cual es mejor práctica:
</h3>
<center> <img src="imagenes/webFont2.png" width= 100% heigth= 100%></center>

# mostly fluid

<center> <img src="imagenes/montlyfluid2.webp" width= 100% heigth= 100%></center>

# Layout Shifter


<center> <img src="imagenes/layoutShifter1.png" width= 100% heigth= 100%></center>



## Tarea : mejorar lo hecho en la clase 47



# Column Drop
Column Drop: En este patrón se tiene todo de forma vertical pero a la hora de que va creciendo el contenido empieza a arrojar los contenedores y los reposiciona a la línea principal, secundaria, etc… En este no se limita el crecimiento del container porque queremos que se estire por completo, que ocupe todo el ancho de la pantalla
<center> <img src="imagenes/columndrop.webp" width= 100% heigth= 100%></center>

# Recomendaciones
- mydevice: es una pagina para ver las dimensiones de diferentes dispositivos.
<center> <img src="imagenes/recomendaciones1.png" width= 100% heigth= 100%></center>

# figure y picture
- figure es usado semánticamente, y le dice al navegador que es un contenedor de, ya sea, diagramas, fotos, etc.  Mientras picture ofrece a los desarrolladores más flexibilidad para especificar recursos de imágenes.
- la etiqueta < picture > ofrece a los desarrolladores web más flexibilidad para especificar recursos de imágenes. Esta contiene dos etiquetas: una o más etiquetas < source > y una etiqueta **< img > **

- width: 100% funciona si la imagen es lo suficientemente grande para abarcar el 100% de su contenedor, pero si no, la imagen se pixelara en su intento de cubrir el 100%. max-width: 100% nos ayuda a que la imagen no supere su ancho original, es como decirle a la imagen: Oye tu, estirate para cubrir el 100% de tu contenedor, pero si ves que no llegas y te pixelas, relaja, no te estires mas.
Pdta: el height siempre sera auto, ayudando a que el aspect ratio de la imagen no se dañe

<center> <img src="imagenes/picture1.png" width= 100% heigth= 100%></center>

# Accesibilidad

  - <h3>Textos:</h3>Se recomienda fuertemente usar medidas relativas como rem, para poder incrementar el tamaño del texto para personas con visibilidad disminuida. Las opciones de navegador que cambian el tamaño de las fuentes no funcionan cuando las fuentes de html en el texto están en pixeles (px).
width= 800px heigth= 300px
- El label ayuda a que se pueda enfocar rápidamente en el input del formulario.

- En el atributo alt de la etiqueta img, de debe colocar una descripción rápida de lo que contiene la imagen, ya que esto será leído por el software para accesibilidad auditiva.

- El atributo de title, de la etiqueta img, le agrega una descripción a la imagen cuando el cursor se pone encima de ella.

<center> <img src="imagenes/label.png" width= 100% heigth= 100%></center>

<center> <img src="imagenes/cheats.webp" width= 100% heigth= 100%></center>