# Manual del Guerrero HTML5

## Indice

- [Conceptos Basicos](#conceptos-basicos)
	- [Carpeta](#carpeta)
	- [Archivo](#archivo)
	- [Sitio Web](#sitio-web)
	- [Pagina Web](#pagina-web)
	- [Dominio](#dominio)
	- [Hosting](#hosting)

- [Hyper Text Markup Language](#hyper-text-markup-language)	
	- [Estructura básica de todo documento HTML5](#estructura-basica-de-todo-documento-html5)
	- [Elementos básicos](#elementos-básicos)
		- [Titulares](#titulares-headings)
		- [Parrafos](#parrafos)
		- [Enlaces](#enlaces-anchors)
		- [Imagenes](#imagenes)
		- [Listas](#listas)
		- [Tablas](#tablas)
		- [Otras etiquetas](#otras-etiquetas)
	- [Agrupadores Semánticos](#agrupadores-semánticos)
		- [Nav](#Nav)
		- [Header](#Header)
		- [Main](#Main)
		- [Footer](#Footer)
		- [Article](#Article)
		- [Section](#Section)
		- [Figure](#Figure)
	- [El elemento agrupador DIV](#El_elemento_agrupador_DIV)
	- [Elementos Multimedia](#Elementos_multimedia)
	- [Elementos de formulario](#Elementos_de_formulario)

- [Estilos CSS](#Estilos_CSS)
	- [Colores](#Colores)
	- [Estilos de Texto](#Propiedades_de_texto)
	- [Estilos de lista](#Estilos_de_lista)
	- [Modelo de Caja](#Modelo_de_caja)
	- [Propiedades Flexbox](#Propiedades_flexbox)
	- [Imagenes de fondo](#Imagenes_de_fondo)
	- [Transiciones](#Transiciones)
	- [Animaciones](#Animaciones)

## Conceptos Basicos

### Carpeta

Contenedor de archivos que sirve para poder mantenerlos organizados, se recomienda nombrarlos en minusculas y sin espacios en blanco, como ejemplos de nombres de carpetas tenemos: images, videos, css, etc.

### Archivo

Conjunto de informacion digital que puede almacenarse en una computadora, existen diferentes tipos de archivos como las imagenes, videos, audios, texto, etc, y van a requerir una extension que los identifique, como ejemplos tenemos: intro.mp4, musica.mp3, banner.jpg, etc.

### Sitio Web

Conjunto de páginas web interconectadas con un proposito determinado, ejemplo: Sitio Web de Nike, Sitio Web del Poder Judicial, etc.

### Pagina Web

Documento digital que permite estructurar informacion ( textos, hipertextos ) y contenido multimedia ( video, audio, imagenes, etc )

### Dominio

Es la url o direccion principal en internet donde se encuentra un sitio web.

### Hosting
Espacio en un servidor web para guardar los archivos de un sitio web, normalmente vinculado a un **dominio**.

## Hyper Text Markup Language

El Hyper Text Markup Language ( HTML ) es un lenguaje de marcado o etiquetado que sirve para estructurar la información dentro de una página web, mediante las etiquetas vamos a poder indicar si un texto es un título o un párrafo, si deseamos tener un listado de cierta información también se tiene una etiqueta para este fin.

Antes de iniciar con los elementos básicos del lenguaje hay que aprender a colocar comentarios dentro de tu código para que te sirvan de recordatorios como notitas donde escribes un texto que te ayude a recordar algún concepto o para que utilizaste tal etiqueta, y además se utilizarán constantemente en los ejemplos.

- Inicio de comentario: `<!--`
- Fin de comentario: `-->`

```html
<!-- Esto es un comentario -->
<!-- Esto es otro comentario 
en dos o 
más líneas -->
```

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

Cuando necesitamos escribir parrafos el texto lo colocamos dentro de la etiquetas `<p></p>`

```html
<p>Todo lo que necesitas para lograr tus objetivos ya está en ti.</p>
<p>
No vas a dominar el resto de tu vida en un día. Relájate. 
Domina el día. Entonces sigue haciendo eso todos los días.
</p>
```

#### Enlaces (Anchors)

Los enlaces son los que nos van a permitir conectar las paginas de nuestro sitio o conectarlas con otras paginas externas, tambien podemos colocar como destinos de los enlaces imagenes o documentos como pdfs.

```html
<!-- enlace a la pagina home del sitio -->
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

#### Imagenes

Podemos vincular imagenes de distintos tipos en nuestras paginas web para que se puedan visualizar al momento de visualizarse de la siguiente manera:

```html
<img src="images/foto.jpg" alt="Foto de Perfil">
```

Requieren de dos atributos, **src** para indicar la ubicacion de la imagen y **alt** que es para indicar un texto alternativo en casos la imagen por algun motivo no se haya descargado, tambien sirve para la accesibilidad, muy importante para los usuarios invidentes. Recordemos que podemos cargar muchos formatos de imagen, como son JPG, PNG y GIF

**TIP:** A las imagenes se les pueñe añadir el atributo **width** y dale un valor númerico para indicar su anchura en pixeles, pero se recomienda no usar imagenes muy grandes pues tu página web pesaría mucho, en ese caso se podría editar con Photoshop.

```html
<img src="images/foto.jpg" alt="Foto de Perfil" width="200">
```

#### Listas

Las lista se utilizan cuando requieres mostras una secuencia de datos o elementos, pueden ser ordenadas o desordenadas.

##### Listas ordenadas

En ellas importa el orden de los elementos podrian ser los pasos para realizar un tramite.

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

#### Tablas

Es para mostras datos tabulares o datos extraido mediante alguna consulta a una base de datos, pudiendo ser estos registros, por ejemplo datos de los usuarios.

```html
<table>
	<thead>
		<tr>
			<td>Codigo</td>
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

##### Strong

Nos sirve para indicar que un texto o palabra es importante:

```html
<p>
	El personaje de Tony Stark es caracterizado 
	por el actor <strong>Robert Downey Jr.</strong>
</p>
```

##### Span

Esta etiqueta sirve para poder cambiar el formato a una palabra a caracter sin que esto afecte su significado, el cambio recien se hace visible aplicando estilos css

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

## Agrupadores semanticos

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

Para envolver a los elementos de la cabecera de una pagina web o seccion, pudiendo ser estos el `<h1></h1>` y el `<nav></nav>`.

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

Representa al pie de la página o sección, normalmente van datos de contacto, enlaces a otras paginas de navegacion o enlaces a las redes sociales.

```html
<footer>
	<p>
		Copyright 2018 - Diseño y Desarrollo por 
		<a href="http://www.anthonystudio.com">anthonystudio.com</a>
	</p>
</footer>
```

### Article

Se usa envolver a una composición de elementos con datos que hacen referencia a una idea o información autonónoma. Un uso común puede ser como entrada de blog, noticia de periódico, ficha técnica de algún producto, etc. Debe tener como mínimo un título y párrafos.

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

Se usa para envolver imágenes, gráficos o fragmentos de código, pueden incluir la etiqueta `<figcaption></figcaption>`para añadirle un título o descripción. Al incluir las imagenes dentro de un elemento este la hace reubicable e independiente pudiendo localizarse en cualquier parte de la página sin afectar el esquema del documento.

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
El atributo src es para indicar la ubicación del archivo de audio mientras el atributo controls permite mostrar los controles de reproducción, si se desea iniciar automaticamente se le puede añadir el atributo autoplay.

## Elementos de formulario

### Form
Este el elemento es el que va envolvera o agrupar todos los campos del formulario, es el formulario en sí.

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
<!-- Este campo es para ingreo de correos electrónicos -->
<input type="email">
<!-- Este tipo de campo para cuando tenemos varias alternativas 
a selecionar pero solo una podemos marcar -->
<input type="radio">
```
### Textarea
Este elemento es para cuando requerimos ingresar un texto multilínea podría ser en caso de escribir un comentario o consulta

```html
<textarea></textarea>	
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
 **rgba(0,0,0,0.5)** sería para un color negro semi transparente, a un nivel de transparencia del cincuenta porciento.

### Propiedades de texto

Entre las propiedades para dar formato al texto tenemos:

#### Font-size
Esta propiedad sirve para indicar el tamaño que van a tener los textos dentro del documento, pudiendo tener valores absolutos como 16px y relativos como: 1.2em o 120%.

```css
.header__title{
  font-size: 31px;
}
```

#### Text-decoration

Es la propiedad para añadir detalles decorativos al texto.

```css
.post__link{
  text-decoration: none; /* quita subrayado */
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

### Modelo de caja
Sirve para comprender las diferentes propiedades que afectan al tamaño y disposición de una caja.

#### Content (contenido): 
Contenido de la caja el cual podría tener un texto, una imagen, u otros elementos, se le puede definir anchura con la propiedad **width** y altura con la propiedad **height**.

```css
.box{
	width: 800px; /* ancho de 800 pixeles */
	height: 600px; /* de preferencia es mejor no aplicarlo y dejar que lo que va dentro le de la altura con su propio volumen */
}
```

#### Padding (relleno):
Es la distancia del contenido de la caja hacia dentro del contenedor.
```css
.box{
	padding-right: 5px; /* distancia hacia el lado derecho. */
	padding-left: 5px; /* distancia hacia el lado izquierdo. */
	padding-top:5px; /* distancia hacia arriba. */
	padding-botton: 5px; /* distancia hacia abajo. */
}
```
**TIP:** Si deseas ahorrar líneas de código puedes aplicar esto:
```css
.box{
	padding: 5px 10px; /* el primero es para el right y left, el segundo es para el top y botton */ 
}
```

#### Margin (margen):
Es la distancia de la caja hacia afuera del contenedor.

```css
.box{
	margin-right: 5px; /* distancia hacia el lado derecho */
	margin-left: 5px; /* distancia hacia el lado izquierdo */
	margin-top:5px; /* distancia hacia arriba */
	margin-botton: 5px; /* distancia hacia abajo */
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
**TIP:** si deseas ahorrar escribiendo todas las declaraciones puedes usar este __shorthand__

```css
.box{
	border: solid 5px black; /* style width color */
}
```

**TIP:** Si deseas  que el padding y border respeten el tamaño de la caja, en otras palabras el tamaño de la caja lo defina el width del content, puedes usar esta propiedad:

```css
.box{
	box-sizing: border-box;
}
```

### Propiedades flexbox

#### Display
A esta propiedad le asignamos un valor **flex** o **flex-inline** (es lo menos común) dependiendo de la necesidad en tu diagramación. Al darle este valor permite disponer de un modo más fácil a todos sus hijos directos. Por defecto lo que va pasar es que todos sus hijos se acomoden de forma horizontal uno al lado del otro.

```css
.menu{
  display: flex;
}
```

#### Justify-content
La propiedad **justify-content** sirve para alinear a los elementos hijos cuando estos no usan todo el espacio disponible en el eje principal (por defecto es el horizontal).

```css
.menu{
  display: flex;
  justify-content: flex-start; /* otros valores posibles son: flex-end, center,  space-between, space-around, space-evenly */
}
```

**flex-start:** Alinea elementos al lado izquierdo del contenedor.
**flex-end:** Alinea elementos al lado derecho del contenedor.
**center: **Alinea elementos en el centro del contenedor.
**space-between:** Muestra elementos con la misma distancia entre ellos.
**space-around:** Muestra elementos con la misma separación alrededor de ellos.

#### Align-items
Esto define el comportamiento predeterminado de cómo se colocan los elementos hijos a lo largo del eje transversal en la línea actual (por defecto es el eje vertical). Es como la versión de **justify-content** para el eje transversal (perpendicular al eje principal).

```css
div{
  display: flex;
  align-items: flex-star; /* otros valores posibles son: flex-end, center, baseline, stretch */
}
```
**flex-start:** Alinea elementos hijos a la parte superior del contenedor padre.
**flex-end:** Alinea elementos hijos a la parte inferior del contenedor padre.
**center:** Alinea elementos hijos en el centro (verticalmente hablando) del contenedor padre.
**baseline:** Muestra elementos hijos en la línea base del contenedor padre.
**stretch:** Elementos hijos se estiran para ajustarse al contenedor padre.


#### Flex-direction

Esto establece el eje principal, definiendo así la dirección en que se colocan los elementos hijos  en el contenedor padre.

```css
.menu{
  display: flex;
  flex-direction: row; /* otros valores posibles son: row-reverse, column,  column-reverse */
}
```
**row:** Elementos son colocados en la misma dirección del texto.
**row-reverse:** Elementos son colocados en la dirección opuesta al texto.
**column:** Elementos se colocan de arriba hacia abajo.
**column-reverse:** Elementos se colocan de abajo hacia arriba.

#### Flex-wrap

Por defecto, todos los elementos hijos  intentarán caber en una línea. Puede cambiar eso y permitir que pasen a una segunda fila (si fuera necesario) con esta propiedad.

```css
.posts{
  display: flex;
  flex-wrap: nowrap; /* otros valores: wrap, wrap-reverse */
}
```
**nowrap:** Cada elemento se ajusta en una sola línea.
**wrap:** los elementos se envuelven alrededor de líneas adicionales.
**wrap-reverse:** Los elementos se envuelven alrededor de líneas adicionales en reversa.


### Imágenes de Fondo

#### Background-image
Sirve para establecer la imagen de fondo de un elemento. La imagen se muestra en la zona que ocupan el contenido y el relleno del elemento, justo hasta su borde.

Para indicar la imagen que se muestra como fondo de un elemento, se utiliza una URL. 

```css
body{
  background-image: url("../images/fondo.jpg");
}
```

#### Background-size
Esta propiedad se utiliza para determinar el tamaño de la imagen de fondo, estableciendo ancho y alto de la misma.

```css
body{
  background-image: url("imagenes/fondo.jpg");
  Background-size: 300px 200px; /* otros valores: 50% 50%, cover */
}
```
**TIP:** si se le asigna el valor **cover** la imagen cubrirá todo el area disponible, muy util para cuando queremos que se adapte a diferentest tamaños de pantalla o dispositivo.

#### Background-attachment
Esta propiedad sirve para controlar si la imagen de fondo se mueve o permanece fija cuando se hace scroll en la ventana del navegador. 

**Scroll:** Es el valor base y consiste en que la imagen de fondo se mueve con el elemento.

**Fixed:** Consiste en que la imagen de fondo permanece fija cuando se hace scroll en la ventana del navegador.

```css
body {
  background-image: url("../images/fondo.jpg");
  background-attachment: fixed;
}
```

#### Background-repeat
Esta propiedad sirve para controlar el tipo de repetición de las imágenes de fondo, si se repite o no y las direcciones en las que se repite. Se pueden usar solo uno de los siguientes valores permitidos a la vez: repeat, repeat-x, 
repeat-y ó no-repeat.

Por defecto, si la imagen de fondo que se establece con la propiedad background-image es más pequeña que el sitio disponible, el navegador repite la imagen en todas las direcciones hasta cubrir completamente la superficie del elemento.
```css
body {
  background-image: url("../images/patron.jpg");
  background-repeat: no-repeat;
}
```


Los valores repeat-x y repeat-y permiten repetir la imagen de fondo sólo en una dirección (horizontal o vertical).
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
La explicación de los valores permitidos para esta propiedad es compleja debido a su gran flexibilidad. Son dos valores separados por un espacio.

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








