# Class29-09

## Que es el hoisting?

El "hoisting" en JavaScript es un comportamiento en el cual las declaraciones de variables y funciones son movidas al principio del ámbito en el que están definidas durante la fase de compilación, antes de que el código se ejecute.

Esto significa que, en términos prácticos, puedes usar una variable o función antes de que hayan sido declaradas en tu código. Sin embargo, ten en cuenta que solo la declaración es movida, no la inicialización (asignación de un valor). Por lo tanto, si intentas usar una variable antes de inicializarla, obtendrás un valor undefined.

Por ejemplo, considera el siguiente código:

javascript
```
console.log(x); // Output: undefined
var x = 10;
```

El comportamiento de hoisting hace que la declaración var x se mueva al principio del ámbito, lo que significa que x existe, pero aún no tiene un valor asignado cuando se imprime en la consola.

Es importante tener en cuenta que este comportamiento es específico para las declaraciones con var y declaraciones de funciones declaradas con la palabra clave function. Las declaraciones let y const no son hoisteadas de la misma manera, y si intentas acceder a ellas antes de su declaración, obtendrás un error.

Por lo tanto, es una buena práctica declarar e inicializar tus variables y funciones antes de usarlas en tu código, independientemente del comportamiento de hoisting. Esto ayuda a mejorar la legibilidad y la mantenibilidad de tu código.

## Partes del for

El bucle `for` en JavaScript es una estructura de control que permite repetir un bloque de código un número específico de veces. Tiene tres partes principales:

1. **Inicialización**: Esta es la primera parte del bucle `for` y se ejecuta solo una vez al principio. Se utiliza para inicializar una variable que actúa como contador o para establecer una condición inicial.

   ```javascript
   for (let i = 0; i < 5; i++) {
     // ...
   }
   ```
   - En este ejemplo, `let i = 0` inicializa una variable `i` con el valor 0.

2. **Condición de Terminación**: Esta es la segunda parte y es evaluada antes de cada iteración del bucle. Si la condición es `true`, el bucle continúa ejecutándose. Si es `false`, el bucle se detiene.

   ```javascript
   for (let i = 0; i < 5; i++) {
     // ...
   }
   ```
   - En este ejemplo, la condición es `i < 5`. Mientras `i` sea menor que 5, el bucle continuará ejecutándose.

3. **Expresión de Iteración**: Esta es la tercera parte del bucle `for`. Se ejecuta después de cada iteración y se utiliza para actualizar la variable de control (en este caso, `i`) y modificar la condición de terminación.

   ```javascript
   for (let i = 0; i < 5; i++) {
     // ...
   }
   ```
   - En este ejemplo, `i++` incrementa el valor de `i` en 1 después de cada iteración.

En el ejemplo completo:

```javascript
for (let i = 0; i < 5; i++) {
  // Código a ejecutar en cada iteración
}
```

- La primera parte (`let i = 0`) inicializa la variable `i`.
- La segunda parte (`i < 5`) es la condición de terminación.
- La tercera parte (`i++`) se ejecuta después de cada iteración.

El código dentro del bloque de un bucle `for` (encerrado en `{}`) se ejecuta repetidamente hasta que la condición de terminación se evalúa como `false`.

Es importante mencionar que cada una de estas partes es opcional, lo que significa que puedes tener un bucle `for` sin inicialización, condición de terminación o expresión de iteración. Esto te permite crear bucles con diferentes comportamientos según tus necesidades.


## Diagrama








