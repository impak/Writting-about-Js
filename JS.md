# **Writting about Javascript**

## **Sentencias**

En un lenguaje de programación, un conjunto de palabras, números, y operadores que llevan a cabo una tarea específica se denomina sentencia. En JavaScript, una sentencia podría verse de la siguiente forma:

```javascript
 a = b * 2;
```

##**Expresiones**

Esta sentencia tiene varias "Expresiones" en ella:

```jsx
a = b * 2;
```

-   `2` es una _expresión literal de valor_
-   `b` es una _expresión de variable_, que significa buscar su valor actual
-   `b * 2` es una _expresión aritmética_, que significa hacer la multiplicación
-   `a = b * 2` es una _expresión de asignación_, que significa asignar el resultado de la expresión `b * 2` a la variable `a`.

## **Ejecución**

Un programa debe ser ejecutado.

```jsx
a = 21;

b = a * 2;

console.log( b );
```

Proceso de ejecutar código en la consola:

![alt text](https://github.com/impak/Writting-about-Js/blob/main/img/fig1.png)

El resultado de la ejecución es **42**.

## **Salida**

```jsx
console.log( x );
```

Muestra un mensaje en la consola web (o del intérprete javascript).

Hay dos características a explicar de comando "console.log(x)":

Primero, desglosando el comando nos vamos a encontrar con "log(x)" que refiere a un "llamado funcional". Estamos ingresando la variable x a la función, lo cual implica tomar el valor de x e imprimirlo.

Segundo, "console" es una referencia al objeto dónde la función log(..) se encuentre.

Otra forma de producir salida es ejecutar la sentencia alert(..). Pero está opción tendrá salida como ventana emergente (Pop-up) interrumpiendo la interfaz del navegador.

## **Entrada**

La manera más común de recibir información para una página en HTML es mostrar elementos de tipo formulario. De modo el usuario pueda escribir, y luego usar JS para leer esos valores y guardarlos en variables. Pero existe un modo más sencillo de obtener entrada del usuario, para efectos de aprendizaje. Use la función prompt(..):

```jsx
age = prompt( "Please tell me your age:" );
console.log( age );
```

El mensaje que se entrega a la función prompt(..) -- en este caso, "Please tell me your age:" -- es impreso en una ventana.

![alt text](https://github.com/impak/Writting-about-Js/blob/main/img/fig2.png)

Una vez se ingresa el texto al dar click en "OK", se observa que el valor que ingresó es guardado en la variable age, lo que puede verse cuando por salida usamos console.log(..):

![alt text](https://github.com/impak/Writting-about-Js/blob/main/img/fig3.png)

## **Operadores**

Los operadores son la forma en la que ejecutamos acciones en variables y valores.

El operador `*` lleva a cabo la multiplicación matemática.

El operador `=` es usado para la asignación. Primero se calcula el valor en el lado derecho (valor fuente) del `=` y luego se asigna a la variable especificada en el lado izquierdo (variable objetivo).

```jsx
a = 2;
b = a + 1;
```

Acá, se asigna el valor 2 a la variable a. Entonces, obtenemos el valor de la variable a (siendo 2), añadiendo 1 para obtener 3 como resultado, luego se guarda este valor en la variable b.

-   Asignación: como en `a = 2`.
    
-   Matemáticos: `+` (adición), `-` (sustracción), `*` (multiplicación), y `/` (división), como en `a * 3`.
    
-   Asignación compuesta: `+=`, `-=`, `*=`, y `/=` son operadores compuestos que combinan una operación matemática con una asignación, como en `a += 2` (que es equivalente a escribir `a = a + 2`).
    
-   Incremento/Decremento: `++` (incremento), `--` (decremento), como en `a++` (que es equivalente a escribir `a = a + 1` ).
    
-   Acceso a las propiedades de un objeto: `.` como en `console.log()`.
    
    Los objetos son valores que guardan otros valores en lugares con nombres específicos llamados propiedades. `obj.a` indica el valor de un objeto llamado `obj` con una propiedad de nombre `a`. Las propiedades pueden ser accedidas alternativamente como `obj["a"]`.
    
-   Igualdad: `==` (igual), `===` (estrictamente-igual), `!=` (distinto), `!==` (estrictamente distinto, como en `a == b`.
    
-   Comparación: `<` (menor que), `>` (mayor que), `<=` (menor o igual), `>=` (mayor o igual), como en `a <= b`.
    
-   Lógicos: `&&` (y), `||` (o), como en `a || b` que selecciona a o b. Estos operadores son usados para expresar condicionales compuestos, como si a o b seanverdaderos.

## **Valores y Tipos**

Las representaciones para los valores se llaman _tipos_ en terminología de programación. JavaScript posee tipos construidos para cada una de estas representaciones también llamados tipos _primitivos_:

-   Cuando necesite hacer matemáticas, usted requerirá un `number`
-   Cuando necesite imprimir un valor en pantalla, usted requerirá un `string` (uno o más caracteres, palabras, oraciones).
-   Cuando necesite tomar una decisión en su programa, usted requerirá un `boolean` (`true` or `false`).

Los valores que son incluídos directamente en el código fuente son llamados _literales_. Los literales `string` están rodeados por comillas dobles `"..."` o comillas sencillas (`'...'`) -- la única diferencia es la preferencia estilística. Los literales `number` y `boolean` se presentan como son (es decir, `42`, `true`, etc.).

Considere:

```jsx
"I am a string";
'I am also a string';

42;

true;
false;
```

## **Conversión Entre Tipos**

Si usted tiene un tipo de dato `number` pero necesita imprimirlo en pantalla, necesitará convertir el valor a tipo `string` y esta conversión en JavaScript es llamada "coerción". Similarmente, si alguien ingresa una serie de caractéres numéricos en un formulario de una página de ecommerce, es un `string`, pero si necesita usar ese valor para realizar operaciones matemáticas, necesitará _coercer_ al dato a que sea un `number`.

JavaScript provee diferentes facilidades para forzar la coerción entre _tipos_. Por ejemplo:

```jsx
var a = "42";
var b = Number( a );

console.log( a );	// "42"
console.log( b );	// 42
```

## **Comentarios en el código**

Estos son partes de texto en su programa que son insertados puramente para explicárselo a un humano. El intérprete/compilador siempre ignora estos comentarios.

Existen muchas opiniones sobre qué hace a un código ser bien comentado; no podemos definir una regla universal sobre esto. Pero algunas observaciones y guías son útiles para este propósito:

-   Código sin comentarios es subóptimo.
-   Muchos comentarios (un comentario por línea, por ejemplo) es probablemente un signo de código pobremente escrito.
-   Los comentarios deben explicar el _porqué_, no el _qué_. Estos pueden explicar el _cómo_ si el código es particularmente confuso.

En JavaScript, existen dos tipos de comentarios en el código: comentarios de una única línea y comentarios de múltiples líneas.

Considere:

```jsx
// This is a single-line comment

/* But this is
       a multiline
             comment.
                      */
```

```jsx
var a = 42;		// 42 is the meaning of life
```

```jsx
/* The following value is used because
   it has been shown that it answers
   every question in the universe. */
var a = 42;
```

```jsx
var a = /* arbitrary value */ 42;

console.log( a );	// 42
```

## **Variables**

Las variables son utilizadas como contenedores donde guardamos algún valor de tipo específico (pueden ser numbers, strings, etc.).


En nuestras variables podemos encontrarnos con dos versiones de tipado:

- El _tipado estático_ o _tipado fuerte_ es utilizado para la precisión buscada dentro de un código, esto previene conversiones de valor no intencionadas.

```jsx
var example = 5;
    //En este caso estamos asignándole a la variable example el valor 5. A esto también se lo llama "hardcodeo", que significa perder la prolijidad dejando valores y/o comportamientos fijos en el código de nuestro programa.
```

- El _tipado dinámico_ o _tipado débil_ permite a una variable almacenar cualquier tipo de valor en el tiempo.

```jsx
var example;

//En este otro caso, no le estamos asignando valor alguno a la variable example, por lo cual, es muy probable que esta variable pueda ser vulnerada ya que no se le ha asignado ningún tipo (string, number, char, etc.).
```

JavaScript utiliza el _tipado dinámico_, lo que significa que las variables pueden guardar valores de cualquier tipo sin ningún tipado fuerte.

Las variables en JavaScript son declaradas utilizando la sentencia <code>_**var**_</code>.

 *Considere:*
```jsx
var valor = 10.00;

valor = valor * 2;

console.log(valor); //20.00

//Si convertimos 'valor' a un string y agregamos "$" al principio:

valor = "$" + String(valor);

console.log(valor); // "$20.00"
```
La variable **valor** inicia guardando el número 10.00, luego almacena el resultado dde tipo **number** de **valor * 2**, lo cual es **20.00**.

La primer instrucción **console.log(...)** tiene que hacer coerción *implícita* desde **number** a **string** para imprimirllo.

Luego, la sentencia **valor = "signoPesos" + String (valor)** realiza coerción *explícita* del valor **20.00** a **string** y añade el caracter **"$"** al inicio. Hasta este punto, **valor** almacena el **string** con valor **"20.00"**, entonces el segundo **console.log(...)** no necesita realizar ninguna coerción para imprimirlo.

Algunos desarrolladores pueden notar la flexibilidad de usar la variable **valor** para cada uno de los valores. En cambio, quienes prefieran el tipado estático podrían preferir una variable separada como **valorStr** para guardar el resultado final **"$20.00"**, ya que es de un tipo diferente.

En este ejemplo **valor** almacena un valor que cambia con el curso del programa, gestionando el estado del mismo (el estado es seguir los cambios a los valores a medida que el programa es ejecutado).

Algunas variables pueden centralizarse en la asignación de valores, estas son llamadas **constantes**, cuando se declara una variable con un valor e intención de *no cambiar* durante el programa.

Las constantes son declaradas en la parte superior de un programa, así es conveniente para el desarrollador tener un lugar donde pueda cambiar el valor si así lo deseáse. 

Por convención, las constantes se escriben con mayúscula sostenida y guiones bajos entre las palabras.

Ejemplo:
 
```jsx
    const TAX_RATE = 0.08;	// 8% sales tax

    var valor = 99.99;

    valor = valor * 2;

    valor = valor + (valor * TAX_RATE);

    console.log( valor );				// 215.9784
    console.log( valor.toFixed( 2 ) );	// "215.98"
 ```

La variable **TAX_RATE** es únicamente *constante* por convención. Si se llegara a necesitar actualizar el valor de el mismo a un 9%, podemos fácilmente actualizar el programa asignando a **TAX_RATE** el valor de **0.09** en un solo lugar, en vez de encontrar todas las ocurrencias del valor **0.08**.


Las constantes son útiles como las variables con valores sin cambiar, excepto que las constantes previenen el cambio accidental de algún valor dónde sea que se haga después de la asignación inicial. Si usted intentó asignar algún valor distinto a **TAX_RATE** luego de su primera declaración, su programa podría rechazar el cambio.



## **Bloques**

Un bloque es definido rodeando una o más sentencias con una pareja de corchetes ``` {..}```. 

*Considere*:

```jsx
var valor = 10.00;

//bloque general
{
    valor = valor * 2;
    console.log(valor); //20.00
}
```

Los bloques son añadidos a algunas secuencias de control, como la sentencia **_if_** o un ciclo.

_Ejemplo_
```jsx
var valor = 99.99;

// iEs el valor mayor a 10?
if (valor > 10) {			// <--Bloque adjunto al if
	valor = valor * 2;
	console.log( valor );	// 199.98
}
```
El bloque <code>{...}</code> ejecutará las sentencias si el condicional es verdadero.


## **Condicionales**

Un condicional muy utilizado en JavaScript es **_if_**. 

La sentencia **_if_** puede ser tratada como *true* o *false*, es decir: "Si esta condición es verdadera, haga lo siguiente...".  Esta sentencia requiere una expresión dentro del paréntesis la cual será tratada como *true* o *false* dependiendo de la cantidad mostrada en la variable.

Asimismo puede declararse una alternativa si la condición no es verdadera, con la sentencia **_else_**. Considere:

```jsx
var edad;
prompt("Ingrese su edad: ");

if(edad > 18)
{
    alert("Ha ingresado al sistema.");
}else
{
    alert("Error. No se puede ingresar al sistema.");
}
// Si la edad es mayor a 18, puede ingresar al sistema. En cambio, si la edad es menor NO puede ingresar al sistema.
```


Los condicionales existen en formas más allá del **_if_**. Por ejemplo, la sentencia _switch_ puede ser usada como un atajo para una serie de sentencias *if...else*.
