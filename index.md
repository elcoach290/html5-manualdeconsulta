# Manual del Guerrero HTML5

## Indice

- [Conceptos Básicos](#conceptos-básicos)
	- [Carpeta](#carpeta)
	- [Archivo](#archivo)
	- [Sitio Web](#sitio-web)
	- [Página Web](#página-web)
	- [Dominio](#dominio)
	- [Hosting](#hosting)

- [Hyper Text Markup Language](#hyper-text-markup-language)	
	- [Estructura básica de todo documento HTML5](#estructura-basica-de-todo-documento-html5)
	- [Comentarios](#comentarios)
	- [Elementos](#elementos)
	- [Atributos](#atributos)
	- [Elementos básicos](#elementos-básicos)
		- [Titulares](#titulares-headings)
		- [Párrafos](#párrafos)
		- [Enlaces](#enlaces-anchors)
		- [Imágenes](#imágenes)
		- [Listas](#listas)
		- [Tablas](#tablas)
		- [Otras etiquetas](#otras-etiquetas)
	- [Agrupadores Semánticos](#agrupadores-semánticos)
		- [Nav](#nav)
		- [Header](#header)
		- [Main](#main)
		- [Footer](#footer)
		- [Article](#article)
		- [Section](#section)
		- [Figure](#figure)
	- [El elemento agrupador DIV](#el-elemento-agrupador-div)
	- [Elementos Multimedia](#elementos-multimedia)
	- [Elementos de formulario](#elementos-de-formulario)

- [Estilos CSS](#estilos-css)
	- [Vinculando una hoja de estilos](#vinculando-una-hoja-de-estilos)
	- [Colores](#colores)
	- [Estilos de Texto](#propiedades_de_texto)
	- [Estilos de lista](#estilos-de-lista)
	- [Modelo de Caja](#modelo-de-caja)
	- [Propiedades Flexbox](#propiedades-flexbox)
	- [Imágenes de fondo](#imágenes-de-fondo)
	- [Transiciones](#transiciones)
	- [Animaciones](#animaciones)

## Conceptos Básicos

### Carpeta

Contenedor de archivos que sirve para poder mantenerlos organizados, se recomienda nombrarlos en minusculas y sin espacios en blanco, como ejemplos de nombres de carpetas tenemos: images, videos, css, etc.

### Archivo

Conjunto de informacion digital que puede almacenarse en una computadora, existen diferentes tipos de archivos como las imágenes, videos, audios, texto, etc, y van a requerir una extension que los identifique, como ejemplos tenemos: intro.mp4, musica.mp3, banner.jpg, etc.

### Sitio Web

Conjunto de páginas web interconectadas con un proposito determinado, ejemplo: Sitio Web de Nike, Sitio Web del Poder Judicial, etc.

### Página Web

Documento digital que permite estructurar informacion ( textos, hipertextos ) y contenido multimedia ( video, audio, imágenes, etc )

### Dominio

Es la url o direccion principal en internet donde se encuentra un sitio web.

### Hosting

Espacio en un servidor web para guardar los archivos de un sitio web, normalmente vinculado a un **dominio**.

## Hyper Text Markup Language

El Hyper Text Markup Language ( HTML ) es un lenguaje de marcado o etiquetado que sirve para estructurar la información dentro de una página web, mediante las etiquetas vamos a poder indicar si un texto es un título o un párrafo, si deseamos tener un listado de cierta información también se tiene una etiqueta para este fin.


### Estructura basica de todo documento HTML5

```html
<!doctype html>
<html lang="es">
	<head>
		<meta charset="UTF-8">
		<title>Título de la Pestaña</title>
	</head>
	<body>
	</body>
</html>
```

**TIP:** Les comparto un video sobre este tema:

[![Estructura Básica de un Documento HTML](http://img.youtube.com/vi/Lat2LyZM6Hs/0.jpg)](http://www.youtube.com/watch?v=Lat2LyZM6Hs "Estructura Básica de un Documento HTML")

### Comentarios

Antes de iniciar con los elementos básicos del lenguaje hay que aprender a colocar comentarios dentro de tu código para que te sirvan de recordatorios como notitas donde escribes un texto que te ayude a recordar algún concepto o para que utilizaste tal etiqueta, y además se utilizarán constantemente en los ejemplos.

- Inicio de comentario: `<!--`
- Fin de comentario: `-->`

```html
<!-- Esto es un comentario -->
<!-- Esto es otro comentario 
en dos o 
más líneas -->
```

### Elementos

El lenguaje html está compuesto por elementos que van a ir dandole estructura a una página web. Estos elementos están compuestos generalmente por una etiqueta de apertura y una de cierre, y dependiendo de que trate el contenido se va a utilizar un determinado tipo de elemento.

```html
<p> <!-- etiqueta de apertura para un párrafo -->
Esto es un párrafo.
</p> <!-- etiqueta que indica el fin del párrafo -->

<br> <!-- Elemento para indicar salto de línea, solo requiere la  etiqueta de apertura,
a este tipo de elemento/etiqueta se le conoce como self-closing tag se puede traducir 
como etiqueta de cierre automático -->

``` 

### Atributos

Los atributos son datos adicionales que llevan los elementos en la etiqueta de apertura; los elementos pueden tener más de un atributo mas no tener atributos repetidos. Los elementos **img** necesitan dos atributos a los que se les asigna un valor según corresponda; al atributo **src** se le asigna la ruta del archivo de imagen y al atributo **alt** se le asigna una descripción corta de la imagen:

```html
<html lang="es">
<!-- el elemento html requiere el atributo lang en el cual
se asigna el idioma del documento en este caso es
de español -->

<img src="images/logo.png" alt="Vía Código">

<a href="index.html">Ir a Página de Inicio</a>
<!-- los enlaces necesitan el atributo href para indicar
la ruta del archivo destino al que te va llevar -->
```

### Elementos básicos

#### Titulares (Headings)

Son los encabezados o títulos que usaremos en nuestro documento existen del **h1** al **h6**, siendo el mas importante el **h1** y asi va bajando hasta el **h6** que es el menor importante.

```html
<h1>El título mas importante del documento</h1>
<h2>El título de un segundo nivel de importancia </h2>
...
<h6>El título menos importante</h6>
```

#### Párrafos (Paragraphs)

Cuando necesitamos escribir párrafos el texto lo colocamos dentro de la etiquetas `<p></p>`

```html
<p>Todo lo que necesitas para lograr tus objetivos ya está en ti.</p>
<p>
No vas a dominar el resto de tu vida en un día. Relájate. 
Domina el día. Entonces sigue haciendo eso todos los días.
</p>
```

#### Enlaces (Anchors)

Los enlaces nos van a permitir conectar una página web  con otra, la página destino puede ser del mismo sitio o de otro, también podemos colocar como destinos de los enlaces imágenes o documentos como pdfs. Normalmente dentro del enlace va un texto pero también podría ser una imagen.

```html
<!-- enlace a la página home del sitio -->
<a href="index.html">Ir al Home</a>
<!-- enlace a un id específico dentro de una web -->
<a href="#id-a-visitar">Ir a sección</a> <!-- en la página actual -->
<a href="seccion/#id-a-visitar">
	Ir a sección
</a> <!-- en otra página de la misma web -->
<a href="http://webdeotracosa.com/seccion/#id-a-visitar">
	Ir a sección
</a> <!-- en otra página de internet -->
<!-- enlace para visualizar un archivo pdf -->
<a href="curriculum.pdf">Ver curriculum</a>
<!-- enlace para visualizar una imagen -->
<a href="images/fotogrande.jpg">Ver foto</a>
<!-- enlace para ir dirigirnos a otro sitio -->
<a href="http://www.google.com">Ir a Google</a>
```
**TIP:** Si deseas que el destino se abra en otra pestaña del navegador le añades el atributo **_target_** con el valor **__blank_**

```html
<a href="http://facebook.com" target="_blank">
	Este enlace abrirá en otra pestaña
</a>
``` 

#### Imágenes

Podemos vincular imágenes de distintos tipos en nuestras páginas web usando el elemento **img**:

```html
<img src="images/foto.jpg" alt="Foto de Perfil">
```

Requieren de dos atributos, **src** para indicar la ubicacion de la imagen y **alt** que es para indicar un texto alternativo en casos la imagen por algun motivo no se haya descargado, tambien sirve para la accesibilidad, muy importante para los usuarios invidentes. Recordemos que podemos cargar muchos formatos de imagen, como son JPG, PNG y GIF

**TIP:** A las imágenes se les puede añadir el atributo **width** y dale un valor númerico para indicar su anchura en pixeles, pero se recomienda no usar imágenes muy grandes pues tu página web pesaría mucho, en ese caso se podría editar con Photoshop.

```html
<img src="images/foto.jpg" alt="Foto de Perfil" width="200">
```

#### Listas

Las listas se utilizan cuando requieres mostrar una secuencia de datos o elementos, basicamente hay dos tipos de listas, ordenadas y desordenadas.

##### Listas ordenadas

En ellas importa el orden de los elementos podrían ser los pasos para realizar un tramite.

```html
<ol>
	<li>Acudir al Banco de la Nación</li>
	<li>Pedir el concepto 1810</li>
	<li>Pagar S/ 98.50 por el pasaporte biométrico.</li>
	<li>Ingresar a www.migraciones.gob.pe</li>
	<li>Llenar el formulario </li>
	<li>Separar una cita.</li>
	<li>El pasaporte será entregado en las 14 sedes de Migraciones. 
		Debe llevar su voucher y DNI, no es necesario una foto.</li>
</ol>
```

##### Listas no ordenadas

En ellas no es relevante el orden de los elementos y se pueden tener otras etiquetas incluso, como en el caso de un listado de enlaces:

```html
<ul>
	<li><a href="index.html">Inicio</a></li>
	<li><a href="servicios.html">Servicios</a></li>
	<li><a href="contacto.html">Contacto</a></li>
</ul>
```

**TIP:** Les comparto un video sobre los elementos básicos:



#### Tablas

Es para mostrar datos tabulares o datos extraidos mediante alguna consulta a una base de datos, por ejemplo datos de los usuarios.

```html
<table>
	<thead>
		<tr>
			<td>Código</td>
			<td>Nombre</td>
			<td>Area</td>
			<td>Cargo</td>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>201801</td>
			<td>Manuel Donayre</td>
			<td>Recursos Humanos</td>
			<td>Jefe de Area</td>
		</tr>
		<tr>
			<td>201801</td>
			<td>Jordy Leomine</td>
			<td>Sistemas</td>
			<td>Jefe de Area</td>
		</tr>
		<tr>
			<td>201801</td>
			<td>Marcos Llunas</td>
			<td>Comedor</td>
			<td>Cocinero principal</td>
		</tr>
	</tbody>
</table>
```

#### Otras etiquetas

##### Br

Se usa para romper la línea, en otras palabras forzar el cambio de línea cuando se quiere un texto debajo de otro.

```html
<h1>El Pez <br> Espada </h1> <!-- la palabra espada pasará
a una segunda línea -->
```

**TIP:** No es bueno abusar de esta etiqueta para agregar espaciados pues esto se puede controlar con css.

##### Strong

Nos sirve para indicar que un texto o palabra es importante:

```html
<p>
	El personaje de Tony Stark es caracterizado 
	por el actor <strong>Robert Downey Jr.</strong>
</p>
```

##### Span

Esta etiqueta sirve para poder cambiar el formato a una palabra o caracter sin que esto afecte su significado, el cambio recien se hace visible aplicando estilos css

```html
<h2><span>Gatotel</span>, un lugar para quedarse.</h2>
```

##### Blockquote

Sirve para citar a un texto de un tercero , que no es de nuestra propia autoría.

```html
<blockquote>
	<p>La genialidad es 1% de inspiración y 99% de transpiración</p>
</blockquote>
```

Para indicar el nombre del autor se puede usar la etiqueta `<cite></cite>`y si se quiere indicar la url de la fuente se puede usar el atribute cite de esta forrma:

```html
<blockquote cite="http://www.thomasalva.com">
	<p>La genialidad es 1% de inspiración y 99% de transpiración</p>
	<cite>Thomas Alva Edison</cite>
</blockquote>
```

## Agrupadores semánticos

Estos elementos propios de HTML5 ayudan a los navegadores y crawlers a entender el significado e intención de las partes del código de una web.
Podemos no utilizarlos, pero hacerlo ayuda a que nuestra página sea entendida con mayor facilidad.

### Nav

Para envolver a la lista de enlaces de navegacion de un sitio web.

```html
<nav>
    <ul>
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Nosotros</a></li>
        <li><a href="#">Portafolio</a></li>
        <li><a href="#">Contacto</a></li>
    </ul>
</nav>
```

### Header

Para envolver a los elementos de la cabecera de una página web o sección, pudiendo ser estos el `<h1></h1>` y el `<nav></nav>`.

```html
<header>
	<h1>
		<a href="index.html">
			<img src="images/logo.svg" alt="Gatotel">
		</a>
	</h1>
	<nav>
		<ul>
			<li><a href="#">Inicio</a></li>
			<li><a href="#">Servicios</a></li>
			<li><a href="#">Habitaciones</a></li>
			<li><a href="#">Reservaciones</a></li>
		</ul>
	</nav>
</header>
```

### Main

Dentro del elemento **main** irá todo el contenido principal de la página web. Solo puede haber una etiqueta **main** por página.

```html
<main>
	<!-- dentro de main irá  el contenido principal-->
	<h2>Bienvenidos</h2>
	<p>Este es un mensaje de bienvenida</p>
	...
</main>
```

### Footer

Representa al pie de la página o sección, normalmente van datos de contacto, enlaces a otras páginas de navegación o enlaces a las redes sociales.

```html
<footer>
	<p>
		Copyright 2018 - Diseño y Desarrollo por 
		<a href="http://www.anthonystudio.com">anthonystudio.com</a>
	</p>
</footer>
```

### Article

Se usa envolver a una composición de elementos con datos que hacen referencia a una idea o información autónoma. Un uso común puede ser como entrada de blog, noticia de periódico, ficha técnica de algún producto, etc. Debe tener como mínimo un título y párrafos.

```html
<article>
	<h2>Perú en alerta epidemiológica</h2>
	<p>
		En dos semanas hay más de 30 afectados confirmados,
	 	cuatro de ellos en Lima ...
	 </p>
	<img src="images/foto.jpg" alt="Afectados por el virus">
</article>
```

### Section

Se usa para envolver información que habla sobre un tema en particular o un area de información dentro del documento, podría usarse para envolver a un conjunto de **articles**, debe llevar un título.

```html
<section>
	<h2>Blog</h2>
	<article>
		...
	</article>
	<article>
		...
	</article>
	...
</section>
```

### Figure

Se usa para envolver imágenes, gráficos o fragmentos de código, pueden incluir la etiqueta `<figcaption></figcaption>`para añadirle un título o descripción. Al incluir las imágenes dentro de un elemento este la hace reubicable e independiente pudiendo localizarse en cualquier parte de la página sin afectar el esquema del documento.

```html
<figure>
	<img src="images/foto.jpg" alt="Afectados por el virus">
	<figcaption>Afectados por el síndrome Guillaín Barré</figcaption>
</figure>
```
## El elemento agrupador DIV

Se usa para agrupar otros elementos con fines de adaptar la disposición de estos al diseño de la interfaz, no aporta semántica. Se usa como elemento *comodín*. Por defecto se comporta como un elemento de tipo bloque.

```html
<article>
	<h2>Juntos como hermanos</h2>
	<div>
		<p>Juntos como hermanos <br>
		Miembros de una iglesia <br>
		Vamos caminando <br>
		Al encuentro del señor </p>
		
		<p>Un largo caminar <br>
		Por el desierto bajo el sol <br>
		No podemos avanzar <br>
		Sin la ayuda del señor</p>
	</div>
	<div>
		<img src="images/hermanos.jpg" alt="Juntos como hermanos">
	</div>
</article>
```

## Elementos Multimedia

Con HTML5 ahora podemos incluir videos y audio.

### Video

De esta forma podríamos incluir un video dentro de nuestro sitio web
```html
<video src="videos/intro.mp4" controls></video>
```

El atributo src es para indicar la ubicación del video mientras el atributo controls permite mostrar los controles de reproducción, otros atributos opcionales son: 
* poster: muestra una imagen como carátula del video (hay que pasarle una URL)
* preload: define si el video debe comenzar a cargarse en cuanto carga la página o no 
* height: altura en pixels del video
* autoplay: define si el video debe comenzar a verse en cuanto haya cargado
* muted: define si debe silenciarse el video de forma automática
* controls: define si los controles de video deben mostrarse o no (pausa, play)

### Audio

De esta forma podríamos incluir un audio o sonido dentro de nuestro sitio web
```html
<video src="audios/sound.mp4" controls></video>
```
El atributo src es para indicar la ubicación del archivo de audio mientras el atributo controls permite mostrar los controles de reproducción, si se desea iniciar automáticamente se le puede añadir el atributo autoplay.

## Elementos de formulario

### Form
Este  elemento sirve para envolver a o agrupar todos los campos del formulario, es el formulario en sí.

```html
<form action="process.php" method="POST">
	...
</form>
```

Por lo general tienen un atributo action que hace referencia la ruta(URL) que se va encargar de procesar los datos ingresados y el atributo method que es indica la forma en que se va enviar para caso de formularios de contacto sería el valor **POST**, los formularios web solo soportan los métodos POST y GET, siendo GET el método por defecto.

### Label

Esta etiqueta siempre acompaña a los campos de entrada así sabemos que dato queremos ingresar en dicho campo.

```html
<label for="username">Nombre:</label>
<input type="text" id="username">
```
**TIP:** con el atributo **_for_** vinculamos el label a su input correspondiente y usamos el atributo **_id_** del input
 
### Input

Son los campos de entrada de datos, existen varios tipos entre ellos tenemos: text, email, radio, checkbox, color, date, etc.  

```html
<!-- Este campo es para ingreso de textos cortos de una sola línea -->
<input type="text">
<!-- Este campo es para ingreso de correos electrónicos -->
<input type="email">
<!-- Este tipo de campo para cuando tenemos varias alternativas 
a seleccionar pero solo una podemos marcar -->
<input type="radio">
<!-- Este tipo de campo para cuando tenemos que marcar una o varias alternativas de un conjunto de opciones -->
<input type="checkbox">
<!-- Este tipo de campo para cuando tenemos que ingresar número, algunos navegadores pueden mostrar unas flechas para aumentar o reducir el valor -->
<input type="number">
```
### Textarea

Este elemento es para cuando requerimos ingresar un texto multilínea podría ser en caso de escribir un comentario o consulta

```html
<textarea></textarea>	
```

### Select

Este elemento es para cuando requerimos seleccionar una opción (usando la etiqueta option) de un conjunto de opciones.

```html
<select>
	<option value="0">Seleccione una Ciudad</option>
	<option value="1">Arequipa</option>
	<option value="2">Cuzco</option>
	<option value="3">Lima</option>
	<option value="4">Trujillo</option>
</select>	
```

### Button

Este elemento nos va servir básicamente para poder envíar el formulario aunque también podría enviarse presionando la tecla **ENTER** debe tener un atributo **_type_** con el valor de **_submit_**

```html
<button type="submit">Enviar</button>
```

**TIP:** A los campos de entrada podemos añadirle un atributo **_required_** que los convierte en campos obligatorios, y también un atributo **_placeholder_** con el valor que desees se muestre dentro del campo cuando no se ha ingresado nada aún, a modo de guía de como se podría llenar.

```html
<input type="email" placeholder="anthony@prodesigner.com" required>
``` 


## Estilos CSS

Para poder dar formato a nuestros documentos HTML vamos a usar el Lenguaje CSS el cual nos permitirá personalizar colores, tipografías, espaciados, diagramación etc.

### Vinculando una hoja de estilos

Para vincular una hoja de estilos debemos incluir dentro del elemento **head** el elemento **link** que nos va permitir conectar ambos archivos ( el html con el css ).

```html
<head>
	<link href="css/style.css" rel="stylesheet"> <!-- ambos atributos son obligatorios -->
</head>
```

Antes de iniciar con las reglas css  hay que aprender a colocar comentarios dentro de tu hoja de estilos para que te sirvan de recordatorios como notitas donde escribes un texto que te ayude a recordar porqué hiciste algo o para que utilizaste tal propiedad, y además se utilizarán constantemente en los ejemplos. Nunca te olvides de cerrar los comentarios:

- Inicio de comentario: `/*`
- Fin de comentario: `*/`

```css
/* Esto es un comentario en css */
/* 
Esto es
otro comentario
en multiples lineas
*/
```

### Colores

Para aplicar colores se pueden usar hacer referencia a estos de  diferentes formas, 
mediante el nombre del color en inglés, por ejemplo para el color negro podemos usar la palabra **black**, 
para el color rosado, la palabra **pink**, etc. 
También se puede usar el formato hexadecimal siendo **#ff0000** para el color rojo,  **#000000** para el color negro. 
El formato rgba que permite añadir un canal alfa que controla el nivel de transparencia,
 **rgba(0,0,0,0.5)** sería para un color negro semi transparente, a un nivel de transparencia del cincuenta por ciento.

 ```css
 .title{
	color: orange; /* aplicamos color naranja al texto */
	border-bottom: solid 5px #ff9900; /* aplicamos un borde inferior de color naranja */
	background-color: rgba(0,0,0,0.8); /* aplicamos color negro
	con ochenta por ciento de opacidad al fondo */
}
 ```

### Propiedades de texto

Entre las propiedades para dar formato al texto tenemos:

#### Font-size

Esta propiedad sirve para indicar el tamaño que van a tener los textos dentro del documento, 
pudiendo tener valores absolutos como 16px y relativos como: 1.2em o 120%.

```css
.header__title{
  font-size: 31px;
}

.footer{
	font-size: 0.8em; /* equivale a 12.8 pixeles (0.8*16) si el tamaño de letra base es 16 pixeles */
}

.the_title{
	font-size: 300%; /* equivale a 48px (16*3) si el tamaño de letra base es de 16px */
}

```

#### Text-align

Sirve alinear el contenido en línea de los bloques, pudiendo ser estos textos, __elementos inline__ y __elementos inline-block__, por ejemplo: enlaces, imágenes, etc.

```css
.intro{
	text-align: center; /* otros valores posibles son: left, right, center, justify */
}
```

- **left:** alineación a la izquierda (por defecto).
- **center:** alineación al centro.
- **right:** alineación a la derecha.
- **justify:** alineación justificada de textos.

#### Line-height

Sirve para precisar el alto que van a tener las líneas de texto o el interlineado. Los valores pueden ser absolutos o relativos (se recomiendan relativos).

```css
p{
	line-height: 1.3; /* equivale al 130% de la altura del texto */
}

h1, h2, h3 {
	line-height: 120%; /* es el porcentaje de la altura del texto */
}

```

#### Text-decoration

Es la propiedad para añadir detalles decorativos al texto.

```css
a{
  text-decoration: none; /* quita subrayado a todos los enlaces de la página, pues estos vienen con un subrayado por defecto */
}

.post__price{
  text-decoration:line-through; /* agrega una línea horizontal
  a la mitad del texto  a modo de tachado */
}

.post__category{
  text-decoration: underline; /* subraya el texto */
}
```





### Estilos de lista

Las listas tiene propiedades que permite cambiar el aspecto de las viñetas la numeración.

#### List-style-type

Esta propiedad permite cambiar la viñeta o numeración de una lista ordenada o desordenada.

```css
ul{
	list-style-type: none; /* quita la viñeta */
}
```
Otros valores que puede aceptar la propiedad son: disc, circle, square, decimal, decimal-leading-zero, lower-roman, upper-roman, lower-greek, lower-latin, upper-latin, armenian, georgian, lower-alpha, upper-alpha. Te sugiero que los pruebes para que veas los resultados.

#### List-style-position

Esta propiedad controla la ubicación de la viñeta con respecto al elemento de la lista.

```css
ul{
	list-style-position: inside; /* coloca la viñeta
	dentro del elemento */
}
```

#### List-style-image

Esta propiedad permite colocar una imagen en vez de viñeta o numeración.

```css
ul{
	list-style-image: url("../images/diamond.png");
}
```
Por defecto el valor es **outside** fuera del elemento de la lista.

**TIP:** la propiedad **list-style** permite resumir las tres propiedades en una sola:

```css
ul{
	list-style: square inside; /* viñeta cuadrada y dentro del elemento */
}
```


### Modelo de caja

Sirve para comprender las diferentes propiedades que afectan al tamaño y disposición de una caja.

![Modelo de caja](/images/boxmodel.gif)

#### Content (contenido): 

Contenido de la caja el cual podría tener un texto, una imagen, u otros elementos, 
se le puede definir anchura con la propiedad **width** y altura con la propiedad **height**.

```css
.box{
	width: 800px; /* ancho de 800 pixeles */
	/* de preferencia es mejor no aplicar height y dejar que lo que 
	va dentro le de la altura con su propio volumen */
	height: 600px; 
}
```

#### Padding (relleno):

Es la distancia del contenido de la caja hacia dentro del contenedor.
```css
.box{
	padding-right: 5px; /* distancia hacia el lado derecho. */
	padding-left: 5px; /* distancia hacia el lado izquierdo. */
	padding-top:5px; /* distancia hacia arriba. */
	padding-bottom: 5px; /* distancia hacia abajo. */
}
```
**TIP:** Si deseas ahorrar líneas de código puedes aplicar esto:
```css
.box{
	padding: 5px 10px; /* el primero es para el right y left, el segundo es para el top y bottom */ 
}
```

#### Margin (margen):

Es la distancia de la caja hacia afuera del contenedor.

```css
.box{
	margin-right: 5px; /* distancia hacia el lado derecho */
	margin-left: 5px; /* distancia hacia el lado izquierdo */
	margin-top: 5px; /* distancia hacia arriba */
	margin-bottom: 5px; /* distancia hacia abajo */
}
```

**TIP:** Si deseas centrar una caja horizontalmente puedes usar este pequeño truco.

```css
.box{
	width: 800px; /* aplicarle un ancho, también funciona con max-width */
	margin-left: auto; /* el valor auto para equilibrar el lado izquierdo */ 
	margin-right: auto; /* con el lado derecho  */
}
```

#### Border (borde):

Trazo o línea de contorno, podrías usar las propiedades:

```css
.box{
	border-style: solid; /* estilo de linea */
	border-color: black; /* color de borde */
	border-width: 10px; /* grosor del trazo */
	border-radius: 5px; /* radio del borde */
}
```
**TIP:** si deseas ahorrar escritura en el border-style, border-width y border-color puedes usar este __shorthand__ (atajo de escritura)

```css
.box{
	border: solid 5px black; /* style width color */
}
```

**TIP:** Si deseas  que el padding y border respeten el tamaño de la caja,
 en otras palabras el tamaño de la caja lo defina el width del content, 
 puedes usar esta propiedad:

```css
.box{
	box-sizing: border-box;
}
```

### Propiedades flexbox

#### Display

A esta propiedad le asignamos un valor **flex** o **flex-inline** (es lo menos común) 
dependiendo de la necesidad en tu diagramación. 
Al darle este valor permite disponer de un modo más fácil a todos sus hijos directos.
Por defecto lo que va pasar es que todos sus hijos se acomoden de forma horizontal 
uno al lado del otro.

```css
.menu{
  display: flex;
}
```

#### Justify-content

La propiedad **justify-content** sirve para alinear a los elementos hijos cuando 
estos no usan todo el espacio disponible en el eje principal 
(por defecto es el horizontal).

```css
.menu{
  display: flex;
  justify-content: flex-start; /* otros valores posibles son: flex-end, center,  space-between, space-around, space-evenly */
}
```

- **flex-start:** Alinea elementos al lado izquierdo del contenedor.
- **flex-end:** Alinea elementos al lado derecho del contenedor.
- **center: **Alinea elementos en el centro del contenedor.
- **space-between:** Muestra elementos con la misma distancia entre ellos.
- **space-around:** Muestra elementos con la misma separación alrededor de ellos.

#### Align-items

Esto define el comportamiento predeterminado de cómo se colocan los elementos hijos a lo largo
del eje transversal en la línea actual (por defecto es el eje vertical). 
Es como la versión de **justify-content** para el eje transversal (perpendicular al eje principal).

```css
div{
  display: flex;
  align-items: flex-start; /* otros valores posibles son: flex-end, center, baseline, stretch */
}
```
- **flex-start:** Alinea elementos hijos a la parte superior del contenedor padre.
- **flex-end:** Alinea elementos hijos a la parte inferior del contenedor padre.
- **center:** Alinea elementos hijos en el centro (verticalmente hablando) del contenedor padre.
- **baseline:** Muestra elementos hijos en la línea base del contenedor padre.
- **stretch:** Elementos hijos se estiran para ajustarse al contenedor padre.


#### Flex-direction

Esto establece el eje principal, definiendo así la dirección en que se colocan los 
elementos hijos  en el contenedor padre.

```css
.menu{
  display: flex;
  flex-direction: row; /* otros valores posibles son: row-reverse, column,  column-reverse */
}
```
- **row:** Elementos son colocados en la misma dirección del texto.
- **row-reverse:** Elementos son colocados en la dirección opuesta al texto.
- **column:** Elementos se colocan de arriba hacia abajo.
- **column-reverse:** Elementos se colocan de abajo hacia arriba.

#### Flex-wrap

Por defecto, todos los elementos hijos  intentarán caber en una línea. 
Puede cambiar eso y permitir que pasen a una segunda fila (si fuera necesario) 
con esta propiedad.

```css
.posts{
  display: flex;
  flex-wrap: nowrap; /* otros valores: wrap, wrap-reverse */
}
```
- **nowrap:** Cada elemento se ajusta en una sola línea.
- **wrap:** los elementos se envuelven alrededor de líneas adicionales.
- **wrap-reverse:** Los elementos se envuelven alrededor de líneas adicionales en reversa.


### Imágenes de Fondo

#### Background-image

Sirve para establecer la imagen de fondo de un elemento. 
La imagen se muestra en la zona que ocupan el contenido y el relleno del elemento,
justo hasta su borde.

Para indicar la imagen que se muestra como fondo de un elemento, se utiliza una URL. 

```css
body{
  background-image: url("../images/fondo.jpg");
}
```

#### Background-size

Esta propiedad se utiliza para determinar el tamaño de la imagen de fondo, 
estableciendo ancho y alto de la misma.

```css
body{
  background-image: url("../images/fondo.jpg");
  Background-size: 300px 200px; /* otros valores: 50% 50%, cover */
}
```
**TIP:** si se le asigna el valor **cover** la imagen cubrirá todo el area disponible, 
muy util para cuando queremos que se adapte a diferentes tamaños de pantalla o dispositivo.

#### Background-attachment

Esta propiedad sirve para controlar si la imagen de fondo se mueve o permanece fija cuando se 
hace scroll en la ventana del navegador. 

- **Scroll:** Es el valor base y consiste en que la imagen de fondo se mueve con el elemento.

- **Fixed:** Consiste en que la imagen de fondo permanece fija cuando se hace scroll en la ventana del navegador.

```css
body {
  background-image: url("../images/fondo.jpg");
  background-attachment: fixed;
}
```

#### Background-repeat

Esta propiedad sirve para controlar el tipo de repetición de las imágenes de fondo, 
si se repite o no y las direcciones en las que se repite. Se pueden usar solo uno de 
los siguientes valores permitidos a la vez: repeat, repeat-x, repeat-y ó no-repeat.

Por defecto, si la imagen de fondo que se establece con la propiedad background-image es 
más pequeña que el sitio disponible, el navegador repite la imagen en todas 
las direcciones hasta cubrir completamente la superficie del elemento.
```css
body {
  background-image: url("../images/patron.jpg");
  background-repeat: no-repeat;
}
```


Los valores repeat-x y repeat-y permiten repetir la imagen de fondo sólo en una 
dirección (horizontal o vertical).
```css
body {
  background-image: url("../images/patron.jpg");
  background-repeat: repeat-x;
}
```

#### Background-position

Esta propiedad se utiliza para controlar la posición de las imágenes de fondo.

```css
body{
	background-image: url("../images/flower.png");
	background-repeat: no-repeat;
	background-position: 10px 30px;
}
```
La explicación de los valores permitidos para esta propiedad es compleja debido a su gran flexibilidad. 
Son dos valores separados por un espacio.

- En el primer valor se puede escribrir: un porcentaje,  medida exacta en pixeles, left, center ó right.
- En el segundo valor se puede escribir: un porcentaje, medida exacta en pixeles, top, center ó bottom.
- Si se utilizan porcentajes, hace referencia a la anchura del propio elemento.

También podrías aplicar:
- En el primer valor: left, center ó right.
- En el segundo valor: top, center ó bottom.

Entonces si deseamos una imagen alineada en la parte derecha inferior sería:

```css
.header{
	background-image: url("../images/petunia.png");
	background-repeat: no-repeat;
	background-position: right bottom;
}
```

### Transiciones

Para añadir transiciones se usan las siguientes propiedades:

- **Transition-property:** Esta propiedad sirve para indicar el nombre de la propiedad que se desea transicionar.
- **Transition-duration:** Esta propiedad sirve para indicar el tiempo que se quiere que dure la transición.
- **Transition-delay:** Esta propiedad sirve para indicar una latencia o retardo para que inicie la transición.
- **Transition-timing-function:** Esta propiedad sirve para indicar si se desea aceleración o un 
movimiento linear (sin aceleración).

```css
.btn{
	background-color: red;
	color: white;		
	transition-property: background-color;
	transition-duration: 200ms;
	transition-delay: 50ms;
	transition-timing-function: linear;	
}

/* básicamente las transiciones para poder ver el cambio de propiedad con 
transicion se tiene que usar en la pseudoclase hover */

.btn:hover{
	background-color: black;
}
```

**TIP:** Las propiedades __transicionables__ son aquellas que tienen valores númericos, por ejemplo: margin, padding, background-color, color, width, height, transform, etc.

### Animaciones

Las animaciones requieren el uso de la regla **keyframes** a la cual se le asigna un nombre y donde se indican las propiedades a interpolar o animar y estás se agrupan en dos o mas grupos dependiendo de cuantos requiera la animación, estos grupos se le asigna un valor porcentual para indicar en que punto de la animación va tener dichas propiedades el elemento a animar. Una vez creada la regla se le asigna al elemento usando la propiedad **animation-name**, **animation-duration**. Otras propiedades opcionales son **animation-iteration-count**, **animation-direction**, **animation-timing-function**, **animation-fill-mode** y **animation-play-state**.

```css
/* se crea la regla keyframes */
@keyframes rotacion{
	0%{
		transform: rotate(0deg);
	}
	100%{
		transform: rotate(360deg);
	}
}
/* se asigna la regla al elemento que se desea animar */

.wheel{
	animation-name: rotacion; /* nombre de la regla keyframes */
	animation-duration: 300ms; /* tiempo que va durar la animación */
	animation-iteration-count: infinite; /* las veces que se va repetir
	 la animación podría ser una vez, dos, tres o de forma infinita */
	animation-timing-function: linear; /* para un movimiento con
	velocidad constante o linear */
}

```







