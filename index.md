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

## Conceptos Basicos

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