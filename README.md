# Microsoft Build: Reto de .NET

## Escritura de código de C# por primera vez.

### Introducción:

El lenguaje de programación C# permite crear muchos tipos de aplicaciones, por ejemplo:

* Aplicaciones empresariales para capturar, analizar y procesar datos
* Aplicaciones web dinámicas a las que se puede acceder desde un explorador web
* Juegos, tanto en 2D como en 3D
* Aplicaciones financieras y científicas
* Aplicaciones basadas en la nube
* Aplicaciones móviles

¿Pero cómo empezamos a escribir una aplicación?

Todas las aplicaciones están formadas por muchas líneas de código que funcionan conjuntamente para lograr una tarea. Sin duda, la mejor manera de aprender a codificar consiste en *escribir* código. Por lo tanto, le recomendamos que escriba el código al realizar los ejercicios de este módulo y de todos los demás de esta ruta de aprendizaje. Si escribe usted mismo el código de cada ejercicio y resuelve los pequeños problemas de codificación, aprenderá mucho más rápido.

También deberá empezar a aprender los conceptos básicos y seguir desarrollándolos con la práctica y la exploración continuas.

En este módulo, aprenderá a:

* Escribir las primeras líneas de código de C#.
* Use dos técnicas distintas para imprimir un mensaje como salida.
* Diagnostique los errores cuando el código sea incorrecto.
* Identificar distintos elementos de la sintaxis de C#, como operadores, clases y métodos.

Al final de este módulo, podrá escribir código de C# para imprimir un mensaje en la salida estándar de una consola, como el Terminal Windows. Estas líneas de código le permitirán echar un primer vistazo a la sintaxis de C# y le proporcionarán información valiosa de forma inmediata.

### Ejercicio: Escribir el primer código:

En este primer ejercicio práctico, usará C# para imprimir la típica frase de un programador en la salida estándar de una consola.

Escritura de la primera línea de código

Es tradicional entre los desarrolladores de software imprimir la frase "¡Hola mundo!" en la ventana de salida de la consola. Como verá, puede aprender mucho sobre la programación y el lenguaje de programación de C# en este sencillo ejercicio.

### Escribir código en el editor de .NET

El editor de .NET y la consola de salida proporcionan una excelente experiencia en el explorador que resulta ideal para el enfoque de este tutorial. El editor de .NET se encuentra en el lado derecho de esta página web. La consola de salida está por debajo de ella.

1. Escriba este código exactamente como aparece en el editor de .NET de la derecha:

   ```
   Console.WriteLine("Hello World!");
   ```

   Verá una explicación de cómo y por qué funciona pronto. Pero primero, debería experimentarlo en ejecución y asegurarse de que lo ha escrito correctamente. Para ello, ejecutará el código.

   Nota

   Es posible que se sienta tentado a seleccionar `Copy` o `Run` para no tener que escribir. Sin embargo, escribir el código usted mismo tiene algunas ventajas. Escribir el código usted mismo refuerza la memoria y la comprensión, lo que le ayudará a obtener información que no conseguiría de otro modo.

### Ejecución del primer código

1. presione el botón Ejecutar, de color verde
   El botón Ejecutar, de color verde, realiza dos tareas:
   * Compila el código en un formato ejecutable que el equipo pueda entender.
   * Ejecuta la aplicación compilada y, si se escribe correctamente, generará `"Hello World!"`.

### Observación de los resultados

1. En la consola de salida, observe el resultado del código. Debería obtener la salida siguiente:
   **Output**Copiar

   ```
   Hello World!
   ```

### Qué hacer si aparece un mensaje de error

El proceso de escribir código de C# es un  *ejercicio de precisión* . Si escribe incorrectamente un solo carácter, recibirá un mensaje de error en el área de salida al ejecutar el código.

Por ejemplo, si usa incorrectamente una `c` minúscula en la palabra `console`, como se ve a continuación:

```
console.WriteLine("Hello World!");
```

Obtendrá el siguiente mensaje de error:

**Output**

```
(1,1): error CS0103: The name 'console' does not exist in the current context
```

La parte `(1,1)` del comienzo indica la línea y la columna donde se produjo el error. Pero, ¿qué significa este mensaje de error?

C# es un lenguaje que distingue mayúsculas de minúsculas, lo que significa que el compilador de C# considera que las palabras `console` y `Console` son tan diferentes como las palabras `cat` y `dog`. En ocasiones, el mensaje de error puede ser un poco confuso. Deberá conocer el verdadero motivo por el que existe el error, para lo que tendrá que ampliar sus conocimientos sobre la sintaxis de C#.

Del mismo modo, si usó comillas simples (`'`) para rodear la cadena literal `Hello World!`, como se indica a continuación:

```
Console.WriteLine('Hello World!');
```

Obtendrá el siguiente mensaje de error:

**Output**Copiar

```
(1,19): error CS1012: Too many characters in character literal
```

De nuevo, la causa se encuentra en la línea 1, carácter 19. Puede usar el mensaje como una pista para investigar el problema. Pero, ¿qué significa este mensaje de error? ¿Qué es exactamente un "literal de carácter?" Más adelante, obtendrá más información sobre los literales de varios tipos de datos (incluidos los literales de caracteres). Por ahora, tenga cuidado al escribir código.

Afortunadamente, los errores nunca son permanentes. Solo tiene que detectar el error, corregirlo y volver a ejecutar el código.

Si se produjo un error al ejecutar el código, tómese un momento para verlo detenidamente. Examine cada carácter y asegúrese de que ha escrito exactamente esta línea de código.

 Nota

El editor de código supervisa en todo momento el código que se escribe, para lo que realiza una compilación previa a fin de detectar posibles errores. A modo de ayuda, agrega líneas onduladas de color rojo subrayando el código que generará un error.

Errores comunes que comenten los programadores inexpertos:

* Usar letras minúsculas en lugar de `C` mayúsculas en `Console`, o las letras `W` o `L` en `WriteLine`.
* Usar una coma en lugar de un punto entre `Console` y `WriteLine`.
* Olvidar utilizar las comillas dobles o usar comillas simples para rodear la frase `Hello World!`.
* Olvidar el punto y coma al final del comando

Todos estos errores impiden que el código se compile correctamente.

El editor de código resalta los errores previos a la compilación para ayudarle a identificar y corregir fácilmente los errores a medida que desarrolla el código. Puede considerarlo como un corrector ortográfico que le ayuda a corregir errores gramaticales u ortográficos de un documento.

Suponiendo que ha realizado correctamente los pasos anteriores, vamos a continuar.

### Mostrar un nuevo mensaje

En esta tarea, va a marcar como comentario la línea de código anterior y, después, va a agregar nuevas líneas de código en el editor de .NET para imprimir un mensaje nuevo

1. Modifique el código que ha escrito para que vaya precedido de un comentario de código con dos barras inclinadas `//`:

   ```
   // Console.WriteLine("Hello World!");
   ```

   Para crear un comentario de código, anteponga dos barras diagonales `//` a una línea de código. Este prefijo indica al compilador que omita todas las instrucciones de esa línea.

   Los comentarios de código son útiles cuando no está listo para eliminar el código todavía, pero quiere omitirlo por ahora. También puede usar comentarios de código para agregar mensajes para usted o para otros usuarios que más adelante puedan leer el código, recordando lo que hace el código.
2. Agregue nuevas líneas de código para que coincidan con el siguiente fragmento de código:

   ```
   Console.Write("Congratulations!");
   Console.Write(" ");
   Console.Write("You wrote your first lines of code.");
   ```
3. Presione de nuevo el botón Ejecutar, de color verde. Esta vez, obtendrá la salida siguiente.
   **Output**Copiar

   ```
   Congratulations! You wrote your first lines of code.
   ```

### La diferencia entre Console.Write y Console.WriteLine

Las tres líneas de código nuevas que ha agregado demostraban la diferencia entre los métodos [Console.WriteLine()](https://learn.microsoft.com/es-es/dotnet/api/system.console.writeline#system-console-writeline) y [Console.Write](https://learn.microsoft.com/es-es/dotnet/api/system.console.write).

Para imprimir un mensaje completo en la consola de salida, ha empleado la primera técnica, `Console.WriteLine()`. Al final de la línea, agregaba un avance de línea, como cuando se crea una línea de texto con la tecla Intro o Entrar del teclado.

Para imprimir en la consola de salida, pero sin agregar un avance de línea al final, ha usado utilizado la segunda técnica, `Console.Write()`. Por lo tanto, la siguiente llamada a `Console.Write()` imprime otro mensaje en la misma línea.

Enhorabuena, ha escrito sus primeras líneas de código.

### Aprenda cómo funciona

Para entender cómo funciona el código, debe volver atrás y reflexionar sobre los lenguajes de programación. Tenga en cuenta cómo comunica el código los comandos al equipo.

### ¿Qué es un lenguaje de programación?

Los lenguajes de programación, como C#, le permiten escribir las instrucciones que quiere que el equipo lleve a cabo. Cada lenguaje de programación tiene su propia sintaxis, pero después de aprender el primer lenguaje de programación y de intentar aprender otro, pronto se dará cuenta de que todos comparten muchos conceptos similares. El trabajo de un lenguaje de programación consiste en permitir que un usuario exprese su intención de un modo comprensible en lenguaje natural. Las instrucciones que se escriben en un lenguaje de programación se denominan "código fuente" o simplemente "código". Los desarrolladores de software escriben código.

En este momento, un desarrollador puede actualizar y cambiar el código, pero el equipo no puede entenderlo. En primer lugar, el código se debe *compilar* en un formato que el equipo pueda entender.

### ¿Qué es la compilación?

Un programa especial denominado **compilador** convierte el código fuente en un formato diferente que la unidad central de procesamiento (CPU) del equipo puede ejecutar. Cuando en la unidad anterior usó el botón  **Ejecutar** , de color verde, el código que escribió primero se compiló y, luego, se ejecutó.

¿Por qué es necesario compilar el código? Aunque la mayoría de los lenguajes de programación inicialmente parecen crípticos, los usuarios pueden entenderlos más fácilmente que el lenguaje *preferido* del ordenador. La CPU entiende las instrucciones que se expresan al activar o desactivar miles o millones de conmutadores pequeños. Los compiladores tienden un puente entre estos dos mundos, ya que traducen las instrucciones en lenguaje natural a un conjunto de instrucciones comprensibles para los equipos.

### ¿Qué es la sintaxis?

Las reglas para escribir código de C# se denominan sintaxis. Al igual que los lenguajes humanos tienen reglas relacionadas con la puntuación y la estructura de oraciones, los lenguajes de programación de equipos también tienen reglas. Estas reglas definen las palabras clave y los operadores de C# y cómo se unen para formar programas.

Al escribir código en el editor de .NET, es posible que haya observado cambios sutiles en el color de varias palabras y símbolos. El resaltado de sintaxis es una característica útil que empezará a usar para detectar fácilmente errores en el código que no se ajustan a las reglas de sintaxis de C#.

### ¿Cómo funciona el código?

Vamos a centrarnos en la siguiente línea de código que ha escrito:

```
Console.WriteLine("Hello World!");
```

Al ejecutar el código, ha visto que el mensaje `Hello World!` se ha impreso en la consola de salida. Cuando la frase está rodeada de comillas dobles en el código de C#, se denomina  **cadena literal** . En otras palabras, quería literalmente que los caracteres `H`, `e`, `l`, `l`, `o`, etc., se enviasen a la salida.

La parte `Console` se denomina  **clase** . Las clases son las "propietarias" de los métodos, o quizás sería más adecuado decir que los métodos se encuentran dentro de una clase. Para visitar el método, debe saber en qué clase se encuentra. Por ahora, piense en una clase como una manera de representar un objeto. En este caso, todos los métodos que operan en la consola de salida se definen dentro de la clase `Console`.

También hay un punto que separa el nombre de clase `Console` y el nombre de método `WriteLine()`. El punto es el  *operador de acceso al miembro* . En otras palabras, el punto es cómo se "navega" de la clase a uno de sus métodos.

La parte `WriteLine()` se denomina  **método** . Siempre puede identificar un método porque incluye después un conjunto de paréntesis. Cada método tiene un trabajo. El trabajo del método `WriteLine()` consiste en escribir una línea de datos en la consola de salida. Los datos que se imprimen se envían entre los paréntesis de apertura y de cierre como parámetro de entrada. Algunos métodos necesitan parámetros de entrada, a diferencia de otros que no, pero para invocar un método siempre hay que usar los paréntesis después del nombre del método. Los paréntesis se conocen como el  *operador de invocación de método* .

Por último, el punto y coma es el  *operador de final de instrucción* . Una **instrucción** es una instrucción completa de C#. El punto y coma le indica al compilador que ha terminado de escribir el comando.

No se preocupe si no entiende qué significan todas estas ideas y términos. Por ahora, lo que necesita recordar es que si quiere imprimir un mensaje en la consola de salida:

* Use `Console.WriteLine("Your message here");`
* Debe poner en mayúsculas `Console`, `Write` y `Line`.
* Use la *puntuación* correcta, ya que desempeña un papel especial en C#.
* Si comete un error, simplemente detéctelo, corríjalo y vuelva a ejecutar.

 Sugerencia

Cree una hoja de referencia rápida para usarla mientras no memorice ciertos comandos clave.

### Acerca del flujo de ejecución

Es importante entender el flujo de ejecución. En otras palabras, las instrucciones del código se ejecutaron en orden (una línea de cada vez) hasta que no había más instrucciones que ejecutar. Algunas instrucciones requerirán que la CPU espere antes de poder continuar. Se pueden usar otras instrucciones para cambiar el flujo de ejecución.

Ahora comprobaremos lo que ha aprendido. Cada módulo contiene un desafío sencillo, pero, si se queda bloqueado, le daremos una solución. En la unidad siguiente, tendrá la oportunidad de escribir algo de código de C# por su cuenta.

### Comprobación de conocimientos

**1.** ¿Cuál es la diferencia entre `Console.Write` y `Console.WriteLine`?

* [ ] `Console.Write` imprime la salida en una nueva línea.
* [ ] `Console.WriteLine` imprime la salida en una nueva línea.
* [ ] `Console.WriteLine` anexa una nueva línea después de la salida.

### Revisión de la solución

**Completado**100 XP

El siguiente código es una posible solución al desafío de la unidad anterior.

```
Console.WriteLine("This is the first line.");

Console.Write("This is ");
Console.Write("the second ");
Console.Write("line.");
```

Este código es solo  *una posible solución* , entre muchas formas posibles de lograr el mismo resultado. Aun así, debería haber usado los métodos [Console.WriteLine()](https://learn.microsoft.com/es-es/dotnet/api/system.console.writeline#system-console-writeline) y [Console.Write(String)](https://learn.microsoft.com/es-es/dotnet/api/system.console.write#system-console-write(system-string)) para generar la salida deseada.

**Output**

```
This is the first line.
This is the second line.
```

Si la ha creado correctamente, enhorabuena. Continúe en la unidad siguiente para la prueba de conocimientos.

### Resumen

El objetivo era escribir código que mostrara mensajes simples en una consola de salida mientras se familiarizaba con la sintaxis. Ha escrito las primeras líneas de código con la sintaxis básica de C#. Se han identificado dos técnicas para mostrar datos de cadena literales en la consola. Hemos aprendido qué debemos buscar cuando se detecta un error en el código. Y, finalmente, ha identificado los elementos de la sintaxis de C#, como clases y métodos, y el propósito de varios símbolos especiales conocidos como operadores. Ha realizado los primeros pasos para crear aplicaciones más sofisticadas.
