# Introducción a CSS

En esta clase, exploraremos los conceptos básicos de CSS (Cascading Style Sheets), el lenguaje utilizado para dar estilo a las páginas web, es decir, "como se verán" (colores, tamaños, posiciones, etc.)

## Contenido de la Clase

- **¿Qué es CSS?**

- **Selectores, propiedades y valores**

- **Estilos de texto, unidades de medida, fondos**


### **¿Qué es CSS?**

CSS (Hojas de Estilo en Cascada) es un lenguaje web para aplicar formato visual (color, tamaño, separación y ubicación) al HTML. CSS puede hacer un texto más grande, ponerle un color, un fondo, una tipografía, etc. Su objetivo es separar la estructura (el HTML) del formato con que se pretende mostrar. Con CSS puedes cambiar por completo el aspecto de cualquier etiqueta HTML. 

#### Sintaxis CSS

El CSS al igual que el HTML tiene una sintaxis a la hora de crear las clases y sus atributos. El CSS se escribe en archivos con la extensión `.css`.

Aquí tienes un ejemplo básico de cómo se ve el código CSS:
![](https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/try3UqBbVsBUt0wJ.png)

Y aquí uno más concreto

![](https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/ZbhHJdvvGy1iyin2.jpg)

#### En clase veremos las 3 formas de INSERTAR CSS en HTML, como además de las REGLAS para escribir un archivo .CSS correctamente.



### **Selectores, propiedades y valores**

En este tema hablaremos sobre los distintos tipos de selectores que podemos utilizar, sus prioridades, y el concepto de herencia y cascada.

#### Tipos de selectores CSS. 

Existen tres los cuales son: `tag`, `class` y `id`

![](https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/a-dtn4lnGSx5OTre.jpg)



### **Estilos de texto, unidades de medida, fondos**

#### Texto - Tipografía/Fuentes

La propiedad font-family define una lista de fuentes (tipografía) para utilizar en un elemento seleccionado. Su posible valor puede ser cualquier nombre de una tipografía disponible en tu computadora.
Cada sistema operativo y navegador interpretan de distinta forma las fuentes predeterminadas.

Ejemplos:
- **Serif**: «Times New Roman» 
- **Sans serif**: «Arial» 
- **Monospace**: «Courrier New» 

![](https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/9_creCDlVsrPwyQV.jpg)


### Texto - Color

La propiedad color selecciona el valor de color del texto de un elemento y sus decoraciones. 
Debes tener en cuenta que existen distintos valores que puede tomar esta propiedad, pero nos centraremos en tres:

#### Unidades de medida de colores: 

- Nombre del color (por ejemplo: red).
- Hexadecimal (por ejemplo: #FFFFFF).
- RGB (por ejemplo: 50, 212, 227). Si agregas un valor más, puedes manejar su opacidad. Cada color permite hasta 256 valores.

![](https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/jQyQZvHsBxwheLFR.jpg)


### Fondos

#### background-color
La forma de indicar el color de fondo de una etiqueta desde CSS es con la propiedad background-color. Como valor, podemos utilizar uno de los colores predeterminados, el sistema hexadecimal, el sistema RGB o la palabra clave transparent.

<img alt="bg-color" src="https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/yVf1lsbJlIf6Z5Vd.jpg" width="700" height="300" />


#### background-image
No sólo podemos aplicar color, sino que además podemos aplicar una imagen como fondo de una etiqueta. La propiedad a utilizar, en este caso, es background-image.

Las imágenes de fondo se indican a través de su URL, y deben ser enlazadas mediante la función url(“...”) como valor de la propiedad.

Algo importante a tener en cuenta, son los formatos de imágenes que podemos utilizar para el fondo. Los mismos son: JPG, PNG o GIF. En todos los casos, tienen que estar en modo RGB.

<img alt="bg-color" src="https://articulateusercontent.com/rise/courses/IsJhcdVTk07F7gXCizLndX7mo7HruKpc/QE2U8VYnQ_Wkvr_4.jpg" width="700" height="300" />