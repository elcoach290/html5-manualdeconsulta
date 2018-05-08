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
		- [Header](#Header)
		- [Nav](#Nav)
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
###Hosting
Espacio en un servidor web para guardar los archivos de un sitio web, normalmente vinculado a un **dominio**.

## Hyper Text Markup Language

El Hyper Text Markup Language ( HTML ) es un lenguaje de marcado o etiquetado que sirve para estructurar la información dentro de una página web, mediante las etiquetas vamos a poder indicar  si un texto es un título o un párrafo, si deseamos tener un listado de cierta información también se tiene una etiqueta para este fin.

### Estructura basica de todo documento HTML5
```html
<!doctype html>
<html>
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
<!-- enlace a una pagina home del sitio -->
<a href="index.html">Ir al Home</a>
<!-- enlace para visualizar un archivo pdf -->
<a href="curriculum.pdf">Ver curriculum</a>
<!-- enlace para visualizar una imagen -->
<a href="images/fotogrande.jpg">Ver foto</a>
<!-- enlace para ir dirigirnos a otro sitio -->
<a href="http://www.google.com">Ir a Google</a>
```

## Imagenes
## Listas
## Tablas
## Otras etiquetas




** Tip: **
## Agrupadores semanticos
### Header
Para envolver a los elementos de la cabecera de una pagina web o seccion, pudiendo ser estos el `<h1></h1>` y el `<nav></nav>`.
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
## Estilos CSS