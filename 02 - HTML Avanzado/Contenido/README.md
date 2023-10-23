# Clase 2: HTML Avanzado

En esta clase, profundizaremos en algunos conceptos más avanzados de HTML. Aprenderás a crear listas, tablas y formularios en tus páginas web.

## Contenido de la Clase

1. **Listas en HTML**: Aprenderás a crear listas ordenadas y desordenadas en HTML, utilizando las etiquetas `<ol>`, `<ul>` y `<li>`.

2. **Formularios y entradas en HTML**: Descubrirás cómo guardar información del usuario a través de formularios, utilizando las etiquetas `<form>`, `<input>`, `<label>` y `<button>`.


## Listas en HTML

Las listas son una forma efectiva de presentar información de manera ordenada en una página web. HTML proporciona dos tipos principales de listas:

1. **Listas ordenadas (`<ol>`)**: Se utilizan cuando el orden de los elementos es importante. Los elementos de la lista (`<li>`) se numeran automáticamente.

```html
<ol>
  <li>Primer elemento</li>
  <li>Segundo elemento</li>
</ol>
```

2. **Listas desordenadas (<ul>)**: Se utilizan cuando el orden de los elementos no es importante. Los elementos de la lista (<li>) se marcann de la misma manera.

```html
<ul>
  <li>Elemento uno</li>
  <li>Elemento dos</li>
</ul>
```


## Formularios en HTML

Los formularios son fundamentales para interactuar con los usuarios, permitiendo recoger información del usuario. Un formulario se crea con la etiqueta `<form>` y puede contener varios tipos de elementos de entrada `<input>`, como campos de texto, casillas de verificación, botones, etc.

Aquí tienes un ejemplo básico de un formulario:

```html
<form action="/submit" method="post">
  <label for="name">Nombre:</label><br>
  <input type="text" id="name" name="name"><br>
  <input type="submit" value="Enviar">
</form>
```
En este ejemplo, el formulario contiene un campo de texto para el nombre del usuario y un botón para enviar el formulario. La etiqueta `<label>` se utiliza para proporcionar una descripción del campo de entrada.

- Observa con atención los atributos de cada "<tag>" ya que profundizaremos en algunos más en clase.

