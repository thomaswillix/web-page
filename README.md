# Página WEB Lenguajes de Marcas

## Página de Inicio (index.html):

Esta página presenta un \<h1>, un \<p>, y un \<div>.
El \<div> se identifica con su id \#timeline y en él se encuentran diferentes links a las dos páginas que he incluido en esta. Estos links están a modo de imágenes y cada imagen representa a la consola más importante de dicha generación.

### CSS:

\#timeline: he puesto el display como “inline” para que las imágenes aparezcan una al lado de la otra.
\<p>, \<h1>: he añadido un padding de 10% por simple estética.
\<img>: apliqué un margin-left para que se separen un poco las imágenes y no estén pegadas a la izquierda y una width del 10% para que el tamaño de las imágenes se vea igualado en todas.


## Primera Generación (firstgen.html):

> Implementé una \<table> en esta página para que la distribución del título,  las imágenes, el texto y las listas  se me hagan más fáciles.
<p> Dentro de la tabla:

Al \<th> le he puesto un colspan de 2 para que ocupe el 100% de la tabla y así será más fácil de modificar su posicionamiento más tarde con CSS.

En el primer \<tr> puse dos \<td>’s, dentro del primero de ellos  describí  un \<div> con id \#atari, en él puse la primera imagen con una etiqueta de style en la que describí su width al 35%. Lo hice de esta manera porque no la conseguí seleccionar con el selector de clases del header.

El segundo de los dos \<td>’s tiene otro \<div> en el que solo hay un gif a modo de  ejemplo de lo que era el juego del que estoy hablando. Puse una etiqueta de style en la que el width lo establecí al 60%.

A continuación viene el siguiente \<tr> en el que solo hay un \<td>, pero, que posee un colspan de 2 como el del \<th>.

Para acabar con la tabla, en el último \<tr> tiene dos \<td>’s, hay una lista en cada uno y cada una de ellas tiene su padding-left ajustado para un correcto posicionamiento.




Y para acabar con la página simplemente añadí los tres links internos que tengo asociados a imágenes que funcionan a modo de navegación entre el sitio web, “página anterior, inicio y página siguiente”. Estos 3 links están contenidos en un \<div> llamado \#links y cada imagen de cada link tiene un id (\#paginaanterior, \#inicio, \#paginasiguiente).</p>


### CSS:

Los \<td> tienen una width del 50% ya que hay 2 por row. El id \#text tiene un text-align: center por estética, el \<h1> tiene un margen del 4% para posicionarse un poco más abajo y centrado que por defecto y un font-size: xx–large.

La id \#atari presenta un display: grid y place-items center para centrar la primera imagen.


## Quinta Generación (fifth.html):

> Al principio de la página puse un link interno al id \#grafico que aparecerá más tarde asociado al \<h1> de la página.

Como en la anterior página, utilicé una \<table> para que sea más fácil distribuir y manipular los elementos.En el primer \<tr> introduje los títulos como \<td>’s, en el segundo imágenes y en el tercero texto.
Dentro del tercer \<tr>, el primer \<td> tiene primero una etiqueta \<p> que modifiqué con el atributo style para establecer el padding-bottom a unset y seguido de esta una \<ul>
El segundo \<td> tiene la misma estructura que el anterior y los últimos 2 solo poseen una etiqueta \<p> cada uno. 

A continuación de la tabla puse un \<div> en el que hay un \<h1> y un \<a> con name: grafico para ser referenciado en el principio de la página por el link interno, dentro de esta etiqueta de link hay una \<img> con su style cambiado “width:40%”.

Para finalizar con la página, como en la anterior hay un div con los links externos de navegación.

### CSS:

\<img>: width: 40% y margin-left: 30%
\<td>: color: white y width: 25%
\<p> y \<h1>: padding del 5% para posicionarlo
\<div> margin-bottom: 2% para separar un poco los elementos.
\<ul> margin-left: 20% para centrarla un poco más en cada \<td> y el padding: unset.
\<a> color: white y text-decoration: none para que la decoración por defecto del link no aparezca.
a:hover tiene un color: violet para que cambie el color al pasar el ratón por encima del link.


## HOJA DE ESTILOS DE CSS (StyleSheet1.css):

> Esta hoja de estilos es referenciada en todos los .html anteriores.
```css
h1,p:{
font-family: ‘Times New Roman’, Times, serif;  /* Establezco como fuentes de letra predeterminadas estas 3 (si una no
                                                  funciona la siguiente en orden respectivo será la predeterminada) */ 
color: white;                                  /* Simplemente le cambio el color al texto */ 
text-align: center;                            /* Esta propiedad alinea el texto al centro. */ 
font-size: x-large; 
}

ul{
	color: white;                                /* Cambio el color para que cualquier texto de listas sea blanco. */
	font-size: larger;                           /* La fuente será de tamaño larger en todos los textos de listas. */
}

p{
	font-style: italic;                          /* Esto hará que los párrafos tengan su letra cursiva. */
}

body{
	background-color: black;                     /* Cambio el color de fondo de las páginas a negro. */
}

table{
	display: block;                              /* Esto hará que todas las tablas se comporten como un bloque y cualquier
}                                                 elemento que vaya seguido de estas se dispondrá debajo. */

#links{
	margin: 5%; 
}

#inicio, #paginasiguiente, #paginaanterior{
display: inline-block;                         /* Esta propiedad hace que los elementos se muestren en la misma
                                                  línea incluso si tienen distinta altura. */
width: 6%;
}

#inicio:hover, #paginasiguiente:hover,#paginaanterior:hover{
width:8%;
}

#inicio{
   	float: left;                                /* Con esta propiedad consigo que el elemento flote a la izquierda. */
    	margin-left: 40%;                         /* Y aquí establezco un margen para posicionarlo. */
}

#paginasiguiente{
    	float: right;                             /* Con esta propiedad consigo que el elemento flote a la derecha. */
}

#paginaanterior{
    	Float:left;                               /* Con esta propiedad consigo que el elemento flote a la izquierda. */
    	margin-left: unset;                       /* Dejo el margen sin definir para que esté pegado a la izquierda. */
}
```
## INFOGRAFÍA Y FUENTES

Las imágenes de las consolas están sacadas de la wikipedia, el gif de la atari lo encontré por google y el gráfico y las tres imágenes de navegación las he realizado con herramientas online (Canva y OnlineChartsBuilder). La información acerca de las consolas como sus juegos, modelos y ventas está en su mayoría sacada de la wikipedia de cada una de ellas aunque hay datos que ya sabía de antes.
