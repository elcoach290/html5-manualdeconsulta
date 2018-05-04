# Manual del Guerrero HTML5
## Indice
- [Terminos Basicos](#Terminos_Basicos_4)
- [Estructura básica de todo documento HTML5](#Estructura_basica_de_todo_documento_HTML5_9)
- [Estilos CSS](#Estilos_CSS)
## Terminos Basicos
- **Sitio Web** conjunto de páginas web interconectadas con un proposito determinado, ejemplo: Sitio Web de Nike, Sitio Web del Poder Judicial, etc.
- **Pagina Web** documento digital que permite estructurar informacion ( textos, hipertextos ) y contenido multimedia ( video, audio, imagenes, etc )
- **Dominio** es la url o direccion principal en internet donde se encuentra un sitio web.
- **Hosting** espacio en un servidor web para guardar los archivos de un sitio web, normalmente vinculado a un **dominio**. 
## Estructura basica de todo documento HTML5
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