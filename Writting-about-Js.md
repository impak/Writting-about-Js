# Writting about Javascript

Apuntes para comprender el lenguaje de programan Javascript y la logica al programar.

**Sentencias**

En un lenguaje de programación, un conjunto de palabras, números, y operadores que llevan a cabo una tarea específica se denomina sentencia. En JavaScript, una sentencia podría verse de la siguiente forma:

```javascript
 a = b * 2;
```

**Expresiones**

Esta sentencia tiene varias "Expresiones" en ella:

```jsx
a = b * 2;
```

Descripciones:

-   `2` es una _expresión literal de valor_
-   `b` es una _expresión de variable_
-   `b * 2` es una _expresión aritmética_
-   `a = b * 2` es una _expresión de asignación_

**Operadores**

Los operadores son la forma en la que ejecutamos acciones en variables y valores.

El operador `=` (expresión de asignación) es usado para la asignación. Primero se calcula el valor en el lado derecho (valor fuente) del operador `=` y luego se asigna a la variable especificada en el lado izquierdo (variable objetivo).

Ejemplo: 

```jsx
a = 2;
b = a + 1;
```

Acá, se asigna el valor `2` a la variable `a`. Entonces, obtenemos el valor de la variable `a` (siendo 2).
Luego se le asigna a la variable `b` la variable `a` (valor `2`) mas el valor `1`(siendo `3` el valor obtenido en la variable `b`).

Algunos de los siguientes operadores los vamos a ver mas adelante:

-   Asignación: como en `a = 2`.
    
-   Matemáticos: `+` (adición), `-` (sustracción), `*` (multiplicación), y `/` (división), como en `a * 3`.
    
-   Asignación compuesta: `+=`, `-=`, `*=`, y `/=` son operadores compuestos que combinan una operación matemática con una asignación, como en `a += 2` (que es equivalente a escribir `a = a + 2`).
    
-   Incremento/Decremento: `++` (incremento), `--` (decremento), como en `a++` (que es equivalente a escribir `a = a + 1` ).
    
-   Acceso a las propiedades de un objeto: `.` como en `console.log()`.
    
    Los objetos son valores que guardan otros valores en lugares con nombres específicos llamados propiedades. `obj.a` indica el valor de un objeto llamado `obj` con una propiedad de nombre `a`. Las propiedades pueden ser accedidas alternativamente como `obj["a"]`.
    
-   Igualdad: `==` (igual), `===` (estrictamente-igual), `!=` (distinto), `!==` (estrictamente distinto, como en `a == b`.
    
-   Comparación: `<` (menor que), `>` (mayor que), `<=` (menor o igual), `>=` (mayor o igual), como en `a <= b`.
    
-   Lógicos: `&&` (y), `||` (o), como en `a || b` que selecciona a o b. Estos operadores son usados para expresar condicionales compuestos, como si a o b seanverdaderos.

**Variables**

Debemos entender que una variable es un "espacio" que contiene valores:

```jsx
a = b * 2;
```

En la sentencia anterior `a` le fue asignado `b * 2` gracias al operador `=`. Esto quiere decir que `a` es la variable que contiene `b * 2` .
