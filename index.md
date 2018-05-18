# Manual del Guerrero HTML5

## Indice

- [Conceptos Basicos](#Conceptos_Basicos_4)
	- [Carpeta](#Carpeta)
	- [Archivo](#Archivo)
	- [Sitio Web](#Sitio_Web)
	- [Pagina Web](#Pagina_Web)
	- [Dominio](#Dominio)
	- [Hosting](#Hosting)

- [Hyper Text Markup Language](#Hyper_Text_Markup_Language)	
	- [Estructura básica de todo documento HTML5](#Estructura_basica_de_todo_documento_HTML5_9)
	- [Elementos básicos](#Elementos_basicos)
		- [Titulares](#Titulares)
		- [Parrafos](#Parrafos)
		- [Enlaces](#Enlaces)
		- [Imagenes](#Imagenes)
		- [Listas](#Listas)
		- [Tablas](#Tablas)
		- [Otras etiquetas](#Otras_etiquetas)
	- [Agrupadores Semánticos](#Agrupadores_semanticos)
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

## Headings

Son los encabezados o titulos que usaremos en nuestro documento existen del **h1** al **h6**, siendo el mas importante el **h1** y asi va bajando hasta el **h6** que es el menor importante.

```html
<h1>El titulo mas importante del documento</h1>
<h2>El titulo de un segundo nivel de importancia </h2>
...
<h6>El titulo menos importante</h6>
```

## Parrafos

Cuando necesitamos escribir parrafos el texto lo colocamos dentro de la etiquetas `<p></p>`

```html
<p>Todo lo que necesitas para lograr tus objetivos ya está en ti.</p>
<p>No vas a dominar el resto de tu vida en un día. Relájate. Domina el día. Entonces sigue haciendo eso todos los días.</p>
```

## Enlaces

Los enlaces son los que nos van a permitir conectar las paginas de nuestro sitio o conectarlas con otras paginas externas, tambien podemos colocar como destinos de los enlaces imagenes o documentos como pdfs.

```html
<!-- enlace a la pagina home del sitio -->
<a href="index.html">Ir al Home</a>
<!-- enlace a un id específico dentro de una web -->
<a href="#id-a-visitar">Ir a sección</a> <!-- en la página actual -->
<a href="seccion/#id-a-visitar">Ir a sección</a> <!-- en otra página de la misma web -->
<a href="http://webdeotracosa.com/seccion/#id-a-visitar">Ir a sección</a> <!-- en otra página de internet -->
<!-- enlace para visualizar un archivo pdf -->
<a href="curriculum.pdf">Ver curriculum</a>
<!-- enlace para visualizar una imagen -->
<a href="images/fotogrande.jpg">Ver foto</a>
<!-- enlace para ir dirigirnos a otro sitio -->
<a href="http://www.google.com">Ir a Google</a>
```
**TIP:** Si deseas que el destino se abra en otra pestaña del navegador le añades el atributo **_target_** con el valor **__blank_**

```html
<a href="http://facebook.com" target="_blank">Este enlace abrirá en otra pestaña</a>
``` 

## Imagenes

Podemos vincular imagenes de distintos tipos en nuestras paginas web para que se puedan visualizar al momento de visualizarse de la siguiente manera:

```html
<img src="images/foto.jpg" alt="Foto de Perfil">
```

Requieren de dos atributos, **src** para indicar la ubicacion de la imagen y **alt** que es para indicar un texto alternativo en casos la imagen por algun motivo no se haya descargado, tambien sirve para la accesibilidad, muy importante para los usuarios invidentes. Recordemos que podemos cargar muchos formatos de imagen, como son JPG, PNG y GIF

## Listas

Las lista se utilizan cuando requieres mostras una secuencia de datos o elementos, pueden ser ordenadas o desordenadas.

### Listas ordenadas

En ellas importa el orden de los elementos podrian ser los pasos para realizar un tramite.

```html
<ol>
	<li>Acudir al Banco de la Nación, pedir el concepto 1810 y pagar S/ 98.50 por el pasaporte biométrico.</li>
	<li>Ingresar a www.migraciones.gob.pe, llenar el formulario y separar una cita.</li>
	<li>El pasaporte será entregado en las 14 sedes de Migraciones. Debe llevar su voucher y DNI, no es necesario una foto.</li>
</ol>
```

### Listas no ordenadas

En ellas no es relevante el orden de los elementos y se pueden tener otras etiquetas incluso, como en el caso de un listado de enlaces:

```html
<ul>
	<li><a href="index.html">Inicio</a></li>
	<li><a href="servicios.html">Servicios</a></li>
	<li><a href="contacto.html">Contacto</a></li>
</ul>
```

## Tablas

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

## Otras etiquetas

### Strong

Nos sirve para indicar que un texto o palabra es importante:

```html
<p>El personaje de Tony Stark es caracterizado por el actor <strong>Robert Downey Jr.</strong></p>
```

### Span

Esta etiqueta sirve para poder cambiar el formato a una palabra a caracter sin que esto afecte su significado, el cambio recien se hace visible aplicando estilos css

```html
<h2><span>Gatotel</span>, un lugar para quedarse.</h2>
```

### Blockquote

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
	<h1><a href="index.html"><img src="images/logo.svg" alt="Gatotel"></a></h1>
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
	<p>Copyright 2018 - Diseño y Desarrollo por <a href="http://www.anthonystudio.com">anthonystudio.com</a></p>
</footer>
```

### Article

Se usa envolver a una composición de elementos con datos que hacen referencia a una idea o información autonónoma. Un uso común puede ser como entrada de blog, noticia de periódico, ficha técnica de algún producto, etc. Debe tener como mínimo un título y párrafos.

```html
<article>
	<h2>Perú en alerta epidemiológica</h2>
	<p>En dos semanas hay más de 30 afectados confirmados, cuatro de ellos en Lima ...</p>
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

Se usa para agrupar otros elementos con fines de adaptar la disposición de estos al diseño de la interfaz, no aporta semántica 

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
Con HTML5 ahora podemos incluir videos y audio ya que antes solo era posible hacerlo usando plugins adicionales como el conocido flash player que ahora solo es parte de la historia del desarrollo web.

### Video
De esta forma podríamos incluir un video dentro de nuestro sitio web
```html
<video src="videos/intro.mp4" controls></video>
```

El atributo src es para indicar la ubicación del video mientras el atributo controls permite mostrar los controles de reproducción, otros atributos opcionales son: poster, preload, height, autoplay, muted.

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
``

Por lo general tienen un atributo action que hace referencia al archivo que se va encargar de procesar los datos ingresados y el atributo method que es indica la forma en que se va enviar para caso de formularios de contacto sería el valor **POST**

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
<!-- Este tipo de campo para cuando tenemos varias alternativas a selecionar pero solo una podemos marcar -->
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



## Estilos CSS
