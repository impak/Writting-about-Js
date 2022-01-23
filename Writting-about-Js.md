# Writting about Javascript

Estos escritos son apuntes simples como recordatorios del lenguaje. 

**Sentencias**

En un lenguaje de programación, un conjunto de palabras, números, y operadores que llevan a cabo una tarea específica se denomina sentencia. En JavaScript, una sentencia podría verse de la siguiente forma:

```javascript
var a = b * 2;
```

**Expresiones**

Esta sentencia tiene varias "Expresiones" en ella:

```jsx
var a = b * 2;
```

Descripciones:

-  `a = b * 2` es una expresión de asignación.
-  `a` y `b` son expresiones de variables.
-  `2` es una expresión literal de valor.
-  `b * 2` es una expresión aritmética.

**Operadores** (Asignación & Aritméticos)

Los operadores son la forma en la que ejecutamos acciones en variables y valores.
Existen varios tipos de operadores, empecemos por Operador de Asignación y Operadores Aritméticos. 

El operador `=`, es usado para la asignación. Primero se calcula el valor en el lado derecho (valor fuente) del operador `=` y luego se asigna a la variable especificada en el lado izquierdo (variable objetivo).

Ejemplo: 

```jsx
a = 2;
b = a + 1;
```

Acá, se asigna el valor `2` a la variable `a`. Entonces, obtenemos el valor de la variable `a` (siendo 2).
Luego se le asigna a la variable `b` la variable `a` (valor `2`) más el valor `1`(siendo `3` el valor obtenido en la variable `b`).

Operadores aritméticos.

- `+` (adición), 
- `-` (sustracción), 
- `*` (multiplicación)
- `/` (división)

Más adelante veremos:
- `%` (módulo aritmético) Divide dos números, obteniendo un "resto" entero: 5 % 2 = 1
- `++ --` (Incrementos y decrementos).

**Variables**

Debemos entender que una variable es un "espacio" con un nombre especí	fico que contiene un valor y este puede cambiar (o variar):

```jsx
var a = b * 2;
```

En la sentencia anterior la palabra reservada `var` especifica que la letra `a` es la variable en cuestión, que a su vez le fue asignado `b * 2` gracias al operador `=`.

Nomenclatura y requisitos para un nombre:

Según por convención el nombre de una variable sigue una nomenclatura de tipo camelCase. Ejemplo:

```jsx
var miIdioma = "Español";
```

Donde si el nombre de la variable tiene dos palabras, deben estar unidas, empezar con minúsculas en la primera palabra, y en la segunda iniciar con mayúsculas.

Es una buena y recomendable práctica, aunque en el lenguaje esto no es estrictamente requerido.

Requisitos a tener en cuenta:

- Comenzar con minúscula, guión bajo o signo peso:

```jsx
var edad;
var _x;
var $nombre;
```

- Solo se puede escribir un nombre con letras minúsculas, mayúsculas.

```jsx
var nombre;
var Nombre;
```

- La variable `Nombre` no es la misma que `nombre` porque JavaScript distingue entre mayúsculas y minúsculas.

```jsx
var Nombre;
var nombre;
```

Declarar e Inicializar variables:

Declarar una variable, se entiende como una variable sin un valor asignado. 

```jsx
var a;
```

Esto sirve para indicar que esa variable existe y que en otra instancia del código se va a inicializar asignando un valor.

```jsx
a = 1;
```

**Programar**

Podemos entender como programa una solución informática a una idea o problema. Y programar es crear ese programa.

Ejemplo: Hacer un programa que sume dos números y que muestre en pantalla el resultado de ellos.

```jsx
var numeroUno, numeroDos, resultado;

numeroUno = 6;
numeroDos = 4;
resultado = numeroUno + numeroDos;

console.log(resultado);
```

Podemos ejecutar este programa pegando el código en la consola de nuestro navegador seguido de enter.

Desglosamos el programa en un algoritmo de 4 pasos:

1. Inicio/Ingreso: `var numeroUno, numeroDos;` inicializa las variables `numeroUno` y `numeroDos` (esto le indica al computador que creaste 2 variables).
2. Proceso: Asignamos el valor `6` a la variable `numeroUno` y el valor `4` a la variable `numeroDos`. Luego a la variable `resultado` y le asignamos las variables `numeroUno + numeroDos`.
3. Egreso: Por último usamos el método `console.log` para imprimir por pantalla la variable `resultado`.
4. Fin: Vemos el resultado.

**console.log**	

En el programa anterior usamos la interface `console` con su método `console.log`, para entender que son empecemos con sus definiciones:

Console es una de las tantas interfaces que tiene javascript con el navegador y proporciona acceso a la consola de depuración del mismo. Por otro lado tenemos uno de los tantos métodos de console, `console.log` que envía un mensaje a la consola web. De este modo pudimos ver que hay de resultado en la variable `resultado`.

