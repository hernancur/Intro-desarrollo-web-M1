En esta clase cubriremos:

* Bucles `for`
* Introducción a los arrays
* Bucles `for` con arrays

## Bucles `for`

La mayoría del software se ejecuta en bucles (ciclos), evaluando expresiones una y otra vez hasta que devuelve lo que estamos buscando o se detiene después de cierto tiempo. Javascript tiene dos expresiones de bucle incorporadas y hoy veremos la primera, el bucle "for".

Los bucles `for` tienen una sintaxis única, similar a la instrucción` if`, pero un poco más compleja. Primero tenemos la palabra clave `for`, seguida de paréntesis y luego abrir y cerrar llaves. Dentro de los paréntesis necesitaremos tres cosas. Primero, debemos declarar una variable, esto es sobre lo que se repetirá el bucle. Entonces tendremos una expresión condicional, el ciclo continuará sucediendo hasta que esta declaración sea `false`. Tercero, incrementaremos nuestra variable. Las tres declaraciones están separadas por un punto y coma.

```javascript
for (let i = 0                 ; i < 10                 ; i++          ) {
// | Declaramos una variable | Expresión condcicional | Incrementamos la variable |
    console.log(i);
}
```

En este ejemplo, vemos que inicialmente establecemos nuestra variable `i` en 0, el ciclo se ejecutará y cada vez que llegue al final, aumentará el contador en uno. El bucle `for` evaluará la expresión condicional. Si es `true`, se ejecutará nuevamente, si es `false` dejará de funcionar.

### El operador ++

Vimos en el último ejemplo el operador `++`. Esta es la abreviatura de Javascript para "Establecer el valor de la variable a su valor actual más uno". Hay algunas más de estas expresiones abreviadas de matemática / asignación variable, las visitaremos en las próximas lecciones.

### Bucles infinitos

Es posible que un bucle se atasque en lo que llamamos un "bucle infinito". Debes asegurarte de que haya una forma de finalizar el bucle. Ejemplo de un bucle infinito:

```javascript
for (let i = 0; i >= 0; i++) {
    console.log(i);
}
```

Debido a que nuestra expresión condicional SIEMPRE será `true` (` i` nunca será menor que 0), este ciclo se ejecutará esencialmente para siempre. Esto interrumpirá su programa y puede bloquear su navegador web o computadora.



## Introducción a los arrays (matrices/arreglos)

En la clases anteriores discutimos 3 tipos de datos básicos (cadenas/strings, números y booleanos) y cómo asignar esos tipos de datos a las variables. Discutimos cómo una variable solo puede apuntar a una sola cadena, número o booleano. Sin embargo, en muchos casos queremos poder apuntar a una colección de tipos de datos. Por ejemplo, ¿qué pasaría si quisiéramos hacer un seguimiento del nombre de cada estudiante en esta clase usando una sola variable, `nombresEstudiantes`. Podemos hacer eso usando Arrays. Podemos pensar en las matrices como contenedores de almacenamiento para colecciones de datos. Construir un array es simple, declarar una variable y establecerla en []. Luego podemos agregar al contenedor (separadas por coma) tantas cadenas, números o booleanos como queramos y acceder a esos elementos cuando lo deseemos.

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];
```

### .length

Al igual que el tipo de dato _String_ tiene un método incorporado `.length`, también lo hace la matriz. De hecho, la matriz tiene muchos métodos incorporados útiles (los discutiremos en lecciones posteriores). Al igual que la cadena `.length` cuenta los caracteres, la matriz` .length` devolverá el número de elementos en una matriz:

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];

console.log(nombresEstudiantes.length);  // 4
```

### Acceso a elementos en una matriz

Podemos acceder a un elemento de una matriza en cualquier momento, solo necesitamos llamar al elemento por su posición en la matriz. Los elementos reciben una posición numérica (índice) de acuerdo con su ubicación en la matriz, en orden. El orden numérico de una matriz SIEMPRE comienza en 0, por lo que el primer elemento está en el índice 0, el segundo en el índice 1, el tercero en el 2, y así sucesivamente (esto puede ser complicado al principio, pero solo recuerda que las matrices siempre comienzan en 0).

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];
                                0         1        2        3
```

Para acceder al elemento, escribiremos el nombre o la variable de matriz, seguidos de corchetes que contienen la asignación numérica.

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];

console.log(nombresEstudiantes[1]);  // 'Antonio'
```

Para acceder dinámicamente al último elemento de la matriz, utilizaremos el método `.length`. En nuestra matriz `nombresEstudiantes`, la longitud es 4. Sabemos que el primer elemento siempre será 0, y cada elemento posterior se desplaza sobre un número. Entonces, en nuestro ejemplo, el último elemento tiene un índice de 3. Usando nuestra propiedad de longitud mostraremos cómo se hace cuando no sabemos el número de elementos en una matriz:

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', ... ,'Samuel'];

console.log(nombresEstudiantes[nombresEstudiantes.length - 1]);  // 'Samuel'
```

### Asignación

Podemos asignar y reasignar cualquier índice en la matriz usando el paréntesis/índice y un "=".

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];

nombresEstudiantes[0] = 'Jorge';

console.log(nombresEstudiantes);  // ['Jorge', 'Antonio', 'Sara', 'Samuel']
```
### `.push` y `.pop`

Otros dos métodos de matriz incorporados muy útiles son `.push` y` .pop`. Estos métodos se refieren a la adición y eliminación de elementos de la matriz después de su declaración inicial.

`.push` agrega un elemento al final de la matriz, incrementando su longitud en 1. `.push` devuelve la nueva longitud.

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];

nombresEstudiantes.push('Patricia');

console.log(nombresEstudiantes);  // ['Martin', 'Antonio', 'Sara', 'Samuel', 'Patricia']
```

`.pop` elimina el último elemento de la matriz, disminuyendo la longitud en 1. `.pop` devuelve el elemento "reventado" (_popped_).

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];

nombresEstudiantes.pop();

console.log(nombresEstudiantes);  // ['Martin', 'Antonio', 'Sara']
```

### `.unshift` y `.shift`

`.unshift` y` .shift` son exactamente como `.push` y` .pop`, excepto que operan en el primer elemento de la matriz. `.unshift(item)` colocará un nuevo elemento en la primera posición de la matriz, y `.shift()` eliminará el primer elemento de la matriz.

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];

nombresEstudiantes.unshift('Leo');

console.log(nombresEstudiantes);  // ['Leo', 'Martin', 'Antonio', 'Sara', 'Samuel']

nombresEstudiantes.shift();

console.log(nombresEstudiantes);  // ['Martin', 'Antonio', 'Sara', 'Samuel']
```

## Utilizando bucles `for` en arrays

La mayoría de las veces, los bucles for se utilizan para iterar sobre todos los elementos de una matriz. Usando la técnica de acceso al índice ("index access technique") podemos acceder a cada elemento de la matriz. Para hacer esto, usamos el método `.length` como punto de parada para el ciclo.

```javascript
const nombresEstudiantes = ['Martin', 'Antonio', 'Sara', 'Samuel'];

for (let i = 0; i < nombresEstudiantes.length; i++) {
    console.log(nombresEstudiantes[i]);
}

// 'Martin'
// 'Antonio'
// 'Sara'
// 'Samuel'
```

## Abre la carpeta "homework" y completa la tarea descrita en el archivo README


## Recursos adicionales

* [MDN: Arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
* [MDN: for Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for)