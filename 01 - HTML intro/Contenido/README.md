# Introducción a HTML

Esta clase cubre los conceptos básicos de HTML (Hypertext Markup Language), el lenguaje utilizado para estructurar contenido en la web. Aprenderás sobre etiquetas HTML, cómo "marcar" contenido y cómo se interpreta este marcado.

## Contenido del Módulo

1. **Etiquetas básicas de HTML**: Etiquetas para encabezados, párrafos, listas, enlaces, imágenes y tablas.

## Para empezar

Imagina que quieres crear una página web con un encabezado "Mi sitio web" y un párrafo "Bienvenidos a mi sitio web". Necesitarías usar etiquetas HTML para marcar este contenido. Aquí tienes un ejemplo:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mi sitio web</title>
</head>
<body>
    <h1>Mi sitio web</h1>
    <p>Bienvenidos a mi sitio web</p>
</body>
</html>
```
## Etiquetas HTML


HTML utiliza etiquetas para proporcionar un significado y legibilidad automática al contenido de la página. Asimismo aprenderemos sobre las jerarquías en HTML: la cabecera (head) y el cuerpo (body), y que estas secciones pueden contener subsecciones. Además, se presenta la etiqueta <!DOCTYPE>, que define el tipo de documento y permite al navegador interpretar correctamente el código.


En el ejemplo, las etiquetas ``` <html>, <head>, y <body> ``` se usan para marcar el inicio y el final de la página web, mientras que las etiquetas``` <title>, <h1>, y <p>``` se usan para marcar el contenido de la página. El encabezado se marca con la etiqueta ```<h1>``` y el párrafo se marca con la etiqueta ```<p>```.


## Estructura de una etiqueta

Una etiqueta es una marca o identificador que se utiliza para definir el inicio y el final de un elemento dentro de una página web. 

Cada etiqueta se compone de corchetes angulares (< y >), seguidos del nombre de la etiqueta, y puede tener atributos y valores que proporcionan información adicional sobre el elemento. Las etiquetas se utilizan para definir la estructura y el contenido de una página web, y permiten al navegador interpretar y renderizar correctamente la información que se muestra al usuario. Ejemplos de etiquetas en HTML incluyen `<html>, <head>, <body>, <p>, <img>, <a>,` entre otras.

Podemos referirnos a las etiquetas como elementos, sin embargo hay una pequeña diferencia entre estos conceptos:

Elemento: Es el bloque de HTML que ya ha sido renderizado, generalmente está conformado por dos etiquetas separadas, una de apertura y otra de cierre.

Etiqueta: La etiqueta está escrita de una forma que el navegador pueda encontrarla, rodeada de los símbolos menor que < y mayor que >.

![](https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/qK50lot7-kj8u9H8.png)

La estructura del ejemplo anterior aplica para casi todas las etiquetas, sin embargo existen excepciones para el caso en que una etiqueta no tenga contenido para trabajar, por lo que se omite la etiqueta de cierre. Algunas excepciones:

`<hr>`
`<br>`
`<img>`
`<input>`
`<link>`
`<meta>`

## Atributos de una etiqueta 

Los atributos en las etiquetas HTML son como etiquetas adicionales que se utilizan para proporcionar información adicional sobre un elemento en una página web. 

Por ejemplo, si tienes una imagen en tu página web, puedes usar el atributo "src" para decirle al navegador de internet dónde encontrar la imagen. Sería como darle una dirección específica a esa imagen. También puedes usar atributos como "alt" para proporcionar una descripción de la imagen.

`<img src="link-de-una-imagen" alt="descripcion" />`

Los atributos ayudan a personalizar y darle significado a los elementos de tu página web, permitiendo que los navegadores y motores de búsqueda entiendan mejor cómo mostrar y procesar tu contenido. En resumen, son como etiquetas adicionales que agregas a tus elementos HTML para proporcionar información adicional o configurar su comportamiento.



## ¿Qué significa marcado?

Significa que con HTML podemos declarar QUÉ se verá en la pagina, pero no del todo COMO se verá. 

Para que la información que está en el documento HTML sea interpretada correctamente, el navegador espera que el documento siga un formato estándar, estructurado jerárquicamente por dos secciones principales: la cabecera (head) y el cuerpo (body).

![](https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/49gBsJrP-xQRfx-C.png)

Tanto el encabezado (head) como el cuerpo (body), permiten anidar más secciones. Lo cual da forma a un tipo de árbol de contenido, que es la forma como el navegador lo ve.

### Etiqueta <!DOCTYPE>

HTML, como todos los lenguajes, ha pasado por diferentes versiones con el pasar del tiempo y su implementación. Por esto mismo, es necesario indicar al navegador la versión de HTML en la que se encuentran escritos los documentos que estamos intentando renderizar (mostrar en la pantalla del navegador).

Para ello, existe la etiqueta <!DOCTYPE> que, como su nombre lo indica, define el tipo de documento e indica al navegador cómo debe interpretar el código HTML y debe ubicarse al inicio del documento. Para el objetivo de nuestro curso sólo usaremos la etiqueta que define el tipo de documento como HTML5. La definimos de la siguiente manera:

 <!DOCTYPE>


## ¿Qué hemos aprendido?

En conclusión, la estructura básica de un documento HTML se divide en dos secciones principales: la cabecera y el cuerpo, las cuales pueden anidar más secciones para conformar un árbol de contenido. Para indicar al navegador la versión de HTML que estamos utilizando, utilizamos la etiqueta <!DOCTYPE>, la cual define el tipo de documento y cómo el navegador debe interpretar el código HTML. 

Las etiquetas son palabras clave con un formato especial que rodean el contenido y aplican significado semántico y legibilidad automática al mismo. Es importante recordar que las etiquetas tienen una etiqueta de apertura y una de cierre, aunque existen excepciones cuando una etiqueta no tiene contenido para trabajar. 

Con esta base, podemos comenzar a crear documentos HTML y a utilizar las etiquetas necesarias para maquetar nuestra página web.🚀🚀🚀🚀 