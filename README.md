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


## Introducción al desarrollo web mediante Visual Studio Code.

Para empezar a trabajar con el desarrollo web, cree un proyecto web sencillo en Visual Studio Code que contenga una página web, un archivo CSS y un archivo JavaScript. Vea cómo usar herramientas de desarrollo en el explorador para comprobar su trabajo.

### Objetivos de aprendizaje

En este módulo, practicará cómo:

* Crear una página web básica con HTML
* Aplicar estilos a los elementos de una página mediante CSS
* Crear temas con CSS
* Adición de compatibilidad para cambiar entre temas con JavaScript
* Revisar el sitio web con las herramientas de desarrollo del explorador

### Introducción

Es impresionante lo que se puede hacer hoy en día en Internet. Puede crear experiencias web que se ejecuten en todos los dispositivos, incluyan todo tipo de contenido multimedia, realicen cálculos complicados e incluso creen aplicaciones que tengan la apariencia de aplicaciones nativas.

Si le interesa empezar hoy mismo con el desarrollo web, puede encontrarse ante un conjunto abrumador de opciones. En este módulo, se mostrarán los componentes básicos de un sitio web y algunas herramientas que puede usar para empezar a desarrollarlo. Deberá usar HTML, CSS y JavaScript conjuntamente para crear un sitio web. Asimismo, usará las herramientas de desarrollo del explorador para comprender lo que está sucediendo.

Con estos conocimientos fundamentales, tendrá un mejor contexto para tomar decisiones en el futuro al crear sitios web. Por ejemplo, si debe elegir plataformas de JavaScript o crear sus propias funciones de JavaScript para crear un sitio web.

Para empezar, echemos un vistazo adonde queremos ir.

### Escenario

Imagine que es un desarrollador web al que se le ha pedido que el sitio web de su empresa sea atractivo para una variedad más amplia de clientes. Para que sus clientes puedan personalizar su experiencia en su sitio web, decide agregar compatibilidad con temas claros y oscuros. Puede crear un sitio web de prueba conceptual sencillo para mostrar la compatibilidad con temas mediante CSS y escribir una función de JavaScript para cambiar entre dichos temas.

Una vez completado, el sitio web tendrá un aspecto similar al de este ejemplo cuando se seleccione el tema oscuro:

[![Captura de pantalla en la que se muestra el sitio web completado con su tema oscuro habilitado.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/themed-website.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/themed-website.png#lightbox)

### ¿Qué hay en una página web?

El contenido, el estilo y la lógica interactiva se separan en archivos HTML, CSS y JavaScript, respectivamente. Un principio de diseño en la programación moderna es la  *separación de los intereses* . Dos de los muchos motivos para separar los intereses son la simplicidad y la reutilización. Por ejemplo, al aplicar estilo a elementos HTML con CSS, puede simplificar el código HTML. En lugar de codificar el aspecto dentro de cada elemento, puede aplicar estilos CSS a todos los elementos de una página, independientemente de la complejidad de la página. Además, puede vincular varias páginas HTML a un único archivo CSS, lo que puede ayudarle a simplificar una apariencia coherente en todo el sitio web.

### Ejercicio: Configuración de la estructura de la aplicación web

Hay diferentes maneras de crear y administrar proyectos de sitio web. Algunas de estas diferencias dependen de las herramientas específicas que tenga y de las preferencias de la organización. Al crear un sitio web, es habitual que la estructura del proyecto cambie con el tiempo a medida que se vuelve más complicado. La clave consiste en mantener la apariencia de organización, y existen estrategias comunes que ayudan a que así sea. Los proyectos de gran tamaño suelen requerir un mayor grado de cuidado y atención para que muchos usuarios puedan mantenerlo todo organizado.

En esta unidad, creará una estructura de proyecto pequeña con Visual Studio Code. El proyecto tendrá tres archivos: un archivo HTML, un archivo CSS y un archivo JavaScript. También agregará una extensión de Visual Studio Code para simplificar la ejecución del sitio web en el explorador.

### Creación de una carpeta nueva para su sitio web

1. Abra Visual Studio Code.
   Al abrir Visual Studio Code, se abre la página de  **Bienvenida** . Tenga en cuenta que puede crear un archivo o abrir una carpeta en la lista  **Inicio** .
   [![Captura de pantalla de la pantalla Introducción de Visual Studio Code.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-get-started.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-get-started.png#lightbox)
   Si la **página principal** no aparece, puede mostrarla seleccionando **Ayuda > Bienvenido** en el menú. (También puede mostrar la página **principal** abriendo la **Paleta de comandos** con el método abreviado de teclado Mayús+Ctrl+P en un equipo con Windows o Mayús+Cmd+P en macOS, o seleccionando **Ver > Paleta de comandos** en el menú Visual Studio Code. Cuando se muestre la  **Paleta de comandos** , escriba **>Ayuda: principal** en el campo de búsqueda para abrir la página  **principal** ).
2. Seleccione **Abrir carpeta** en la lista **Inicio** de la **página principal** o seleccione **Archivo > Abrir carpeta** en el menú de Visual Studio Code.
   [![Captura de pantalla del cuadro de diálogo Abrir carpeta del sistema operativo Windows.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-open-folder.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-open-folder.png#lightbox)
   Al abrir una carpeta, el sistema operativo tiene una opción de menú para crear una  **Nueva carpeta** .
3. Vaya a la ubicación donde desea crear la nueva carpeta para el sitio web y seleccione  **Nueva carpeta** .
4. Asigne a la carpeta el nombre **simple-website** y seleccione  **Seleccionar carpeta** .
   Importante

   Si aparece el cuadro de diálogo  **Visual Studio Code** , seleccione  **Confiar en los autores de todos los archivos de la carpeta principal...** ; se trata de la característica de Workspace Trust que permite decidir si las carpetas del proyecto deben permitir o restringir la ejecución automática de código. Acaba de crear la carpeta, por lo que es segura.

### Creación de algunos archivos

1. Cree un archivo; para ello, seleccione **Archivo > Nuevo archivo** en el menú o use Control+N en Windows o Comando+N en macOS.
2. Guarde el archivo mediante Control+S en Windows o Comando+S en macOS.
3. Escriba `index.html` como nombre de archivo y, a continuación, seleccione  **Guardar** .
4. Repita los pasos anteriores para crear dos archivos más, `main.css` y `app.js`. Cuando haya terminado, en el explorador de Visual Studio Code, verá que la carpeta del proyecto **simple-website** contiene el siguiente archivo, que incluye el sitio web:

   * index.html
   * main.css
   * app.js

   [![Captura de pantalla de los archivos en la vista del explorador de Visual Studio Code.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-explorer-view.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-explorer-view.png#lightbox)

Puede crear un sitio web incluyendo todo el código HTML, los estilos CSS y el código JavaScript en un único archivo. Sin embargo, en este ejercicio está usando un archivo HTML para el contenido, un archivo CSS para los estilos y un archivo JavaScript para la interactividad.

La configuración de tres archivos ayuda a mantener organizado el proyecto del sitio web. La separación de contenido, estilos y lógica es un ejemplo de  *mejora progresiva* . Si JavaScript no está habilitado o no es compatible con los clientes, HTML y CSS seguirán funcionando. Sin embargo, si CSS no es compatible con los clientes, al menos su contenido HTML aparecerá.

### Instalación de extensiones o paquetes

Puede ampliar la funcionalidad de Visual Studio Code mediante el marketplace de extensiones. Tenga en cuenta que estas extensiones son recursos desarrollados por la comunidad y que suele haber varias soluciones para el mismo tipo de característica. Puede instalar las extensiones de forma individual en el editor, o bien varias al mismo tiempo con la línea de comandos.

Para el desarrollo web, todo lo que necesita ahora es  **open-in-browser** . Esta extensión lo ayuda a abrir rápidamente el sitio web en el explorador predeterminado, en lugar de copiar y pegar la dirección URL del archivo en el explorador.

Para instalar esta extensión, siga estos pasos:

1. Seleccione el icono **Extensiones** en la **barra de actividad** vertical (panel izquierdo).
2. Escriba "abrir en" en el cuadro de búsqueda y, a continuación, seleccione la extensión **abrir en el explorador** publicada por  *TechER* .
3. Seleccione  **Instalar** , y Visual Studio Code instalará la extensión.
   [![Captura de pantalla en la que se muestra la barra lateral de la extensión de Visual Studio Code con las palabras ](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-get-extension.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-get-extension.png#lightbox)
4. Vuelva al  **Explorador** ; para ello, haga clic en el icono superior de la **barra de actividad** o use Control+Maýus-E en Windows o Comando+Maýus-E en macOS.

Bien hecho. El proceso de instalación y configuración tarda un poco más, pero solo debe realizarse una vez. Ahora ya está listo para crear un sitio web.

### Ejercicio: Adición de HTML básico a la aplicación web

Por el momento, el sitio web tiene un archivo HTML vacío. Se agregará algo de código. El objetivo es usar el lenguaje de marcado de hipertexto (HTML) para describir la página web que deben mostrar los exploradores de los clientes. ¿No sería buena idea tener una plantilla inicial? De forma cómoda, los editores pueden rellenar automáticamente parte del texto reutilizable o la estructura HTML típica.

En esta unidad, agregará contenido HTML básico, abrirá la página HTML en un explorador y echará el primer vistazo a las herramientas de desarrollo.

### Incorporación de código HTML

Visual Studio Code proporciona compatibilidad básica para la programación de HTML desde el principio. Incluye resaltado de sintaxis, finalizaciones inteligentes con IntelliSense y formato personalizable.

1. Abra el sitio web en **Visual Studio Code** y, a continuación, abra el archivo `index.html` seleccionando el archivo `index.html` en el  **Explorador** .
2. En la página `index.html`, escriba `html:5` y después seleccione ENTRAR. El código de plantilla HTML5 se agrega al archivo.
   Nota

   Si el código de plantilla HTML5 no se agrega al archivo `index.html`, pruebe a cerrar y volver a abrir el archivo.
3. Edite el código para que se parezca al siguiente. A continuación, guarde el archivo mediante Control+S en Windows o Comando+S en macOS.
   **HTML**Copiar

   ```
   <!DOCTYPE html>
   <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Document</title>
   </head>
   <body>

   </body>
   </html>
   ```

Ha habido diferentes versiones de HTML. El  *tipo de documento* `<!DOCTYPE html>` indica que este documento HTML contiene código HTML5.

Si bien no vamos a profundizar demasiado en el significado de todos los elementos HTML, sí señalaremos algunos elementos importantes. La etiqueta `meta` indica información de *metadatos* que normalmente no será visible para el usuario que visualice la página, a menos que vea el código fuente en su explorador. Los elementos o etiquetas meta proporcionan información descriptiva sobre la página web. Por ejemplo, ayuda a los motores de búsqueda a procesar la información de las páginas web que se devuelve en los resultados de la búsqueda.

El *juego de caracteres* (`charset`) para UTF-8 puede parecer insignificante, pero es fundamental para establecer cómo interpretan los caracteres los equipos. Si faltan los metadatos del juego de caracteres, la seguridad podría ponerse en peligro. Hay bastante historia e información técnica detrás del atributo charset, pero lo importante de este ejercicio es que el código reemplazable de **VS Code** proporciona algunos valores de manera predeterminada.

### Edición del elemento head

El elemento `<head>` del código HTML contiene información sobre el sitio web no visible dentro de la pestaña del explorador.

Los *metadatos* definen datos sobre el documento HTML, como el juego de caracteres, los scripts y el explorador en el que se abre la página web.

El *título* de una página web aparece en la parte superior de la ventana del explorador y es significativo por muchos motivos. Por ejemplo, el título lo usan y lo muestran los motores de búsqueda. Vamos a agregar un título.

 Importante

A partir de ahora, los puntos suspensivos (...) indican que el código anterior o siguiente se ha declarado previamente. Debe haber suficiente código proporcionado como contexto para realizar los cambios necesarios o actualizar el trabajo, pero no debe copiar ni pegar los puntos suspensivos en el código.

1. En el editor, modifique el elemento `<title>` para que se parezca al ejemplo siguiente.
   **HTML**Copiar

   ```
   ...
   <head>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple website</title>
   ...
   ```

Para aplicar estilos a los elementos HTML de la página web, podría escribir el código CSS directamente en el encabezado de la página web. La escritura de CSS en la página HTML se denomina  *CSS interno* . Pero un procedimiento recomendado consiste en separar la estructura HTML y los estilos CSS. Tener una página CSS independiente se denomina  *CSS externa* . El código suele ser más fácil de leer cuando es conciso y compartimentado. Puede usar una o varias hojas de estilos externas para dar servicio a varias páginas web. En lugar de actualizar cada página HTML con código CSS replicado, puede realizar cambios en un único archivo CSS y hacer que esas actualizaciones se apliquen a todas las páginas web dependientes. Vamos a vincular a una hoja de estilos externa.

1. En el editor de  **VS Code** , agregue una línea en blanco después del elemento `<title>`, escriba `link` y, a continuación, seleccione ENTRAR. **VS Code** debe agregar la siguiente línea al archivo `index.html`.
   **HTML**Copiar

   ```
   <link rel="stylesheet" href="">
   ```
2. Actualice `href=` a `href="main.css"` y guarde el archivo presionando Control+S en Windows o Comando+S en macOS.
   **HTML**Copiar

   ```
   ...
   <head>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Task List</title>
     <link rel="stylesheet" href="main.css">
   </head>
   ...
   ```

### Edición del cuerpo

Para empezar, ahora se rellenará el elemento `<body>`.

El elemento `<body>` contiene el contenido del sitio web visible para sus clientes en sus exploradores.

1. Agregue un elemento `<h1>` de  *encabezado* , seguido de un elemento `<p>` de *párrafo* y, después, cree una  *lista sin ordenar* `<ul>` que contenga varios elementos `<li>` de  *elementos de lista* .
2. Edite el código, o cópielo y péguelo, para que tenga un aspecto similar al siguiente ejemplo.
   **HTML**Copiar

   ```
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="utf-8">
       <meta http-equiv="X-UA-Compatible" content="IE=edge">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Simple website</title>
       <link rel="stylesheet" href="main.css">
     </head>
     <body>
       <h1>Task List</h1>
       <p id="msg">Current tasks:</p>
       <ul>
         <li class="list">Add visual styles</li>
         <li class="list">Add light and dark themes</li>
         <li>Enable switching the theme</li>
       </ul>
     </body>
   </html>
   ```

Se puede usar un atributo ID (que se usa en el elemento `<p>`) para aplicar estilo a un elemento, mientras que el atributo de clase (que se usa en el elemento `<li>`) sirve para aplicar un estilo a todos los elementos de la misma clase.

Antes del paso siguiente, asegúrese de que el archivo se guarda presionando Control+S o Comando+S.

### Abrir en el explorador

Puede obtener una vista previa local de la página web si abre el archivo HTML en un explorador. En lugar de una dirección de sitio web que comienza con `https://`, el explorador apunta a la ruta de acceso del archivo local, que debería tener un aspecto similiar a `C:/dev/simple-website/index.html`.

* Para obtener una vista previa con  **Visual Studio Code** , haga clic con el botón derecho en `index.html` y seleccione **Abrir en el explorador predeterminado** o seleccione el archivo `index.html` y use el método abreviado de teclado Alt+B.
  [![Captura de pantalla del elemento de menú contextual Abrir en el explorador Visual Studio Code.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-open-in-browser.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/vs-code-open-in-browser.png#lightbox)
  Importante

  Si tiene problemas, asegúrese de que hace clic con el botón derecho en el icono o el texto del nombre de archivo. Si aparece el cuadro de diálogo  **Visual Studio Code** , seleccione **Yes, I trust the authors** (Sí, confío en los autores); se trata de la característica de Workspace Trust que permite decidir si las carpetas del proyecto deben permitir o restringir la ejecución automática de código. Acaba de crear el archivo, por lo que es seguro.

  La página web se abre en el explorador predeterminado.

### Visualización de la página con las herramientas de desarrollo

Puede inspeccionar una página web mediante las herramientas para desarrolladores del explorador. Vamos a probarlo.

1. Abra Herramientas de desarrollo; para ello, haga clic con el botón derecho del ratón en la página web y seleccione  **Inspeccionar** , o bien pruebe estos métodos abreviados de teclado:

   * Presione el método abreviado de teclado para  **Herramientas de desarrollo** , que es F12.
   * Presione Ctrl+Mayús+I en Windows y Linux u Opción+Comando+I en Mac.

   Estos métodos abreviados de teclado funcionan en  **Microsoft Edge** , **Chrome** y  **Firefox** . Si usa  **Safari** , consulte la información sobre las [Herramientas de desarrollo web](https://developer.apple.com/safari/tools/). Cuando esté instalado, seleccione **Safari > Preferencias** y, luego, elija  **Avanzado** . En la parte inferior del panel, active la casilla  **Mostrar el menú Desarrollo en la barra de menús** . Seleccione  **Desarrollo > Mostrar inspector web** . Para más información, consulte la documentación de Inspector web de Safari.
   Para obtener más información sobre cómo abrir las Herramientas de desarrollo y las principales características disponibles, consulte el artículo [Información general sobre las Herramientas de desarrollo](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/overview).
2. Haga clic en la pestaña **Elements** (Elementos).
   [![Captura de pantalla en la que se muestra una ventana del explorador con el sitio web y Herramientas de desarrollo junto a ella con la pestaña Elementos seleccionada.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/developer-tools-elements-tab.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/developer-tools-elements-tab.png#lightbox)
3. Mueva el mouse sobre los elementos HTML que se muestran en la pestaña **Elementos** y expanda el contenido de los distintos elementos.

La pestaña **Elementos** de las herramientas de desarrollo muestran el modelo de objetos de documento (DOM) tal como se representa en el explorador. Al depurar, a menudo es importante ver cómo el explorador interpreta el código fuente.

La inspección de la página en un explorador proporciona todo tipo de información útil y puede ayudar a solucionar problemas. Con el inspector también puede ver detalles de CSS, como verá en la sección siguiente.

### Ejercicio: Aplicación de estilos al código HTML con CSS

Las Hojas de estilos en cascada (CSS) le permiten especificar la apariencia de la página. La idea básica es definir cuál debe ser el estilo para los elementos que se usan en las páginas HTML. Mientras que los elementos HTML definen el contenido, los estilos CSS definen el aspecto de este contenido.

Por ejemplo, puede aplicar esquinas redondeadas o asignar un fondo degradado a un elemento. También puede usar CSS para especificar el aspecto de los hipervínculos y su respuesta al interactuar con ellos. También puede realizar diseños de página sofisticados y efectos de animación.

Puede aplicar estilos a elementos concretos, a todos los elementos de un tipo en particular o usar clases para aplicar estilos a muchos elementos diferentes.

En este ejercicio, aplicará estilos CSS a los elementos de la página HTML y agregará código CSS para definir los temas claros y oscuros. También comprobará los resultados en las herramientas de desarrollo del explorador.

### CSS externas

En la unidad anterior sobre HTML, ha creado un vínculo a un archivo CSS externo desde HTML.

**HTML**

```
...
<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Task Timeline</title>
  <link rel="stylesheet" href="main.css">
...
```

Una ventaja de las CSS externas es que se pueden vincular varias páginas HTML al mismo archivo CSS. Si realiza un cambio en la CSS, se actualizará el estilo de cada página. El uso de un archivo HTML para el contenido de la página, de un archivo CSS para aplicar estilos y de un archivo JavaScript para la interacción se denomina  *separación de preocupaciones* .

Tal como se ha descrito anteriormente, también puede escribir CSS directamente en HTML, lo que se denomina  *CSS interno* . Incluso para un sitio web básico, hay tantas reglas CSS que la página HTML se puede desordenar muy rápidamente. Con más de una página, la misma CSS se repetiría con frecuencia y sería difícil de administrar.

### Reglas de CSS

Las reglas CSS son la forma en que se aplican los estilos a los elementos HTML. Las reglas CSS tienen un  **selector** , que se usa para expresar a qué elemento o elementos se deben aplicar los estilos.

En  **Visual Studio Code** , abra el archivo `main.css` y escriba lo siguiente.

**css**

```
body {
    font-family: monospace;
}

ul {
    font-family: helvetica;
}
```

El fragmento de código anterior contiene dos reglas. Cada regla tiene lo siguiente:

* Un  *Selector* . `body` y `ul` son los selectores de las dos reglas y se usan para seleccionar a qué elementos se aplican los estilos.
* Una llave de apertura (`{`).
* Una lista de *declaraciones* de estilo que determinan el aspecto que deben tener los elementos seleccionados.
* Una llave de cierre (`}`).

Por ejemplo, el selector `ul` selecciona el elemento HTML `<ul>` de la página para aplicarle estilos. La declaración es `font-family: helvetica` y determina cuál debe ser el estilo. El *nombre de la propiedad* es `font-family` y el *valor* es `helvetica`.

Como verá a continuación, puede definir nombres personalizados propios para los elementos.

### Selectores

Los selectores *id.* y *clase* permiten aplicar estilos a los nombres de atributo personalizados del código HTML. Un identificador se usa para aplicar estilo a un elemento, mientras que las clases se pueden usar para aplicar estilo a varios elementos.

1. Copie el código siguiente en el archivo CSS, después de la llave de cierre del selector `ul` que ha agregado antes.
   **css**

   ```
   li {
     list-style: circle;
   }

   .list {
     list-style: square;
   }

   #msg {
     font-family: monospace;
   }
   ```

   El código anterior contiene tres reglas CSS, y las dos últimas usan atributos personalizados para seleccionar elementos: `.list` y `#msg`.

   * `.list` es un  *selector de clases* . Cada elemento HTML que contenga un atributo `class` establecido en `list` obtendrá los estilos definidos dentro de este selector.
   * `#msg` es un  *selector de Id* . El elemento HTML que tenga su atributo `id` establecido en `msg` obtendrá los estilos definidos dentro de este selector.

   Los nombres que use para los selectores pueden ser arbitrarios, siempre que coincidan con lo que haya definido en el código HTML.
2. Guarde el trabajo mediante Control+S en Windows o Comando+S en macOS.

### Visualización en un explorador

1. Para obtener una vista previa con  **VS Code** , haga clic con el botón derecho en el nombre de archivo `index.html` y seleccione  **Abrir en el explorador predeterminado** .
   Importante

   Aunque solo estuviera editando el archivo `main.css`, para obtener una vista previa de los cambios, debe seleccionar el archivo `index.html`.

   La página web se abre en el explorador predeterminado.
   [![Captura de pantalla del sitio web con los estilos de fuente aplicados.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/applied-font-styles.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/applied-font-styles.png#lightbox)

¿Los estilos de fuente son los que esperaba ver? Es interesante cómo los estilos aplicados a `<body>` se heredan en el elemento `<h1>`. No hemos definido nada para `<h1>`, pero aun así ha obtenido la fuente que se definió en `<body>`. Este mecanismo de herencia de elementos principales a sus descendientes es uno de los aspectos clave de CSS. Sin embargo, los elementos `<li>` tienen una fuente diferente, que reemplaza la que se definió en `<body>`, porque también son descendientes del elemento `<ul>` para el que definió un estilo.

Tenga en cuenta que, al usar **Abrir en el explorador predeterminado** en  **VS Code** , cada vez se abre una nueva pestaña en el explorador. Para evitar abrir una pestaña nueva, puede volver a cargar la pestaña que ya contiene su sitio web.

Para volver a cargar la pestaña, presione F5, que es el método abreviado de teclado para actualizar, o bien presione Ctrl+R en Windows o Linux, y Comando+R en Mac.

### Incorporación de un tema claro

A continuación, agregará compatibilidad con un tema de color para el sitio web. Comience por definir un tema de color claro mediante códigos de color hexadecimal.

1. En el archivo CSS, agregue el código siguiente al final del archivo.
   **css**

   ```
   .light-theme {
     color: #000000;
     background: #00FF00;
   }
   ```

   En este ejemplo, `#000000` especifica el negro para el color de fuente y `#00FF00` especifica el verde para el color de fondo.
2. En el archivo HTML, actualice el elemento `<body>` con un nombre de clase, `light-theme`, para que el selector de clases del tema claro aplique correctamente los estilos.
   **HTML**

   ```
   <body class="light-theme">
   ```

### Visualización en un explorador

* Para obtener una vista previa con  **Visual Studio Code** , haga clic con el botón derecho en `index.html` y, a continuación, seleccione  **Abrir en el explorador predeterminado** , o bien vuelva a cargar la pestaña anterior presionando F5.
  Observe que aparece el tema claro con un fondo verde.
  [![Captura de pantalla del sitio web con su tema claro aplicado.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/light-theme.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/light-theme.png#lightbox)

### Visualización de CSS aplicado

1. En la vista del explorador, abra Herramientas de desarrollo.
   Haga clic con el botón derecho en la página y seleccione  **Inspeccionar** , o bien seleccione el método abreviado de teclado F12 o Ctrl+Mayús+I.
2. Seleccione la pestaña **Elementos** y, dentro de la pestaña  **Elementos** , seleccione la pestaña **Estilos** (ya debería estar seleccionada de manera predeterminada).
3. Mantenga el puntero sobre los distintos elementos HTML y, a medida que seleccione algunos, observe cómo las herramientas de desarrollo muestran qué estilos se han aplicado a dichos elementos en la pestaña  **Estilos** .
4. Seleccione el elemento `<body>`. Observe el elemento `light-theme` aplicado.
5. Seleccione el elemento `<ul>` de la lista sin ordenar. Observe el estilo personalizado `font-family: helvetica;`, que reemplaza el estilo del elemento `<body>`.

[![Captura de pantalla del sitio web con su tema claro aplicado y las Herramientas de desarrollo junto a él en las que se muestra el panel Elementos con el código HTML y CSS.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/light-theme-in-dev-tools.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/light-theme-in-dev-tools.png#lightbox)

Para obtener más información sobre cómo ver los estilos CSS en las Herramientas de desarrollo, consulte el artículo [Comenzar a ver y cambiar CSS](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/css/).

### Incorporación de un tema oscuro

En el tema oscuro, establecerá la infraestructura como preparación para la próxima unidad, en la que habilitará el cambio de tema en la página web.

Para agregar compatibilidad con un tema oscuro para su CSS, siga estos pasos.

1. Agregue algunas constantes a la raíz de la página en la parte superior del archivo CSS.
   **css**

   ```
   :root {
     --green: #00FF00;
     --white: #FFFFFF;
     --black: #000000;
   }
   ```

   El selector `:root` representa el elemento `<html>` en la página HTML. Para este tipo de tarea, un procedimiento recomendado es definir un conjunto de variables de CSS globales en una regla CSS con el selector `:root`. En este ejemplo, ha definido tres variables de color. A continuación, podrá usar estas variables en otras reglas CSS.
2. Al final del archivo CSS, reemplace la regla `light-theme` por el código siguiente para actualizarlo y agregar el selector `dark-theme`.
   **css**

   ```
   .light-theme {
     --bg: var(--green);
     --fontColor: var(--black);
   }
   .dark-theme {
     --bg: var(--black);
     --fontColor: var(--green);
   }
   ```

   En el código anterior, ha definido dos variables nuevas, `bg` y `fontColor`, que especifican un color de fuente y de fondo. Estas variables usan la palabra clave `var` para establecer sus valores de propiedad en las variables especificadas anteriormente en el selector `:root`.
3. A continuación, en el archivo CSS, reemplace el selector `body` actual por el código siguiente.
   **css**

   ```
   body {
     background: var(--bg);
     color: var(--fontColor);
     font-family: helvetica;
   }
   ```

   En este ejemplo, se usa el selector `body` para establecer las propiedades `background` y `color` y, dado que los elementos visibles en la página web están dentro del elemento `<body>`, heredarán los colores establecidos en `<body>`.
4. En el archivo CSS, quite las reglas con los selectores `#msg` y `ul` para que también hereden la misma fuente de `<body>`.
5. Para ver el tema oscuro, abra el archivo `index.html`, edite manualmente el tema predeterminado del atributo de clase `<body>` en tema oscuro (`dark-theme`) y, a continuación, vuelva a cargar la página en el explorador.
   [![Captura de pantalla del sitio web con su tema oscuro aplicado y las Herramientas de desarrollo junto a él.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/dark-theme.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/dark-theme.png#lightbox)
6. Edite el atributo de clase `<body>` para volver a cambiar el valor predeterminado al tema claro.

En la unidad siguiente, usará JavaScript para proporcionar interactividad y permitir cambiar los temas.


### Ejercicio: Adición de interactividad con JavaScript

JavaScript (o  *ECMAScript* ) es un lenguaje de programación que le ayuda a agregar interactividad a las páginas web.

Por ejemplo, puede usar JavaScript para definir el comportamiento que se va a producir cuando un usuario selecciona un botón, como por ejemplo, abrir una ventana emergente. Con JavaScript, puede agregar o quitar contenido de una página web sin volver a cargarla.

En esta unidad, configurará un archivo JavaScript de ejemplo para la página web. Creará un botón para cambiar entre los temas claro y oscuro. A continuación, adjuntará el botón al código JavaScript que realiza el cambio de tema real. Por último, comprobará el proyecto terminado en las herramientas de desarrollo del explorador.

### Vínculo a JavaScript

Al igual que CSS, puede agregar JavaScript directamente al archivo HTML, pero un procedimiento recomendado es guardar el código JavaScript en un archivo independiente. Agregar el código JavaScript a un archivo independiente facilita su reutilización en varias páginas web. Por ejemplo, podría crear una alerta emergente agregando `<script>alert('Hello World')</script>` en cualquier parte del cuerpo de las páginas web; sin embargo, es mejor agregar el código JavaScript a un archivo independiente que se pueda vincular a todos los archivos que necesiten su funcionalidad personalizada.

La etiqueta de script HTML `<script>` nos permitirá vincular a un archivo JavaScript externo, que es la forma en que configurará la aplicación web en este ejercicio.

1. En  **VS Code** , abra el archivo `index.html`.
2. En una nueva línea antes del elemento `script:src` de cierre, escriba `</body>` y después seleccione ENTRAR. Las etiquetas de apertura y cierre de un script se agregan al código.
3. Modifique el elemento `<script>` para cargar el archivo `app.js` como se muestra en el ejemplo siguiente, y asegúrese de que se encuentra después del elemento `</ul>` de cierre de la lista.
   **HTML**

   ```
   ...
   <ul>
     <li class="list">Add visual styles</li>
     <li class="list">Add light and dark themes</li>
     <li>Enable switching the theme</li>
   </ul>
   <script src="app.js"></script>
   ...
   ```

El elemento `<script>` se puede colocar en `<head>` o en otra parte de `<body>`. Sin embargo, colocar el elemento `<script>` al final de la sección `<body>` permite que primero se muestre todo el contenido de la página y, después, se cargue el script.

### Incorporación de tolerancia a errores

1. En el archivo HTML, agregue un elemento `<noscript>` después de la etiqueta `</script>` de cierre, que se puede usar para mostrar un mensaje si JavaScript está desactivado.
   **HTML**

   ```
   <script src="app.js"></script>
   <noscript>You need to enable JavaScript to view the full site.</noscript>
   ```

   La adición del elemento `<noscript>` es un ejemplo de *tolerancia a errores* o  *degradación correcta* . Al utilizar el elemento `<noscript>`, su código puede detectar y planificar cuando una característica no es compatible o no está disponible.
2. Guarde los cambios con el método abreviado de teclado Control+S en Windows o Comando+S en macOS.

### Establecimiento del modo strict

JavaScript se diseñó para ser fácil de aprender y permite que el desarrollador cometa ciertos errores. Por ejemplo, JavaScript no produce un error al usar una variable mal escrita y, en su lugar, crea una nueva variable global. Aunque tener menos errores es tentador al empezar a aprender JavaScript, puede llevar a escribir código más difícil de optimizar para los exploradores y más difícil de depurar.

Cambie al modo strict para obtener errores más útiles al cometer equivocaciones.

* En  **VS Code** , abra el archivo `app.js` y escriba lo siguiente.
  **JavaScript**

  ```
  'use strict';
  ```

### Adición de un botón

Necesita un modo de permitir que el usuario cambie entre los temas claro y oscuro en la página web. En este ejercicio, implementará esa funcionalidad con un elemento `<button>` HTML.

1. En el archivo HTML, agregue un elemento `<button>`. Coloque el botón al final de la lista dentro de un elemento `<div>`.
   **HTML**

   ```
   ...
   <ul>
     <li class="list">Add visual styles</li>
     <li class="list">Add light and dark themes</li>
     <li>Enable switching the theme</li>
   </ul>
   <div>
     <button class="btn">Dark</button>
   </div>
   <script src="app.js"></script>
   ...
   ```

   Observe que el elemento `<button>` de este ejemplo tiene un atributo *class* que usará para aplicar estilos CSS.
2. En el archivo CSS, agregue una regla nueva con un n selector de clases `.btn` para el botón HTML. Para que los colores de los botones sean distintos de los colores generales de los temas claro u oscuro, establezca las propiedades `color` y `background-color` en esta regla. Invalidarán las predeterminadas establecidas en la regla `body` del archivo CSS.
   **css**

   ```
   .btn {
     color: var(--btnFontColor);
     background-color: var(--btnBg);
   }
   ```
3. A continuación, modifique la regla `.btn` para agregar algunos estilos para el tamaño, la forma, la apariencia y la ubicación del botón. El CSS siguiente crea un botón redondo a la derecha del encabezado de la página.
   **css**

   ```
   .btn {
     position: absolute;
     top: 20px;
     left: 250px;
     height: 50px;
     width: 50px;
     border-radius: 50%;
     border: none;
     color: var(--btnFontColor);
     background-color: var(--btnBg);
   }
   ```
4. A continuación, actualice el CSS para el tema claro y oscuro. Defina algunas variables nuevas, `--btnBg` y `--btnFontColor`, para especificar el color de fondo y el color de la fuente del botón.
   **css**

   ```
   .light-theme {
     --bg: var(--green);
     --fontColor: var(--black);
     --btnBg: var(--black);
     --btnFontColor: var(--white);
   }

   .dark-theme {
     --bg: var(--black);
     --fontColor: var(--green);
     --btnBg: var(--white);
     --btnFontColor: var(--black);
   }
   ```

### Agregar un controlador de eventos

Para hacer que el botón realice alguna acción cuando lo seleccione, necesita un controlador de eventos en el archivo JavaScript. Un controlador de eventos es una forma de ejecutar una función JavaScript cuando se produce un evento en la página. Para el botón, vamos a agregar un controlador de eventos para el evento `click`; la función del controlador de eventos se ejecuta cuando se produce el evento `click`.

Para poder agregar el controlador de eventos, necesita una referencia al elemento de botón.

1. En el archivo JavaScript, use `document.querySelector` para obtener la referencia de botón.
   **JavaScript**

   ```
   const switcher = document.querySelector('.btn');
   ```

   La función `document.querySelector` usa selectores de CSS, igual que los que ha usado en el archivo CSS. `switcher` ahora es una referencia al botón de la página.
2. A continuación, agregue el controlador de eventos para el evento `click`. En el código siguiente, agregue un cliente de escucha para el evento `click` y defina una función de controlador de eventos que el explorador ejecutará cuando se produzca el evento `click`.
   **JavaScript**

   ```
   switcher.addEventListener('click', function() {
       document.body.classList.toggle('light-theme');
       document.body.classList.toggle('dark-theme');
   });
   ```

En el código anterior, ha usado el método `toggle` para modificar el atributo de clase del elemento `<body>`. Este método agrega o quita automáticamente las clases `light-theme` y `dark-theme`. Este código aplica los estilos oscuros en lugar de los estilos claros al hacer clic y, a continuación, los estilos claros en lugar de los oscuros al volver a hacer clic.

Pero también es necesario actualizar la etiqueta del botón para mostrar el tema correcto, por lo que debe agregar una instrucción `if` para determinar el tema actual y actualizar la etiqueta del botón.

El código JavaScript completo debería verse así.

**JavaScript**

```
'use strict';

const switcher = document.querySelector('.btn');

switcher.addEventListener('click', function() {
    document.body.classList.toggle('light-theme');
    document.body.classList.toggle('dark-theme');

    const className = document.body.className;
    if(className == "light-theme") {
        this.textContent = "Dark";
    } else {
        this.textContent = "Light";
    }
});
```

Por convención de JavaScript, se usan *mayúsculas y minúsculas concatenadas* para los nombres de variables con más de una palabra; por ejemplo, la variable `className`.

### Mensaje de consola

Como desarrollador web, puede crear mensajes ocultos que no aparecerán en la página web, pero que se pueden leer en las herramientas de desarrollo, en la pestaña  **Consola** . El uso de *mensajes de consola* es útil para ver el resultado del código.

* Agregue una llamada a `console.log` después de la instrucción `if`, pero dentro de la escucha de eventos.
  **JavaScript**

  ```
  switcher.addEventListener('click', function() {
      document.body.classList.toggle('light-theme');
      document.body.classList.toggle('dark-theme');

      const className = document.body.className;
      if(className == "light-theme") {
          this.textContent = "Dark";
      } else {
          this.textContent = "Light";
      }

      console.log('current class name: ' + className);
  });
  ```

En  **VS Code** , en un archivo JavaScript, puede usar la función de autocompletar para `console.log` escribiendo `log` y presionando ENTRAR.

Puede definir una *cadena* de texto con comillas simples o dobles alrededor del texto.

### Abrir en el explorador

1. Para obtener una vista previa, seleccione `index.html` y seleccione  **Abrir en el explorador predeterminado** , o bien vuelva a cargar la misma pestaña del explorador presionando F5.
   [![Captura de pantalla del sitio web en la que se muestra el nuevo botón.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/light-theme-with-button.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/light-theme-with-button.png#lightbox)
2. Seleccione el botón **Oscuro** nuevo para cambiar al tema oscuro.
   [![Captura de pantalla del sitio web después de cambiar al tema oscuro.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/dark-theme-with-button.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/dark-theme-with-button.png#lightbox)
3. Asegúrese de que todo parece correcto y se comporta según lo previsto. Si no es así, debe revisar los pasos anteriores para ver si ha pasado algo por alto.

### Comprobación de la página en las herramientas de desarrollo

1. Abra Herramientas de desarrollo.
   * Haga clic con el botón derecho del ratón y seleccione  **Inspeccionar** , o bien use el método abreviado de teclado F12. Como alternativa, use el método abreviado Ctrl+Mayús+I en Windows o Linux y Opción+Comando+I en macOS.
2. Seleccione la pestaña **Elementos** y, dentro de la pestaña  **Elementos** , seleccione la pestaña  **Estilos** .
3. Seleccione el elemento `<body>`. En la pestaña  **Estilos** , revise el tema aplicado. Si el tema actual es oscuro, se aplican los estilos `dark-theme`.
   Asegúrese de que esté seleccionado el tema oscuro.
4. Selecciona la pestaña **Consola** para ver el mensaje `console.log`, `current class name: dark-theme`.

[![Captura de pantalla de la ventana del explorador con el sitio web y la consola de Herramientas de desarrollo abierta, en la que se muestra el mensaje de la consola.](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/console-output.png)](https://learn.microsoft.com/es-es/training/windows/get-started-with-web-development/media/console-output.png#lightbox)

Con la consola, puede obtener información interesante de su código JavaScript. Agregue más mensajes de consola para comprender qué partes del código se están ejecutando y conocer los valores actuales de otras variables.

Para obtener más información sobre la consola, consulte el artículo [Información general sobre la consola](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/console/).

### Resumen

En este módulo, ha configurado un entorno de trabajo para el desarrollo web. También ha creado un sitio web y ha probado que todo funciona en un explorador web. Vamos a mirar todo lo que ha conseguido:

* Ha descargado e instalado las herramientas que necesita para el desarrollo web y ha personalizado el editor con paquetes básicos.
* Ha creado un directorio de proyecto y los archivos para crear un sitio web.
* Ha creado un encabezado y otros elementos de página y después los ha vinculado a archivos externos y ha probado la página en un explorador.
* Ha aplicado estilos a distintos elementos y ha probado el sitio en el explorador, y ha agregado compatibilidad con temas mediante CSS.
* Ha agregado JavaScript para habilitar la interacción personalizada con la página y el cambio entre temas.
* Ha aprendido a crear y usar mensajes de consola para inspeccionar el código.

Está recopilando herramientas y construyendo los cimientos para su labor como desarrollador web. Puede volver a usar el sitio web como una plantilla para proyectos futuros. A medida que aumente sus habilidades y conocimientos, podrá acercarse más a la visión que tiene para su sitio web. También es reconfortante ver cómo una idea cobra vida.

### Más información

### Conceptos de desarrollo web

* [Tolerancia a errores (degradación correcta)](https://wikipedia.org/wiki/Fault_tolerance)
* [Separación de intereses](https://wikipedia.org/wiki/Separation_of_concerns)
* [Mejora progresiva](https://wikipedia.org/wiki/Progressive_enhancement)

### Referencias de desarrollo web

#### HTML5

* [W3C: historia de HTML](https://www.w3.org/TR/html52/introduction.html#introduction-history)
* [Webhint - Use charset &#39;Utf-8&#39;](https://webhint.io/docs/user-guide/hints/hint-meta-charset-utf-8/) (Webhint: Uso de charset "Utf-8")
* [Documentación web de MDN: ¿Qué hay en la cabecera?](https://developer.mozilla.org/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)
* [Documentos web MDN: referencia de elementos HTML](https://developer.mozilla.org/docs/Web/HTML/Element)

#### CSS

* [Documentos web MDN: CSS: Hojas de estilo CSS](https://developer.mozilla.org/docs/Web/CSS)

#### JavaScript

* [Documentación web de MDN: Modo strict](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Strict_mode)
* [Documentos web MDN: referencia de JavaScript](https://developer.mozilla.org/docs/Web/JavaScript/Reference)

### Tecnologías de desarrollo web

#### Documentación de Microsoft Edge

* [Herramientas de desarrollo de Microsoft Edge](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/landing/)
* [Inspección, edición y depuración de HTML y CSS con la herramienta Elementos](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/elements-tool/elements-tool)
* [Información general sobre la consola](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/console/)

#### Azure Static Web Apps

Una manera de implementar el sitio web es usar Azure Static Web Apps.

* [Rutas de aprendizaje de Azure Static Web Apps](https://learn.microsoft.com/es-es/training/paths/azure-static-web-apps/)
* [Documentación de Azure Static Web Apps](https://learn.microsoft.com/es-es/azure/static-web-apps)

#### Documentación de Visual Studio Code

* [Interfaz de usuario](https://code.visualstudio.com/docs/getstarted/userinterface)
* [Emmet en Visual Studio Code](https://code.visualstudio.com/docs/editor/emmet)
*
