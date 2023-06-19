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

### HTML5

* [W3C: historia de HTML](https://www.w3.org/TR/html52/introduction.html#introduction-history)
* [Webhint - Use charset &#39;Utf-8&#39;](https://webhint.io/docs/user-guide/hints/hint-meta-charset-utf-8/) (Webhint: Uso de charset "Utf-8")
* [Documentación web de MDN: ¿Qué hay en la cabecera?](https://developer.mozilla.org/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)
* [Documentos web MDN: referencia de elementos HTML](https://developer.mozilla.org/docs/Web/HTML/Element)

### CSS

* [Documentos web MDN: CSS: Hojas de estilo CSS](https://developer.mozilla.org/docs/Web/CSS)

### JavaScript

* [Documentación web de MDN: Modo strict](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Strict_mode)
* [Documentos web MDN: referencia de JavaScript](https://developer.mozilla.org/docs/Web/JavaScript/Reference)

### Tecnologías de desarrollo web

### Documentación de Microsoft Edge

* [Herramientas de desarrollo de Microsoft Edge](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/landing/)
* [Inspección, edición y depuración de HTML y CSS con la herramienta Elementos](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/elements-tool/elements-tool)
* [Información general sobre la consola](https://learn.microsoft.com/es-es/microsoft-edge/devtools-guide-chromium/console/)

### Azure Static Web Apps

Una manera de implementar el sitio web es usar Azure Static Web Apps.

* [Rutas de aprendizaje de Azure Static Web Apps](https://learn.microsoft.com/es-es/training/paths/azure-static-web-apps/)
* [Documentación de Azure Static Web Apps](https://learn.microsoft.com/es-es/azure/static-web-apps)

### Documentación de Visual Studio Code

* [Interfaz de usuario](https://code.visualstudio.com/docs/getstarted/userinterface)
* [Emmet en Visual Studio Code](https://code.visualstudio.com/docs/editor/emmet)

## Los aspectos básicos de la accesibilidad web

### Objetivos de aprendizaje

En este módulo, aprenderá lo siguiente:

* Herramientas que usan los usuarios para examinar páginas web
* Herramientas que usan los desarrolladores para garantizar la accesibilidad
* Aptitudes para garantizar que las páginas sean accesibles

### Asegurarse de que las páginas web sean accesibles para todos los usuarios

Asegurarse de que la página web sea accesible para todos los usuarios y todos los clientes es algo fundamental. Tal y como afirmó Tim Berners-Lee, creador del World Wide Web: "El poder de la Web está en su universalidad. Que cualquier persona pueda acceder, aunque tenga una discapacidad, es un aspecto esencial".

Como desarrollador web con experiencia, es importante aprender a asegurarse de que las páginas sean accesibles desde el principio. Siempre es más fácil crear una página para que sea accesible que adaptarla más adelante. Si aprende estas aptitudes al principio, se convertirán en algo natural. Después puede crear páginas accesibles y detectar posibles problemas.

### Navegación por la Web con más de un explorador

Probablemente esté muy familiarizado con un explorador para navegar por la Web. Cuando piense en diseñar páginas web, puede imaginarse la experiencia del usuario con este explorador porque tiene experiencia personal con él. Pero no todos los usuarios usan un explorador de la misma manera, o ni siquiera usan un explorador. Para crear experiencias para todos los usuarios, debe conocer las distintas herramientas que los usuarios pueden usar al navegar por la Web.

#### Lectores de pantalla

Una de las herramientas de accesibilidad más conocidas es un [lector de pantalla](https://en.wikipedia.org/wiki/Screen_reader). Los lectores de pantalla son clientes que usan con frecuencia las personas con discapacidades visuales. Además, están integrados en la mayoría de los sistemas operativos. A medida que dedicamos tiempo a garantizar que un explorador transmita correctamente la información que queremos compartir, también debemos asegurarnos de que un lector de pantalla hace lo mismo.

En su nivel más básico, un lector de pantalla lee en voz alta una página de arriba abajo. Si la página es todo texto, el lector transmite la información de forma similar a un explorador. Por supuesto, las páginas web rara vez incluyen simplemente texto, ya que contienen vínculos, gráficos, colores y otros componentes visuales. Hay que tener cuidado para que un lector de pantalla pueda leer correctamente esta información.

Algunos exploradores también tienen herramientas y extensiones integradas que pueden leer texto en voz alta o incluso proporcionar algunas características básicas de navegación, como [estas herramientas de explorador Edge centradas en la accesibilidad](https://support.microsoft.com/help/4000734/microsoft-edge-accessibility-features). Estas herramientas de explorador también son herramientas de accesibilidad importantes, pero funcionan de forma diferente a los lectores de pantalla. No deben confundirse con las herramientas de pruebas de lectores de pantalla.

 Nota:

Pruebe un lector de pantalla y un lector de texto del explorador. En Windows, [Narrador](https://support.microsoft.com/windows/complete-guide-to-narrator-e4397a0d-ef4f-b386-d8ae-c172f109bdb1) se incluye de forma predeterminada. También se pueden instalar [JAWS](https://www.nvaccess.org/about-nvda/) y [NVDA](https://webaim.org/articles/jaws/) en Windows. En macOS e iOS, [VoiceOver](https://support.apple.com/guide/voiceover/welcome/10) está instalada de forma predeterminada.

#### Zoom

Otra herramienta que usan normalmente las personas con discapacidades visuales es el zoom. El tipo más básico de zoom es el zoom estático, que se controla mediante el método abreviado de teclado Ctrl+Signo más (+) o disminuyendo la resolución de la pantalla. Este tipo de zoom cambia el tamaño de toda la página. Es importante usar el [diseño dinámico](https://developer.mozilla.org/docs/Learn/CSS/CSS_layout/Responsive_Design), donde los elementos se mueven en función de la [ventanilla](https://developer.mozilla.org/docs/Web/CSS/Viewport_concepts), para proporcionar una buena experiencia de usuario en niveles de zoom mayores.

Es probable que el sistema operativo tenga funcionalidades de zoom integradas que permitan ampliar partes de la pantalla de forma muy parecida a una lupa real. La herramienta [Lupa](https://support.microsoft.com/windows/use-magnifier-to-make-things-on-the-screen-easier-to-see-414948ba-8b1c-d3bd-8615-0e5e32204198) está integrada en Windows, aunque también se puede usar [ZoomText](https://www.freedomscientific.com/training/zoomtext/getting-started/), un complemento de asociados más completo y popular. Tanto macOS como iOS tienen una herramienta de ampliación integrada denominada [Zoom](https://www.apple.com/accessibility/mac/vision/).

### Garantizar la accesibilidad con herramientas de desarrollo

Probar la página web en varios clientes y vistas es tan importante como probarla en varios exploradores. Es posible que estas pruebas no sean prácticas en todos los escenarios, y se pueden pasar por alto situaciones en las que los usuarios utilizan un explorador pero que podrían tener otra discapacidad. Afortunadamente, hay herramientas que puede usar como desarrollador para medir la accesibilidad de una página.

#### Herramientas de comprobación del contraste

Es posible que una persona daltónica no pueda diferenciar entre colores o que tenga dificultades para trabajar con colores similares entre sí. World Wide Web Consortium (W3C), la organización de estándares para la Web, estableció un [sistema de clasificación para el contraste de colores](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html).

Elegir los colores adecuados para asegurarse de que la página sea accesible para todos puede ser difícil de conseguir manualmente. Por tanto, puede usar las siguientes herramientas para generar los colores adecuados y probar el sitio para garantizar el cumplimiento con W3C:

* Herramientas de generación de paletas:
  * [Adobe Color](https://color.adobe.com/create/color-accessibility): una herramienta interactiva para probar combinaciones de colores
  * [Color Safe](http://colorsafe.co/): una herramienta para generar colores de texto basados en un color de fondo seleccionado
* Herramientas de comprobación del cumplimiento:
  * Extensiones del explorador para probar una página:
    * [Edge: WCAG Color contrast checker](https://microsoftedge.microsoft.com/addons/detail/wcag-color-contrast-check/idahaggnlnekelhgplklhfpchbfdmkjp)
    * [Firefox: WCAG Contrast checker](https://addons.mozilla.org/firefox/addon/wcag-contrast-checker/)
    * [Chrome: Colour Contrast Checker](https://chrome.google.com/webstore/detail/colour-contrast-checker/nmmjeclfkgjdomacpcflgdkgpphpmnfe)
  * Aplicaciones:
    * [Colour Contrast Analyser (CCA)](https://www.tpgi.com/color-contrast-checker/)

#### Lighthouse

Lighthouse es una herramienta creada por Google para analizar sitios web. Se ha vuelto tan popular que viene incluida en las herramientas de desarrollo de muchos exploradores. Lighthouse puede examinar la optimización del motor de búsqueda (SEO) de una página, el rendimiento de la carga y otros procedimientos recomendados. Lighthouse también puede analizar una página y proporcionar una puntuación para su accesibilidad actual.

 Nota

Al igual que con cualquier herramienta automatizada, no puede confiar en la puntuación que Lighthouse proporciona como única indicación de la accesibilidad de una página. Pero proporciona un buen punto de partida para identificar y solucionar problemas.

#### Ejercicio: Generación de la puntuación de accesibilidad de una página con Lighthouse

Pruebe Lighthouse en el explorador. En las capturas de pantalla siguientes se usa [Edge](https://www.microsoft.com/edge), pero puede seguir los mismos pasos en Chrome y muchos otros exploradores.

1. Abra el explorador y vaya a la [página web principal de Microsoft](https://microsoft.com/).
2. Presione la tecla F12 para abrir las herramientas de desarrollo.
3. En la parte superior, seleccione el botón de contenido adicional ( **>>** ) para abrir la lista de pestañas ocultas.
   ![Captura de pantalla de las herramientas de desarrollo con el botón de contenido adicional resaltado.](https://learn.microsoft.com/es-es/training/modules/web-development-101-accessibility/media/choose-tab.png)
4. Seleccione **Lighthouse** en la lista.
5. En **Categories** (Categorías), desactive todos los elementos, excepto **Accessibility** (Accesibilidad).
6. En **Device** (Dispositivo), seleccione **Desktop** (Escritorio).
   ![Captura de pantalla de Lighthouse con solo Accessibility (Accesibilidad) seleccionado en Categories (Categorías), y Desktop (Escritorio) seleccionado en Device (Dispositivo).](https://learn.microsoft.com/es-es/training/modules/web-development-101-accessibility/media/lighthouse-option-selection.png)
7. Seleccione **Generate report** (Generar informe).
8. Observe la puntuación y la información asociada sobre la página.
9. Para probar otras páginas, seleccione **Clear all** (Borrar todo) en Lighthouse, vaya a otra página y, a continuación, seleccione **Generate report** (Generar informe).
   ![Captura de pantalla de la sección de URL de Lighthouse, con el botón para borrar todos los elementos resaltado.](https://learn.microsoft.com/es-es/training/modules/web-development-101-accessibility/media/lighthouse-clear.png)

Ya hemos visto cómo usar Lighthouse, junto con la información de accesibilidad que puede proporcionar la herramienta.

### Asegurarse de que los vínculos e imágenes sean accesibles

Dos de los componentes más comunes de cualquier página web son los vínculos y las imágenes. Estos elementos tienen un fuerte impacto en la accesibilidad. Garantizar un buen texto alternativo y de vínculo es uno de los primeros pasos que puede realizar para mejorar las páginas para todos los usuarios.

#### Texto del vínculo

Los hipervínculos son fundamentales para navegar por la Web. Asegurarse de que un lector de pantalla pueda leer correctamente los vínculos permite a todos los usuarios examinar el sitio.

Observe los dos vínculos del texto de ejemplo siguiente:

* "El pingüino pequeño, a veces conocido como 'pingüino del hada', es el pingüino más pequeño del mundo. [Haga clic aquí](https://en.wikipedia.org/wiki/Little_penguin) para obtener más información".
* "El pingüino pequeño, a veces conocido como 'pingüino del hada', es el pingüino más pequeño del mundo. Visite [https://en.wikipedia.org/wiki/Little_penguin](https://en.wikipedia.org/wiki/Little_penguin) para obtener más información".

 Nota

Los dos ejemplos muestran lo que *no* debe hacer como desarrollador web.

Aunque estos vínculos pueden parecer buenos para alguien sin discapacidad visual, un lector de pantalla no podrá procesarlos correctamente. Recuerde que los lectores de pantalla leen el texto. Si aparece una dirección URL en el texto, el lector de pantalla leerá la dirección URL. En general, la dirección URL no transmite información significativa y puede molestar. Es posible que haya experimentado este problema si el teléfono le ha leído un mensaje de texto con una dirección URL.

Los lectores de pantalla también tienen pueden leer solo los hipervínculos de una página, de la misma manera que una persona sin discapacidad visual examinaría una página en busca de vínculos. Si el texto del vínculo siempre es "haga clic aquí", el usuario escuchará "haga clic aquí, haga clic aquí, haga clic aquí, haga clic aquí, haga clic aquí..." Ahora, todos los vínculos son indistinguibles entre sí, por lo que genera una experiencia frustrante.

La palabra "clic" también es un problema, porque no todos los usuarios harán clic. Los usuarios de teléfono pulsan, los usuarios del teclado pueden presionar la tecla Entrar o la barra espaciadora, y otros clientes usarán otros medios.

Siempre es necesario usar textos de vínculo que sean significativos. Un texto de vínculo bueno describe brevemente lo que hay en el otro lado del vínculo. En el ejemplo anterior sobre pingüinos pequeños, el vínculo redirige a la página de Wikipedia sobre la especie. La frase *pingüinos pequeños* sería un texto de vínculo perfecto porque deja claro lo que alguien aprenderá si selecciona el vínculo:

* "El [pingüino pequeño](https://en.wikipedia.org/wiki/Little_penguin), a veces conocido como 'pingüino del hada', es el pingüino más pequeño del mundo".

 Nota

Y como ventaja para garantizar que el sitio sea accesible para todos los usuarios, también ayudará a los motores de búsqueda a examinar el sitio. Los motores de búsqueda usan texto de vínculo para aprender los temas de las páginas. Por lo tanto, usar un buen texto de vínculo ayuda a todos los usuarios.

#### Atributos ARIA

Imagínese la siguiente página de un producto:

| Producto    | Descripción           | Ordenar          |
| ----------- | ---------------------- | ---------------- |
| Widget      | `[Description]('#')` | `[Order]('#')` |
| Superwidget | `[Description]('#')` | `[Order]('#')` |

Se trata de un diseño común para una página que muestra información sobre varios elementos de una tabla, con vínculos a la descripción y el pedido. Duplicar el texto de la descripción y el pedido tiene sentido para alguien que usa un explorador. Sin embargo, una persona que usa un lector de pantalla solo escucharía las palabras *descripción* y *pedido* repetidos sin contexto.

Para admitir estos tipos de escenarios, HTML admite un conjunto de atributos conocidos como [aplicaciones de Internet enriquecidas y accesibles (ARIA)](https://developer.mozilla.org/docs/Web/Accessibility/ARIA). Puede usar estos atributos para proporcionar más información a los lectores de pantalla.

Por ejemplo, puede usar `aria-label` para describir un vínculo cuando el formato de la página no se lo permite. La descripción del *widget* podría establecerse de esta forma:

**HTML**

```
<a href="#" aria-label="Widget description">description</a>
```

ARIA puede usarse para muchas más cosas que agregar texto para que los lectores de pantalla lean los vínculos. Puede usarse para describir los roles que determinados elementos desempeñan cuando el código HTML semántico no está disponible. Al crear un árbol, por ejemplo, puede usar roles de ARIA para describir la interfaz a un lector de pantalla:

**HTML**

```
<h2 id="tree-label">File Viewer</h2>
<div role="tree" aria-labelledby="tree-label">
  <div role="treeitem" aria-expanded="false" tabindex="0">Uploads</div>
</div>
```

 Importante

El uso de marcado semántico y texto de vínculo bueno como se describió anteriormente suele sustituir el uso de ARIA. Los exploradores y los lectores de pantalla no son los únicos clientes que un usuario podría usar, y diseñar la página para que funcione bien para todos los clientes y usuarios debe ser el objetivo principal.

#### Texto alternativo para imágenes

Como regla general, los lectores de pantalla no pueden leer el contenido de una imagen. Aunque algunos podrían usar inteligencia artificial, es posible que los resultados generados no sean precisos contextualmente. Afortunadamente, asegurarse de que las imágenes son accesibles no lleva mucho trabajo; de eso trata el atributo `alt`. Todas las imágenes significativas deben tener un atributo `alt` (conocido ocasionalmente como  *texto alternativo* ) para describir lo que son o la información que intentan transmitir.

Las imágenes que son puramente decorativas deben tener su atributo `alt` establecido en una cadena vacía: `alt=""`. Esta configuración evita que los lectores de pantalla anuncien innecesariamente la imagen interior.

 Nota

Como es de esperar, los motores de búsqueda no pueden entender lo que hay en una imagen, ya que se basan en texto alternativo. Por lo tanto, una vez más, asegurarse de que la página es accesible proporciona ventajas.

### Accesibilidad del diseño

La accesibilidad es un tema relativamente largo. No puede abarcarse por completo en un solo módulo de Learn. Sin embargo, hay algunos principios básicos que recomendamos implementar en cada página que cree. Diseñar una página accesible desde el principio siempre es más fácil que hacer que una página que ya exista sea accesible.

#### Uso del código HTML de la forma en que se diseñó

HTML proporciona muchos elementos que puede usar para crear una página, incluidos botones, vínculos y controles de formulario. Cada uno de esos elementos tiene un conjunto de funcionalidades integradas para, por ejemplo, que se puede hacer clic en ellos, que tengan un vínculo o que acepten el foco.

 Nota

*Foco* es un término de desarrollo web que significa que un control puede aceptar entradas de un teclado. Un botón puede aceptar el foco, lo que permite a alguien activarlo o "hacer clic" en él seleccionando la barra espaciadora.

Con CSS y JavaScript, es posible que cualquier elemento se parezca a cualquier tipo de control. Por ejemplo, puede usar `<span>` para crear un elemento `<button>`, y `<b>` puede convertirse en `<a>`. Aunque esta funcionalidad proporciona algunos accesos directos para aplicar estilos o diseñar la página, se quita la funcionalidad integrada. Herramientas como los lectores de pantalla no podrán entender que `<span>` se usa como `<a>`. Alguien que navega con un teclado no podrá establecer el foco en un elemento `<div>` que se haya programado para simular un elemento `<button>`.

Otro elemento HTML que a menudo se omite son los encabezados (de `<h1>` a `<h6>`). Desde un punto de vista visual, las etiquetas de encabezado van de mayor a menor tamaño de texto. Esta convención lleva a muchos desarrolladores a renunciar a los elementos de encabezado y, en su lugar, a aplicar estilo en `<div>` o en otros elementos genéricos.

Desafortunadamente, los elementos genéricos con estilos solo transmiten información visual en lugar de estructural. Los usuarios de lectores de pantalla [dependen en gran medida de los encabezados](https://webaim.org/projects/screenreadersurvey8/#finding) para buscar información y navegar por una página. La creación de un contenido de encabezado descriptivo y el uso de etiquetas de encabezado semánticas son importantes para crear un sitio fácilmente navegable para los usuarios de lectores de pantalla.

Como procedimiento recomendado, siempre debe usar el código HTML adecuado al crear controles en una página. Si desea un hipervínculo, use `<a>` o `<button>` para un botón.

#### Uso de buenas indicaciones visuales

Los desarrolladores suelen pensar que los lectores de pantalla son la única herramienta de accesibilidad. Sin embargo, es posible que los usuarios usen muchas otras herramientas, o que no usen ninguna. Los usuarios que usan el explorador dependerán de determinadas indicaciones visuales para comprender cómo interactuar con la página.

Una de las características excelentes de CSS es que proporciona un control completo sobre cómo mostrar una página, incluida la eliminación de determinados elementos para mostrar. Por ejemplo, puede quitar el contorno de un cuadro de texto o quitar el subrayado de un hipervínculo. Desafortunadamente, quitar esos tipos de indicaciones puede hacer más difícil que alguien que depende de ellas reconozca el tipo de control.

#### Tenga en cuenta el teclado

Algunos usuarios no pueden usar un mouse o panel táctil. En su lugar, estos usuarios dependen de las interacciones del teclado para desplazarse con la tecla de tabulación de un elemento al siguiente. Es importante que las páginas presenten el contenido en un orden lógico para que un usuario de teclado pueda acceder a cada elemento interactivo a medida que se desplaza hacia abajo.

Cuando un usuario se desplaza por una página mediante tabulación, el foco se mueve de un control al siguiente en función del orden en el que se enumeran los controles en el origen HTML. Los controles de la página deberían aparecer enumerados en el origen HTML en el orden en el que espera que se navegue por la página, y a la vez usar CSS para mostrar la página visualmente a los usuarios.

Por ejemplo, imagínese que crea un formulario con dos columnas. Recomendamos tener en cuenta cuál es el flujo natural para alguien que rellena el formulario y, a continuación, enumerar los controles en ese orden. A continuación, puede usar CSS para crear las columnas y mostrar los controles en sus ubicaciones adecuadas.

La navegación mediante teclado se basa en gran medida en HTML semántico. Ciertos controles (como botones) aceptan el foco, al contrario que los elementos `div`. Si va a volver a crear controles que ya existen en HTML, está dificultando que alguien use la página con un teclado.

 Importante

La navegación con el teclado debe probarse manualmente, y debe hacerlo en todas las páginas que cree. [WebAIM](https://webaim.org/techniques/keyboard/) tiene más información sobre las estrategias de navegación con el teclado.

### Prueba de conocimientos

Elija la respuesta más adecuada para cada pregunta. Después, seleccione  **Comprobar las respuestas** .

**1.** ¿Cuál de los siguientes elementos es un vínculo accesible?

* [ ] `<a href="https://www.microsoft.com">https://www.microsoft.com</a>`
* [ ] `<a href="https://www.microsoft.com">Microsoft</a>`
* [ ] `<a href="https://www.microsoft.com/>Click here</a>`

**2.** ¿Cuál de las siguientes afirmaciones es un uso adecuado de los atributos ARIA (aplicaciones de Internet enriquecidas y accesibles)?

* [ ] Indicar a un lector de pantalla que un elemento `div` es realmente un elemento `button`.
* [ ] Proporcionar texto diferente para que un lector de pantalla lo lea en voz alta cuando el texto del vínculo diga "haga clic aquí".
* [ ] Dar contexto a un lector de pantalla cuando un control no existe en HTML semántico, como un árbol.

**3.** Para agregar un control que el usuario selecciona para realizar una acción, ¿qué elemento HTML se debe usar?

* [ ] `div`
* [ ] `span`
* [ ] `p`
* [ ] `button`

### Resumen

En este módulo, hemos analizado los conceptos de accesibilidad web. Ha obtenido información sobre lo siguiente:

* Herramientas que usan los usuarios para examinar páginas web
* Herramientas que usan los desarrolladores para garantizar la accesibilidad
* Aptitudes para garantizar que las páginas sean accesibles

### Desafío

La mejor manera de entender cómo hacer que las páginas sean accesibles y el impacto de las decisiones que se toman al crear HTML es usar algunas de las herramientas que emplean los usuarios para navegar por la Web.

Desplácese por un par de páginas mediante un lector de pantalla. Abra un sitio web que tenga un formulario y use solo el teclado para completarlo. Esta actividad le dará una idea de lo que algunos usuarios experimentan a diario al usar la Web y la importancia de garantizar que las páginas sean accesibles.

### Créditos

Este módulo se publicó por primera vez como una lección del plan de estudios [Desarrollo web para principiantes](https://github.com/microsoft/Web-Dev-For-Beginners) por parte de promotores de Azure. El autor de la lección original es Christopher Harrison.

## Creación de una interfaz de usuario web con ASP.NET Core

Aprenda a crear páginas web mediante Razor con ASP.NET Core.

### Objetivos de aprendizaje

En este módulo, aprenderá a:

* Entender cuándo y por qué usar Razor Pages para la aplicación ASP.NET Core.
* Revisar una aplicación de ASP.NET Core que usa Razor Pages
* Crear una página de Razor que admita los requisitos de administración de datos de productos de la aplicación
* Usar asistentes de etiquetas para reducir el cambio de contexto entre HTML y C#
* Usar controladores de página de Razor para controlar las solicitudes HTTP

### Introducción

En este módulo, creará una aplicación web Razor Pages de ASP.NET Core multiplataforma con .NET y C#.

#### Escenario de ejemplo

Imagine que es empleado de una empresa de pizzas llamada Contoso Pizza. El administrador le ha pedido que desarrolle un servicio de administración del inventario de pizzas como requisito previo para el sitio web de administración interna de la empresa. La aplicación debe compilarse de tal forma que los intereses del modelo de datos y la vista estén separados.

#### ¿Qué va a hacer?

En este módulo, aprenderá a:

* Entender cuándo y por qué usar Razor Pages para la aplicación ASP.NET Core.
* Revisar una aplicación de ASP.NET Core que usa Razor Pages
* Crear una página de Razor que admita los requisitos de administración de datos de productos de la aplicación
* Usar aplicaciones auxiliares de etiquetas para reducir el cambio de contexto entre HTML y C#
* Usar controladores de página de Razor para controlar las solicitudes HTTP

Al final de este módulo, hay vínculos a contenido que proporcionan análisis más profundos de cada área de características presentada.

#### Herramientas necesarias

En este módulo se usa la [CLI de .NET](https://learn.microsoft.com/es-es/dotnet/core/tools/) y [Visual Studio Code](https://code.visualstudio.com/) (Windows, Linux y macOS) para demostrar el desarrollo de Razor Pages con ASP.NET Core. Cuando complete este módulo, podrá aplicar sus conceptos mediante un entorno de desarrollo como Visual Studio (Windows), Visual Studio para Mac (macOS) o Visual Studio Code.

 Sugerencia

Puede omitir la instalación de las herramientas siguientes mediante GitHub Codespaces como su IDE. En otra pestaña del explorador, vaya al [repositorio de GitHub que contiene la aplicación de inicio de este módulo](https://github.com/MicrosoftDocs/mslearn-create-razor-pages-aspnet-core), seleccione el botón **Código** y cree un nuevo codespace en la rama `main`. Para obtener más información, consulte [Crear un codespace](https://docs.github.com/github/developing-online-with-codespaces/creating-a-codespace).

Como alternativa, puede usar la extensión [Contenedores de desarrollo](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) para Visual Studio Code. Con la extensión instalada, presione **F1** para abrir la paleta de comandos y, a continuación, busque y seleccione **Contenedores de desarrollo: Clonar repositorio en volumen de contenedor** y proporcione la dirección URL `https://github.com/MicrosoftDocs/mslearn-create-razor-pages-aspnet-core`. Esto clonará el repositorio y lo abrirá en un contenedor con todas las herramientas necesarias instaladas.

Se requieren las herramientas siguientes:

#### .NET SDK

En este módulo se usa el SDK de .NET 7.0. Asegúrese de que tiene instalado .NET 7.0 mediante la ejecución del siguiente comando en el terminal que prefiera:

**CLI de .NET**

```
dotnet --list-sdks
```

Verá un resultado similar al siguiente:

**Consola**

```
6.0.308 [C:\Program Files\dotnet\sdk]
7.0.100 [C:\Program Files\dotnet\sdk]
7.0.102 [C:\Program Files\dotnet\sdk]
```

Asegúrese de que aparece una versión que comienza por `7`. Si no aparece ninguna o no se encuentra el comando, [instale el SDK más reciente de .NET 7.0](https://dotnet.microsoft.com/download).

#### CLI de GitHub

Para clonar la aplicación de ejemplo desde GitHub, necesitará la [CLI de GitHub](https://cli.github.com/).

#### Visual Studio Code

Asegúrese de que tiene las versiones más recientes de [Visual Studio Code](https://code.visualstudio.com/) y la [extensión de C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp).

### Entender cuándo y por qué usar Razor Pages

En esta unidad, aprenderá cuándo y por qué usar Razor Pages para la aplicación ASP.NET Core.

#### Ventajas de Razor Pages

Razor Pages es un modelo de programación centrado en páginas en el lado servidor para crear interfaces de usuario web con ASP.NET Core. Dicha integración aporta las siguientes ventajas:

* Instalación fácil para aplicaciones web dinámicas con HTML, CSS y C#.
* Archivos organizados por característica para facilitar el mantenimiento.
* Combina el marcado con código de C# del lado servidor mediante la sintaxis Razor.

En Razor Pages se usa *[Razor](https://learn.microsoft.com/es-es/aspnet/core/mvc/views/razor)* para insertar código basado en servidor en las páginas web. La sintaxis de Razor combina HTML y [C#](https://dotnet.microsoft.com/languages/csharp) para definir la lógica de representación dinámica. Esto significa que puede usar variables y métodos de C# en el marcado HTML para generar contenido web dinámico en el servidor en tiempo de ejecución. Resulta importante saber que Razor Pages no sustituye a HTML, CSS o JavaScript. Es una forma de combinar estas tecnologías para crear contenido web dinámico.

#### Separación de intereses

Razor Pages aplica la separación de intereses con una clase `PageModel` de C#, encapsulando propiedades de datos y operaciones lógicas con ámbito en su página de Razor, y definiendo controladores de página para las solicitudes HTTP. La clase `PageModel` es una [clase parcial](https://learn.microsoft.com/es-es/dotnet/csharp/programming-guide/classes-and-structs/partial-classes-and-methods) generada automáticamente por la plantilla de proyecto de ASP.NET Core. La clase `PageModel` se encuentra en la carpeta `Pages` y tiene el nombre de la página de Razor. Por ejemplo, la clase `PageModel` de la página de Razor `Index.cshtml` se llama `IndexModel.cs`.

#### Cuándo usar Razor Pages

Use Razor Pages en la aplicación ASP.NET Core cuando:

* Quiera generar una interfaz de usuario web dinámica.
* Prefiera un enfoque centrado en páginas.
* Quiera reducir la duplicación con vistas parciales.

Razor Pages simplifica la organización de páginas de ASP.NET Core. Para ello, mantiene juntas las páginas relacionadas y su lógica en su propio espacio de nombres y directorio.

 Nota

ASP.NET Core también admite el [patrón de Controlador de vista de modelo (MVC)](https://learn.microsoft.com/es-es/aspnet/core/mvc/overview) para compilar aplicaciones web. Use MVC cuando prefiera una separación clara entre el modelo, la vista y el controlador. Tanto Razor Pages como MVC pueden coexistir dentro de la misma aplicación. MVC está fuera del ámbito de este módulo.

En la unidad siguiente, realizará un recorrido por una aplicación de Razor Pages.

#### Comprobación de conocimientos

**1.** ¿Cuál de las siguientes afirmaciones es verdadera para Razor Pages?

* [ ] Use Razor Pages para una aplicación ASP.NET Core que no se centre en la generación de HTML, como una API web.
* [ ] Razor Pages no puede coexistir en una aplicación ASP.NET°Core MVC.
* [ ] Una ventaja de productividad de Razor Pages es que mantiene juntos los elementos que suelen cambiar para las vistas de la aplicación.

### Ejercicio: Personalización del proyecto

El equipo ha dividido el trabajo de la aplicación de administración del inventario de pizzas. Sus compañeros de equipo han creado la aplicación web ASP.NET Core para usted y ya han creado un servicio para leer y escribir pizzas en una base de datos. Se le ha asignado para trabajar en la página Lista de pizzas, que mostrará una lista de pizzas y le permitirá agregar nuevas pizzas a la base de datos. Empezará explorando el proyecto para comprender cómo se organiza.

#### Obtención de los archivos de proyecto

Si usa GitHub Codespaces, solo tiene que [abrir el repositorio en el explorador](https://github.com/MicrosoftDocs/mslearn-create-razor-pages-aspnet-core), seleccionar **Código** y, después, crear un codespace en la rama `main`.

Si no usa GitHub Codespaces, obtenga los archivos del proyecto y ábralos en Visual Studio Code con los pasos siguientes:

1. Abra un shell de comandos y clone el proyecto desde GitHub mediante la línea de comandos:
   **Bash**

   ```
   git clone https://github.com/MicrosoftDocs/mslearn-create-razor-pages-aspnet-core
   ```
2. Vaya al directorio `mslearn-create-razor-pages-aspnet-core` y abra el proyecto en Visual Studio Code:
   **Bash**

   ```
   cd mslearn-create-razor-pages-aspnet-core
   code .
   ```

 Sugerencia

Si tiene instalado un entorno de ejecución de contenedor compatible, puede usar la extensión [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) para abrir el repositorio en un contenedor con las herramientas preinstaladas.

#### Revisión del trabajo de sus compañeros de equipo

Dediquemos un momento a familiarizarnos con el código de la carpeta ContosoPizza. El proyecto es una aplicación web ASP.NET Core creada con el comando `dotnet new webapp`. Los cambios realizados por los compañeros de equipo se describen a continuación.

 Sugerencia

No dedique demasiado tiempo a revisar estos cambios. Sus compañeros de equipo ya han realizado el trabajo para crear la base de datos y el servicio para leer y escribir pizzas en la base de datos, pero no realizaron ningún cambio en la interfaz de usuario. Va a crear una interfaz de usuario que consuma su servicio en la unidad siguiente.

* Se agregó una carpeta *Models* al proyecto.
  * La carpeta model contiene una clase `Pizza` que representa una pizza.
* Se agregó una carpeta *Data* al proyecto.
  * La carpeta Data contiene una clase `PizzaContext` que representa el contexto de la base de datos. Hereda de la clase `DbContext` de Entity Framework Core. Entity Framework Core es un asignador relacional de objetos (ORM) que facilita el trabajo con bases de datos.
* Se agregó una carpeta *Services* al proyecto.
  * La carpeta Services contiene una clase `PizzaService` que expone métodos para enumerar y agregar pizzas.
  * La clase `PizzaService` usa la clase `PizzaContext` para leer y escribir pizzas en la base de datos.
  * La clase se registra para la inserción de dependencias en *Program.cs* (línea 10).

Entity Framework Core también generó algunas cosas:

* Se generó una carpeta  *Migrations* .
  * La carpeta Migrations contiene código para crear el esquema de la base de datos.
* Se generó el archivo de base de datos SQLite  *ContosoPizza.db* .
  * Si tiene instalada la [extensión SQLite](https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite) (o usa GitHub Codespaces), puede ver la base de datos haciendo clic con el botón derecho en el archivo y seleccionando  **Abrir base de datos** . El esquema de la base de datos se muestra en la pestaña **SQLite Explorer** del panel Explorador.

#### Revisión de la estructura del proyecto de Razor Pages

Todo lo demás del proyecto no cambia desde el momento en que se creó el proyecto. En la tabla siguiente se describe la estructura del proyecto generada por el comando `dotnet new webapp`.

| Nombre                  | Descripción                                                                                                                                |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| *Pages/*              | Contiene Razor Pages y archivos auxiliares. Cada página de Razor tiene un archivo*.cshtml* y un archivo de clase*.cshtml.cs*`PageModel`. |
| *wwwroot/*            | Contiene archivos de recursos estáticos, como HTML, JavaScript y CSS.                                                                      |
| *ContosoPizza.csproj* | Contiene los metadatos de configuración del proyecto, como las dependencias.                                                               |
| *Program.cs*          | Actúa como punto de entrada de la aplicación y configura el comportamiento de la aplicación, como el enrutamiento.                       |

Otras observaciones destacadas:

* **Archivos de página de Razor y su archivo de clase `PageModel` emparejado**
  Las páginas de Razor se almacenan en el directorio  *Pages* . Como se indicó anteriormente, cada página de Razor tiene un archivo *.cshtml* y un archivo de clase *.cshtml.cs* `PageModel`. La clase `PageModel` permite la separación de la lógica y la presentación de una página de Razor, define los controladores de página para las solicitudes y encapsula las propiedades de datos y la lógica con ámbito en su página de Razor.
* **La estructura de directorios *Pages *y las solicitudes de enrutamiento de páginas**
  Razor Pages usa la estructura del directorio *Pages* como convención para el enrutamiento de las solicitudes. En la tabla siguiente se muestra cómo se asignan las direcciones URL a los nombres de archivo:

  | Resolución                | Asignaciones a la página de Razor |
  | -------------------------- | ---------------------------------- |
  | `www.domain.com`         | */Pages/Index.cshtml*            |
  | `www.domain.com/Index`   | */Pages/Index.cshtml*            |
  | `www.domain.com/Privacy` | *Pages/Privacy.cshtml*           |
  | `www.domain.com/Error`   | *Pages/Error.cshtml*             |

  Las subcarpetas del directorio *Pages* se usan para organizar las páginas de Razor. Por ejemplo, si hubiera un directorio  *Pages/Products* , las direcciones URL reflejarían esa estructura:

  | Resolución                        | Asignaciones a la página de Razor |
  | ---------------------------------- | ---------------------------------- |
  | `www.domain.com/Products`        | *Pages/Products/Index.cshtml*    |
  | `www.domain.com/Products/Index`  | *Pages/Products/Index.cshtml*    |
  | `www.domain.com/Products/Create` | *Pages/Products/Create.cshtml*   |
* **Diseño y otros archivos compartidos**
  Hay varios archivos que se comparten entre varias páginas. Estos archivos determinan las importaciones de páginas y elementos de diseño comunes. En la siguiente tabla se describe la finalidad de cada campo.

  | Archivo                                           | Descripción                                                                                                                      |
  | ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
  | _ViewImports.cshtml                               | Importa espacios de nombres y clases que se usan en varias páginas.                                                              |
  | _ViewStart.cshtml                                 | Especifica el diseño predeterminado para todas las páginas de Razor.                                                            |
  | *Pages/Shared/_Layout.cshtml*                   | Este es el diseño especificado por el archivo `_ViewStart.cshtml`. Implementa elementos de diseño comunes en varias páginas. |
  | *Pages/Shared/_ValidationScriptsPartial.cshtml* | Proporciona funcionalidad de validación a todas las páginas.                                                                    |

#### Ejecución del proyecto por primera vez

Vamos a ejecutar el proyecto para que podamos verlo en acción.

1. Haga clic con el botón derecho en la carpeta *ContosoPizza* en el **Explorador** y seleccione  **Abrir en terminal integrado** . Se abre una ventana de terminal en el contexto de la carpeta del proyecto.
2. Escriba el siguiente comando en el terminal:
   **CLI de .NET**

   ```
   dotnet watch
   ```

   Este comando:

   * Compila el proyecto.
   * Inicia la aplicación.
   * Busca cambios en los archivos y reinicia la aplicación cuando detecta un cambio.
3. El IDE le pide que abra la aplicación en un explorador. Seleccione  **Abrir en el explorador** .
   Sugerencia

   También puede abrir la aplicación buscando la dirección URL en la ventana del terminal. Mantenga presionada la tecla **Ctrl** y haga clic en la dirección URL para abrirla en un explorador.
4. Compare la página principal representada con *Pages/Index.cshtml* en el IDE:

   * Observe la combinación de código HTML, sintaxis de Razor y C# en el archivo.
     * La sintaxis de Razor se indica mediante caracteres `@`.
     * El código de C# se incluye en bloques `@{ }`. Tome nota de las directivas en la parte superior del archivo:
     * La directiva `@page` especifica que este archivo es una página de Razor.
     * La directiva `@model` especifica el tipo de modelo de la página (en este caso, `IndexModel`, que se define en  *Pages/Index.cshtml.cs* ).
   * Revise el bloque de código de C#.
     * El código establece el valor del elemento `Title` dentro del diccionario `ViewData` en "Página principal".
     * El diccionario `ViewData` se usa para pasar datos entre la página de Razor y la clase `IndexModel`.
     * En tiempo de ejecución, el valor `Title` se usa para establecer el elemento `<title>` de la página.

Deje la aplicación en ejecución en la ventana del terminal. Lo usaremos en las próximas unidades. Deje también la pestaña del explorador con la aplicación Contoso Pizza en ejecución. Realizará cambios en la aplicación y el explorador se actualizará automáticamente para mostrar los cambios.

#### Personalización de la página de aterrizaje

Vamos a realizar algunos cambios en la página de aterrizaje para que sea más relevante para la aplicación de pizza.

1. En  *Pages/Index.cshtml* , reemplace el código del bloque de código de C# por el código siguiente:
   **C#**

   ```
   ViewData["Title"] = "The Home for Pizza Lovers";
   TimeSpan timeInBusiness = DateTime.Now - new DateTime(2018, 8, 14);
   ```

   El código anterior:

   * Establece el valor del elemento `Title` dentro del diccionario `ViewData` en "The Home for Pizza Lovers".
   * Calcula la cantidad de tiempo transcurrido desde que se abrió la empresa.
2. Modifique el código HTML de la siguiente manera:

   * Reemplace el elemento `<h1>` por el código siguiente:
     **CSHTML**

     ```
     <h1 class="display-4">Welcome to Contoso Pizza</h1>
     ```
   * Reemplace el elemento `<p>` por el código siguiente:
     **CSHTML**

     ```
     <p class="lead">The best pizza in town for @Convert.ToInt32(timeInBusiness.TotalDays) days!</p>
     ```

   El código anterior:

   * Cambia el encabezado a "Le damos la bienvenida a Contoso Pizza".
   * Muestra el número de días transcurridos desde que se abrió la empresa.
     * El carácter `@` se usa para cambiar de HTML a sintaxis de Razor.
     * El método `Convert.ToInt32` se usa para convertir la propiedad `TotalDays` de la variable `timeInBusiness` en un entero.
     * La clase `Convert` forma parte del espacio de nombres `System`, que el elemento importa automáticamente `<ImplicitUsings>` en el archivo  *ContosoPizza.csproj* .
3. Guarde el archivo. La pestaña del explorador con la aplicación se actualiza automáticamente para mostrar los cambios. Si usa GitHub Codespaces, el archivo se guarda automáticamente, pero tendrá que actualizar manualmente la pestaña del explorador.

 Importante

Vigile la ventana del terminal con `dotnet watch` cada vez que guarde el archivo. A veces, el código puede contener lo que llama a una  *edición superficial* . Esto significa que el código que ha cambiado no se puede volver a compilar sin reiniciar la aplicación. Si se le pide que reinicie la aplicación, presione `y` (sí) o `a` (siempre). Si se produce un error en todo lo demás, detenga la aplicación presionando **Ctrl+C** en la ventana del terminal y, a continuación, reiníciela ejecutando `dotnet watch` de nuevo.

Ha realizado sus primeros cambios en una página de Razor. En la unidad siguiente, agregará una nueva página a la aplicación para mostrar una lista de pizzas.

### Ejercicio: Adición de una nueva página de Razor

En la unidad anterior, obtuvo el código fuente del proyecto Contoso Pizza y, a continuación, realizó algunos cambios sencillos en la página principal. En esta unidad, agregará una nueva página de Razor al proyecto.

#### Creación de la página Lista de pizzas

Para crear una nueva página de Razor, usará la CLI de .NET.

1. Como el comando bloquea el comando `dotnet watch`, abra otro comando haciendo clic con el botón derecho en la carpeta *ContosoPizza* en el **Explorador** y seleccione  **Abrir en terminal integrado** .
2. Escriba el siguiente comando en la ventana del terminal:
   **CLI de .NET**

   ```
   dotnet new page --name PizzaList --namespace ContosoPizza.Pages --output Pages
   ```

   El comando anterior:

   * Crea los archivos siguientes en el espacio de nombres `ContosoPizza.Pages`:
     * *PizzaList.cshtml* : la página de Razor
     * *PizzaList.cshtml.cs* : la clase `PageModel` que la acompaña
   * Almacena ambos archivos en el directorio *Pages* del proyecto.
3. En  *Pages/PizzaList.cshtml* , agregue el código siguiente dentro del bloque de código `@{ }`:
   **razor**

   ```
   ViewData["Title"] = "Pizza List 🍕";
   ```

   Esto establece el elemento `<title>` de la página.
4. Agregue el siguiente código al final del archivo :
   **razor**

   ```
   <h1>Pizza List 🍕</h1>

   <!-- New Pizza form will go here -->

   <!-- List of pizzas will go here -->
   ```

   Esto agrega un encabezado a la página, así como dos marcadores de posición de comentario HTML para la funcionalidad que agregará más adelante.
5. Guarde el archivo. Si usa GitHub Codespaces, el archivo se guarda automáticamente.
6. Vuelva al terminal en ejecución `dotnet watch` y presione **Ctrl+R** para volver a cargar la aplicación y detectar los nuevos archivos.

#### Adición de la página Lista de pizzas al menú de navegación

Este sería un buen momento para probar la página, pero aún no puede hacerlo porque la página no está vinculada al menú de navegación. Lo haremos ahora después.

1. Abra  *Pages/Shared/_Layout.cshtml* .
2. En el elemento `<ul>` con la clase `navbar-nav` (comienza en la línea 21), observe los elementos `<li>` que contienen los vínculos a las páginas *Inicio* y  *Privacidad* . Agregue el código siguiente al final de la lista, después del elemento `<li>` que contiene el vínculo  *Privacidad* :
   **razor**

   ```
   <li class="nav-item">
       <a class="nav-link text-dark" asp-area="" asp-page="/PizzaList">Pizza List 🍕</a>
   </li>
   ```

   Esto agrega un vínculo a la página *Lista de pizzas* al menú de navegación.
3. Guarde el archivo. La pestaña del explorador con la aplicación se actualiza automáticamente para mostrar los cambios. Si usa GitHub Codespaces, el archivo se guarda automáticamente, pero tendrá que actualizar manualmente la pestaña del explorador.
4. Seleccione el vínculo *Lista de pizzas 🍕* en el menú de navegación. Aparece la página Lista de pizzas.

#### Registro de la clase PizzaService con el contenedor de inserción de dependencias

La página Lista de pizzas depende del objeto `PizzaService` para recuperar la lista de pizzas. Usará la inserción de dependencias para proporcionar el objeto `PizzaService` a la página. Para que esto suceda, debe registrar la clase `PizzaService` con el contenedor.

1. Abra  *Program.cs* .
2. En la sección que agrega servicios al contenedor, agregue el código siguiente:
   **C#**

   ```
   builder.Services.AddScoped<PizzaService>();
   ```

   Este código registra la clase `PizzaService` con el contenedor de inserción de dependencias. El método `AddScoped` indica que se debe crear un nuevo objeto `PizzaService` para cada solicitud HTTP. Ahora `PizzaService` se puede insertar en cualquier página de Razor.
3. Guarde el archivo. Si usa GitHub Codespaces, el archivo se guarda automáticamente.

#### Presentación de una lista de pizzas

Vamos a modificar la clase d `PageModel` e la página Lista de pizzas para recuperar la lista de pizzas del objeto `PizzaService` y almacenarla en una propiedad .

1. Abra  *Pages/PizzaList.cshtml.cs* .
2. Agregue las siguientes instrucciones `using` al principio del archivo:
   **C#**

   ```
   using ContosoPizza.Models;
   using ContosoPizza.Services;
   ```

   Estas instrucciones importan los tipos `Pizza` y `PizzaService` que usará en la página.
3. Dentro del bloque de espacio de nombres `ContosoPizza.Pages`, reemplace toda la clase `PizzaListModel` por el código siguiente:
   **C#**

   ```
   public class PizzaListModel : PageModel
   {
       private readonly PizzaService _service;
       public IList<Pizza> PizzaList { get;set; } = default!;

       public PizzaListModel(PizzaService service)
       {
           _service = service;
       }

       public void OnGet()
       {
           PizzaList = _service.GetPizzas();
       }
   }
   ```

   En el código anterior:

   * Se crea un objeto `PizzaService` privado de solo lectura llamado `_service`. Esta variable contendrá una referencia a un objeto `PizzaService`.
     * La palabra clave `readonly` indica que el valor de la variable `_service` no se puede cambiar después de establecerlo en el constructor.
   * Se define una propiedad `PizzaList` para contener la lista de pizzas.
     * El tipo `IList<Pizza>` indica que la propiedad `PizzaList` contendrá una lista de objetos `Pizza`.
     * `PizzaList` se inicializa en `default!` para indicar al compilador que se inicializará más adelante, por lo que no se requieren comprobaciones de seguridad nulas.
   * El constructor acepta un objeto `PizzaService`.
     * La inserción de dependencias proporciona el objeto `PizzaService`.
   * Se define un método `OnGet` para recuperar la lista de pizzas del objeto `PizzaService` y almacenarla en la propiedad `PizzaList`.

   Sugerencia

   Si necesita ayuda para comprender la seguridad de NULL, consulte [Seguridad de NULL en C#](https://learn.microsoft.com/es-es/training/modules/csharp-null-safety/).
4. Guarde el archivo. Si usa GitHub Codespaces, el archivo se guarda automáticamente.
5. Vuelva al terminal en ejecución `dotnet watch` y presione **Ctrl+R** para volver a cargar la aplicación con el servicio registrado y el nuevo constructor para `PizzaListModel`.

#### Presentación de la lista de pizzas

Ahora que la página tiene acceso a la lista de pizzas, usará esa lista para mostrar las pizzas en la página.

1. Abra  *Pages/PizzaList.cshtml* .
2. Reemplace el comentario `<!-- List of pizzas will go here -->` por el código siguiente:
   **razor**

   ```
   <table class="table mt-5">
       <thead>
           <tr>
               <th scope="col">Name</th>
               <th scope="col">Price</th>
               <th scope="col">Size</th>
               <th scope="col">Gluten Free</th>
               <th scope="col">Delete</th>
           </tr>
       </thead>
       <tbody>
       @foreach (var pizza in Model.PizzaList)
       {
           <tr>
               <td>@pizza.Name</td>
               <td>@($"{pizza.Price:C}")</td>
               <td>@pizza.Size</td>
               <td>@(pizza.IsGlutenFree ? "✔️" : string.Empty)</td>
               <td>
                   <form method="post" asp-page-handler="Delete" asp-route-id="@pizza.Id">
                       <button class="btn btn-danger">Delete</button>
                   </form>
               </td>
           </tr>
       }
       </tbody>
   </table>
   ```

   En el código anterior:

   * Se crea un elemento `<table>` para mostrar la lista de pizzas.
   * Se crea un elemento `<thead>` para contener el encabezado de tabla.
   * La instrucción `@foreach` dentro de la iteración `<tbody>` sobre la lista de pizzas.
     * La propiedad `Model` hace referencia al objeto `PizzaListModel` que se creó en el archivo de código subyacente.
     * La propiedad `PizzaList` hace referencia a la propiedad `PizzaList` definida en el archivo de código subyacente.
   * Cada iteración de la instrucción `@foreach`crea un elemento `<tr>` para contener los datos de pizza:
     * La sintaxis de Razor se usa para mostrar los datos de pizza en los elementos `<td>`. Esta sintaxis se usa para mostrar las propiedades del objeto `Pizza` almacenado en la variable `pizza` .
     * `Price` tiene formato mediante la interpolación de cadenas de C#.
     * Se usa una expresión ternaria para mostrar el valor de la propiedad `IsGlutenFree` como "✔️" o una celda en blanco.
     * Se crea un formulario para eliminar la pizza.
       * El atributo `asp-page-handler` indica que el formulario debe enviarse al controlador `Delete` en el archivo de código subyacente. Creará ese controlador en una unidad posterior.
       * El atributo `asp-route-id` indica que la propiedad `Id` del objeto `Pizza` se debe pasar al controlador `Delete`.
3. Guarde el archivo. En el explorador, la página Lista de pizzas se actualiza con la lista de pizzas. Si usa GitHub Codespaces, el archivo se guarda automáticamente, pero tendrá que actualizar manualmente la pestaña del explorador.

![Captura de pantalla de la página Lista de pizzas con la lista de trabajo.](https://learn.microsoft.com/es-es/training/aspnetcore/create-razor-pages-aspnet-core/media/pizza-list.png)

¡Excelente trabajo! Ha creado una página de Razor que muestra una lista de pizzas. En la unidad siguiente, obtendrá información sobre los asistentes de etiquetas y los controladores de página.

### Entender las aplicaciones auxiliares de etiquetas y los controladores de página

En la unidad anterior, ha creado una página de Razor que muestra una lista de pizzas. Ha usado el símbolo `@` para cambiar de contexto entre HTML y C#. En esta unidad, obtendrá información sobre las  *aplicaciones auxiliares de etiquetas* . Las aplicaciones auxiliares de etiquetas son un tipo especial de elemento HTML que puede contener código de C#. También obtendrá información sobre los  *controladores de página* . Los controladores de página son métodos que controlan las solicitudes del explorador. Usará controladores de página en la unidad siguiente para agregar y eliminar pizzas.

#### Aplicaciones auxiliares de etiquetas

Las aplicaciones auxiliares de etiquetas se usan para abordar las ineficacias del cambio de contexto entre HTML y C#. La mayoría de las aplicaciones auxiliares de etiquetas integradas de ASP.NET Core amplían los elementos HTML estándar. Las aplicaciones auxiliares de etiquetas proporcionan atributos adicionales del lado servidor para los elementos HTML, lo que aumenta su solidez.

Hay cuatro aplicaciones auxiliares de etiquetas que debe conocer para este proyecto:  **Parcial** ,  **Etiqueta** , **Entrada** y  **Mensaje de resumen de la validación** .

#### Asistente de etiquetas parciales

**CSHTML**

```
<partial name="_ValidationScriptsPartial" />
```

Inserta el contenido del archivo `_ValidationScriptsPartial.cshtml` en una página. El archivo `_ValidationScriptsPartial.cshtml` contiene JavaScript que se usa para validar la entrada de formularios, por lo que debe incluirse en cada página que contenga un formulario.

#### Aplicación auxiliar de etiquetas

**CSHTML**

```
<label asp-for="Foo.Id" class="control-label"></label>
```

Extiende el elemento HTML `<label>` estándar. Como es común para muchas aplicaciones auxiliares de etiquetas, usa un atributo `asp-for`. El atributo acepta una propiedad de la clase `PageModel`. En este caso, el nombre de la propiedad `Foo.Id` de `PageModel` (específicamente, la cadena `"Id"`), se representará como el contenido de un elemento HTML `<label>`.

#### Aplicación auxiliar de etiquetas de entrada

**CSHTML**

```
<input asp-for="Foo.Id" class="form-control" />
```

De forma similar al ejemplo anterior, extiende el elemento HTML `<input>` estándar. También usa un atributo `asp-for` para especificar una propiedad `PageModel`. En este caso, el valor de la propiedad `Foo.Id` se representará como el atributo `value` de un elemento HTML `<input>`.

#### Asistente de etiquetas de resumen de validación

**CSHTML**

```
<div asp-validation-summary="All"></div>
```

La aplicación auxiliar de etiquetas de resumen de validación muestra un mensaje de validación para una única propiedad del modelo.

 Nota

Elementos como las reglas de validación y los nombres para mostrar de propiedad se definen en la clase `PageModel`. Señalaremos dónde encontrarlos en el código en la unidad siguiente.

#### Controladores de página

La clase `PageModel` define controladores de página para las solicitudes HTTP y los datos que se usan para representar la página. En el ejercicio anterior, la clase `PizzaListModel` controló la solicitud HTTP GET mediante el establecimiento del valor de la propiedad `PizzaList` en el valor de `_service.GetPizzas()`.

Entre los controladores comunes se incluyen `OnGet` para la inicialización de página y `OnPost` para los envíos de formularios. Para controlar un HTTP POST, un controlador de página podría comprobar los datos enviados por el usuario, presentar de nuevo la página del formulario de entrada si carece de validez o enviar los datos válidos a un servicio o base de datos para su conservación.

En la unidad siguiente, agregará un formulario para crear pizzas nuevas con varias aplicaciones auxiliares de etiquetas. También agregará controladores de página para controlar el envío de formularios y la eliminación de pizzas.

### Ejercicio: Adición de un nuevo formulario de pizza

En esta unidad, finalizará la página Lista de pizzas mediante la adición de un formulario para crear pizzas nuevas. También agregará controladores de página para controlar el envío de formularios y la eliminación de pizzas.

#### Agregar un formulario para crear pizzas nuevas

Empecemos agregando propiedades a la clase `PizzaListModel` para representar la entrada del usuario. También agregará el controlador de página adecuado.

1. Abra *Pages\PizzaList.cshtml.cs* y agregue la siguiente propiedad a la clase `PizzaListModel`:
   **C#**

   ```
   [BindProperty]
   public Pizza NewPizza { get; set; } = default!;
   ```

   En el código anterior:

   * Se agrega una propiedad llamada `NewPizza` a la clase `PizzaListModel`.
     * `NewPizza` es un objeto `Pizza`.
   * Se aplica el atributo `BindProperty` a la propiedad `NewPizza`.
     * El atributo `BindProperty` se usa para enlazar la propiedad `NewPizza` a la página de Razor. Al realizarse una solicitud HTTP POST, la propiedad `NewPizza` se rellenará con la entrada del usuario.
   * La propiedad `NewPizza` se inicializa en `default!`.
     * La palabra clave `default!` se usa para inicializar la propiedad `NewPizza` en `null`. Esto impide que el compilador genere una advertencia sobre la propiedad `NewPizza` que no se inicializa.
2. Ahora agregue el controlador de página para HTTP POST. En el mismo archivo, agregue el siguiente método a la clase `PizzaListModel`:
   **C#**

   ```
   public IActionResult OnPost()
   {
       if (!ModelState.IsValid || NewPizza == null)
       {
           return Page();
       }

       _service.AddPizza(NewPizza);

       return RedirectToAction("Get");
   }
   ```

   En el código anterior:

   * La propiedad `ModelState.IsValid` se usa para determinar si la entrada del usuario es válida.
     * Las reglas de validación se deducen a partir de atributos (como `Required` y `Range`) en la clase `Pizza` en  *Models\Pizza.cs* .
     * Si la entrada del usuario no es válida, se llama al método `Page` para volver a representar la página.
   * La propiedad `NewPizza` se usa para agregar una pizza nueva al objeto `_service`.
   * El método `RedirectToAction` se usa para redirigir al usuario al controlador de página `Get`, que volverá a representar la página con la lista actualizada de pizzas.
3. Guarde el archivo. Si usa GitHub Codespaces, el archivo se guarda automáticamente.
4. Vuelva al terminal en ejecución `dotnet watch` y presione **Ctrl+R** para volver a cargar la aplicación.

Ahora que hay un controlador de página para controlar el envío de formularios, vamos a agregar el formulario a la página de Razor.

1. Abra *Pages\PizzaList.cshtml* y reemplace `<!-- New Pizza form will go here -->` por el código siguiente:
   **razor**

   ```
   <form method="post">
   <div asp-validation-summary="ModelOnly" class="text-danger"></div>
   <div class="form-group">
       <label asp-for="NewPizza.Name" class="control-label"></label>
       <input asp-for="NewPizza.Name" class="form-control" />
       <span asp-validation-for="NewPizza.Name" class="text-danger"></span>
   </div>
   <div class="form-group">
       <label asp-for="NewPizza.Size" class="control-label"></label>
       <select asp-for="NewPizza.Size" class="form-control" id="PizzaSize">
           <option value="">-- Select Size --</option>
           <option value="Small">Small</option>
           <option value="Medium">Medium</option>
           <option value="Large">Large</option>
       </select>
       <span asp-validation-for="NewPizza.Size" class="text-danger"></span>
   </div>
   <div class="form-group form-check">
       <label class="form-check-label">
           <input class="form-check-input" asp-for="NewPizza.IsGlutenFree" /> @Html.DisplayNameFor(model => model.NewPizza.IsGlutenFree)
       </label>
   </div>
   <div class="form-group">
       <label asp-for="NewPizza.Price" class="control-label"></label>
       <input asp-for="NewPizza.Price" class="form-control" />
       <span asp-validation-for="NewPizza.Price" class="text-danger"></span>
   </div>
   <div class="form-group">
       <input type="submit" value="Create" class="btn btn-primary" />
   </div>
   </form>
   ```

   En el código anterior:

   * El atributo `asp-validation-summary` se usa para mostrar errores de validación para todo el modelo.
   * Cada campo de formulario (elementos `<input>` y `<select>`) y `<label>` se enlaza a la propiedad `NewPizza` con el atributo `asp-for`.
   * El atributo `asp-validation-for` se usa para mostrar errores de validación para cada campo de formulario.
   * El método `@Html.DisplayNameFor` se usa para mostrar el nombre para mostrar de la propiedad `IsGlutenFree`. Se trata de un método auxiliar de Razor que se usa para mostrar el nombre para mostrar de una propiedad. Con la etiqueta de esta forma, se garantiza que la casilla se active cuando el usuario haga clic en la etiqueta.
   * Un botón de envío se agrega al formulario para publicar los datos de formulario en el servidor. En tiempo de ejecución, el explorador enviará el formulario como una solicitud HTTP POST al servidor cuando el usuario haga clic en el botón de envío.
2. En la parte inferior de la página, agregue el código siguiente:
   **razor**

   ```
   @section Scripts {
   <partial name="_ValidationScriptsPartial" />
   }
   ```

   Inserta los scripts de validación del lado cliente en la página. Los scripts de validación del lado cliente se usan para validar la entrada del usuario antes de enviarse el formulario al servidor.
3. Guarde el archivo. En el explorador, la página Lista de pizzas se actualiza con el formulario nuevo. Si usa GitHub Codespaces, el archivo se guarda automáticamente, pero tendrá que actualizar manualmente la pestaña del explorador.
   ![Captura de pantalla de la página Lista de pizzas con el formulario de nueva pizza.](https://learn.microsoft.com/es-es/training/aspnetcore/create-razor-pages-aspnet-core/media/pizza-list-with-form.png)
4. Especifique una pizza nueva y seleccione el botón  **Crear** . La página debe actualizarse y mostrar la pizza nueva en la lista.

#### Agregar un controlador de página para eliminar pizzas

Hay un último componente para agregar a la página Lista de pizzas: un controlador de página para eliminar pizzas. Los botones para eliminar pizzas ya aparecen en la página, pero aún no hacen nada.

1. De nuevo en  *Pages\PizzaList.cshtml.cs* , agregue el siguiente método a la clase `PizzaListModel`:
   **C#**

   ```
   public IActionResult OnPostDelete(int id)
   {
       _service.DeletePizza(id);

       return RedirectToAction("Get");
   }
   ```

   En el código anterior:

   * Se llama al método `OnPostDelete` cuando el usuario hace clic en el botón **Eliminar** de una pizza.
     * La página sabe usar este método porque el atributo `asp-page-handler` en el botón **Eliminar** en *Pages\PizzaList.cshtml* se establece en `Delete`.
   * El parámetro `id` se usa para identificar la pizza que se va a eliminar.
     * El parámetro `id` se enlaza al valor de ruta `id` en la dirección URL. Esto se logra con el atributo `asp-route-id` en el botón **Eliminar** en  *Pages\PizzaList.cshtml* .
   * Se llama al método `DeletePizza` en el objeto `_service` para eliminar la pizza.
   * El método `RedirectToAction` se usa para redirigir al usuario al controlador de página `Get`, que volverá a representar la página con la lista actualizada de pizzas.
2. Guarde el archivo. Si usa GitHub Codespaces, el archivo se guarda automáticamente.
3. Pruebe el botón **Eliminar** de una pizza. La página debe actualizarse y la pizza seleccionada debe quitarse de la lista.

¡Enhorabuena! Ha creado correctamente una página de Razor en la que se muestra una lista de pizzas y que permite al usuario agregar pizzas nuevas y eliminar pizzas.

#### Comprobación de conocimientos

**1.** ¿Qué método usaría para controlar el envío de formularios en un elemento `PageModel`?

* [ ] Use un método `OnPost` (o `OnPostAsync`).
* [ ] Use un método `OnGet`.
* [ ] Use un `DataAnnotation` para controlar el envío de formularios.

#### Resumen

En este módulo, ha aprendido los conceptos básicos de Razor Pages. Ha aprendido a crear una página de Razor, agregar un modelo y agregar un controlador de páginas. También ha aprendido a usar asistentes de etiquetas para enlazar elementos HTML a propiedades del modelo y generar direcciones URL. Además, ha aprendido a usar la inserción de dependencias para insertar un servicio en una página de Razor.

#### Pasos siguientes

Profundice en la documentación. En este módulo se han presentado las características y los conceptos de ASP.NET Core siguientes:

* [Razor Pages](https://learn.microsoft.com/es-es/aspnet/core/razor-pages/)
* [Referencia de sintaxis Razor](https://learn.microsoft.com/es-es/aspnet/core/mvc/views/razor)
* [Aplicaciones auxiliares de etiquetas](https://learn.microsoft.com/es-es/aspnet/core/mvc/views/working-with-forms)
* [Vistas parciales](https://learn.microsoft.com/es-es/aspnet/core/mvc/views/partial)
* [Diseño](https://learn.microsoft.com/es-es/aspnet/core/mvc/views/layout)
* [Enrutamiento](https://learn.microsoft.com/es-es/aspnet/core/fundamentals/routing)
* [Inserción de dependencias](https://learn.microsoft.com/es-es/aspnet/core/fundamentals/dependency-injection)
* [Realización de solicitudes HTTP mediante IHttpClientFactory en ASP.NET Core](https://learn.microsoft.com/es-es/aspnet/core/fundamentals/http-requests#consumption-patterns)

#### Más información con una serie de vídeos de .NET

* [.NET para principiantes](https://www.youtube.com/playlist?list=PLdo4fOcmZ0oWoazjhXQzBKMrFuArxpW80)
* [ASP.NET Core para principiantes](https://www.youtube.com/playlist?list=PLdo4fOcmZ0oW8nviYduHq7bmKode-p8Wy)

## Creación de una API web con controladores de ASP.NET Core

Cree un servicio RESTful con controladores de ASP.NET Core que admita las operaciones de creación, lectura, actualización y eliminación (CRUD).

### Objetivos de aprendizaje

En este módulo, aprenderá a:

* Crear un proyecto de API web con controladores de ASP.NET Core.
* Cree una base de datos en memoria para almacenar productos.
* Agregue compatibilidad con las operaciones CRUD.
* Pruebe los métodos de acción de la API web desde el shell de comandos.

### Introducción

En este módulo, se explica cómo crear un servicio RESTful multiplataforma mediante controladores de la API web de ASP.NET Core con .NET y C#.

En este módulo se usan la [CLI (interfaz de la línea de comandos) de .NET](https://learn.microsoft.com/es-es/dotnet/core/tools/) y [Visual Studio Code](https://code.visualstudio.com/) para el desarrollo local. Cuando complete este módulo, podrá aplicar sus conceptos mediante un entorno de desarrollo como Visual Studio (Windows) y Visual Studio para Mac (macOS). También puede aplicar los conceptos al desarrollo continuo mediante Visual Studio Code (Windows, Linux y macOS).

#### Escenario de ejemplo

Imagine que es empleado de una empresa de pizzas llamada Contoso Pizza. El administrador le ha pedido que desarrolle un servicio RESTful de administración del inventario de pizzas como requisito previo para el escaparate web y la aplicación móvil de la empresa. El servicio debe permitir la adición, visualización, modificación y eliminación de tipos de pizzas; un uso estandarizado de los verbos de acción HTTP más conocidos como *crear, leer, actualizar y eliminar* (CRUD).

#### ¿Qué hará?

En este módulo va a crear una nueva aplicación de API web con ASP.NET Core y va a aprender a ejecutarla y probarla desde la línea de comandos. Luego va a agregar un almacén de datos y un nuevo controlador de API. Por último, va a implementar y probar los métodos de API para crear, leer, actualizar y eliminar pizzas del almacén de datos.

#### ¿Cuál es el objetivo principal?

Al final de esta sesión, podrá crear nuevas aplicaciones de API web mediante ASP.NET Core. También sabrá cómo crear controladores de API que implementen lógica CRUD básica.

### REST de ASP.NET Core

Al ir a una página web, el servidor web se comunica con el explorador mediante HTML, CSS y JavaScript. Si se interactúa con la página haciendo algo como enviar un formulario de inicio de sesión o seleccionar un botón de compra, el explorador envía la información de vuelta al servidor web.

De forma parecida, los servidores web pueden comunicarse mediante servicios web con una amplia gama de clientes, como exploradores, dispositivos móviles y otros servidores web. Los clientes de API se comunican con el servidor a través de HTTP, y los dos intercambian información mediante un formato de datos como JSON o XML. Las API se suelen usar en aplicaciones de página única (SPA) que realizan la mayor parte de la lógica de interfaz de usuario en un explorador web. La comunicación con el servidor web se produce principalmente a través de las API web.

#### REST: un patrón común para compilar API con HTTP

Transferencia de estado representacional (REST) es un estilo arquitectónico para compilar servicios web. Las solicitudes REST se realizan a través de HTTP. Usan los mismos verbos HTTP que usan los exploradores web para recuperar páginas web y enviar datos a los servidores. Los verbos son:

* `GET`: Recuperar datos del servicio web.
* `POST`: Crear un nuevo elemento de datos en el servicio web.
* `PUT`: Actualizar un elemento de datos en el servicio web.
* `PATCH`: Actualizar un elemento de datos en el servicio web describiendo un conjunto de instrucciones sobre cómo se debe modificar el elemento. La aplicación de ejemplo de este módulo no usa este verbo.
* `DELETE`: Eliminar un elemento de datos en el servicio web.

Las API de servicio web que se adhieren a REST se denominan API de RESTful. Se definen a través de:

* Identificador URI base.
* Métodos HTTP, como `GET`, `POST`, `PUT`, `PATCH` o `DELETE`.
* Un tipo de medio para los datos, como notación de objetos JavaScript (JSON) o XML.

Una API a menudo tiene que proporcionar servicios para unas cuantas cosas diferentes, aunque relacionadas. Por ejemplo, la API de pizzas puede administrar pizzas, clientes y pedidos. Usamos *enrutar* para asignar URI a divisiones lógicas del código, de modo que las solicitudes a https://localhost:5000/pizza se enruten a `PizzaController` y las solicitudes a https://localhost:5000/order lo hagan a `OrderController`.

#### Ventajas de crear API en ASP.NET Core

Con ASP.NET se pueden usar el mismo marco y los mismos patrones para compilar páginas web y servicios. Esto significa que se pueden reutilizar clases de modelos y lógica de validación, e incluso servir a páginas web y servicios en paralelo en el mismo proyecto. Este enfoque tiene ventajas:

* **Serialización simple** : ASP.NET diseñado para experiencias web modernas. Los puntos de conexión serializan automáticamente las clases en JSON con el formato correcto de serie. No se necesita ninguna configuración especial. Por supuesto, puede [personalizar la serialización](https://learn.microsoft.com/es-es/aspnet/core/web-api/advanced/custom-formatters) para los puntos de conexión con requisitos únicos.
* **Autenticación y autorización** : por motivos de seguridad, los puntos de conexión de API tienen compatibilidad integrada con JSON Web Token (JWT) estándares del sector. La autorización basada en directivas ofrece la flexibilidad necesaria para definir reglas de control de acceso eficaces en el código.
* **Enrutamiento junto con el código** : ASP.NET permite definir rutas y verbos en línea con el código, mediante atributos. Los datos de la ruta de acceso de la solicitud, la cadena de consulta y el cuerpo de la solicitud se enlazan automáticamente a parámetros de método.
* **HTTPS predeterminado** : HTTP es una parte importante de las API web modernas y profesionales. Se basa en el cifrado de un extremo a otro para proporcionar privacidad y ayudar a garantizar que las llamadas API no se intercepten ni se modifiquen entre el cliente y el servidor.
  ASP.NET proporciona compatibilidad con HTTPS de serie. Genera automáticamente un certificado de prueba y lo importa fácilmente para habilitar HTTPS local de modo que puede ejecutar y depurar las aplicaciones de forma segura antes de publicarlas.

#### Uso compartido de código y conocimientos con aplicaciones .NET

Puede usar sus aptitudes y el ecosistema de .NET para compartir la lógica de la API web con otras aplicaciones compiladas con .NET, como móviles, web, escritorio y servicios.

#### Prueba de API web mediante .NET HTTP REPL

Al desarrollar un sitio web tradicional, normalmente el trabajo se ve y se prueba en un explorador web. Las API web aceptan y devuelven datos en lugar de HTML, por lo que un explorador web no es la mejor herramienta de pruebas de API web.

Una de las opciones más fáciles para explorar API web e interactuar con ellas es .NET HTTP REPL. REPL significa  *read-evaluate-print loop* . Es una manera sencilla y popular de compilar entornos de línea de comandos interactivos. En la unidad siguiente va a crear una API web simple y a interactuar con ella mediante .NET HTTP REPL.

#### Comprobación de conocimientos

**1.** ¿Cuál de las siguientes *no* es una razón para compilar una API web mediante ASP.NET Core?

* [ ] Para proporcionar un servidor back-end para un front-end de SPA, como Angular o React.
* [ ] Proporcionar datos a una aplicación cliente móvil mediante XML o JSON.
* [ ] Servir a una aplicación web tradicional basada en HTML.

### Ejercicio: Creación de un proyecto de API web

En este módulo se usa el SDK de .NET 6.0. Asegúrese de que tiene instalado .NET 6.0 mediante la ejecución del siguiente comando en el terminal que prefiera:

**CLI de .NET**

```
dotnet --list-sdks
```

Verá un resultado similar al siguiente:

**Consola**

```
3.1.100 [C:\program files\dotnet\sdk]
5.0.100 [C:\program files\dotnet\sdk]
6.0.100 [C:\program files\dotnet\sdk]
```

Asegúrese de que aparece una versión que comienza por `6`. Si no aparece ninguna o no se encuentra el comando, [instale el SDK más reciente de .NET 6.0](https://dotnet.microsoft.com/download).

#### Creación y exploración de un proyecto de API web

Para configurar un proyecto de .NET para que funcione con API web se va a usar Visual Studio Code. Visual Studio Code incluye un terminal integrado que facilita la creación de un proyecto. Si no quiere usar un editor de código, puede ejecutar los comandos de este módulo en un terminal.

1. En Visual Studio Code, seleccione  **Archivo** > **Abrir carpeta** .
2. Cree una carpeta con el nombre **ContosoPizza** en la ubicación que prefiera y haga clic en  **Seleccionar carpeta** .
3. Abra el terminal integrado desde Visual Studio Code; para ello, seleccione  **Ver** >**Terminal** en el menú principal.
4. En la ventana del terminal, copie y pegue el siguiente comando:
   **CLI de .NET**

   ```
   dotnet new webapi -f net6.0
   ```

   Este comando crea los archivos para un proyecto de API web básico que usa controladores, junto con un archivo de proyecto de C# llamado  *ContosoPizza.csproj* , que va a devolver una lista de previsiones meteorológicas. Si se produce un error, asegúrese de que tiene instalado el [SDK de .NET 6](https://dotnet.microsoft.com/download).

   Importante

   Los proyectos de API web están protegidos con `https` de forma predeterminada. Si tiene problemas, [configure el certificado de desarrollo HTTPS de ASP.NET Core](https://learn.microsoft.com/es-es/aspnet/core/security/enforcing-ssl#trust-the-aspnet-core-https-development-certificate-on-windows-and-macos).

   Puede recibir un mensaje de Visual Studio Code para que agregue recursos a fin de depurar el proyecto. Seleccione **Sí** en el cuadro de diálogo.
   El comando usa una plantilla de proyecto de ASP.NET Core, con el alias  *webapi* , para aplicar scaffolding a un proyecto de API web basado en C#. Se crea un directorio  *ContosoPizza* . Este directorio contiene un proyecto ASP.NET Core que se ejecuta en .NET. El nombre del proyecto coincide con el nombre del directorio  *ContosoPizza* .
   Ahora debería tener acceso a estos archivos y directorios:
   **Bash**

   ```
   -| Controllers
   -| obj
   -| Properties
   -| appsettings.Development.json
   -| appsettings.json
   -| ContosoPizza.csproj
   -| Program.cs
   -| WeatherForecast.cs
   ```
5. Examine los archivos y directorios siguientes:

   | Nombre                  | Descripción                                                                                                                                     |
   | ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
   | *Controllers/*        | Contiene clases con métodos públicos expuestos como puntos de conexión HTTP.                                                                  |
   | *Program.cs*          | Configura los servicios y la canalización de solicitudes HTTP de la aplicación, y contiene el punto de entrada administrado de la aplicación. |
   | *ContosoPizza.csproj* | Contiene los metadatos de configuración del proyecto.                                                                                           |

#### Compilación y prueba de la API web

1. Ejecute el comando siguiente de la CLI de .NET Core en el shell de comandos:
   **CLI de .NET**

   ```
   dotnet run
   ```

   El comando anterior:

   * Busca el archivo de proyecto en el directorio actual.
   * Recupera e instala las dependencias de proyecto necesarias para este proyecto.
   * Compila el código del proyecto.
   * Hospeda la API web con el servidor web de Kestrel de ASP.NET Core en un punto de conexión HTTP y HTTPS.

   Se seleccionará un puerto de 5000 a 5300 para HTTP, y de 7000 a 7300 para HTTPS, en el momento de crear el proyecto. Los puertos usados durante el desarrollo se pueden cambiar fácilmente editando el archivo *launchSettings.json* del proyecto. En este módulo se usa la dirección URL `localhost` segura que comienza por `https`.
   Obtendrá una salida similar a la siguiente, que indica que la aplicación se está ejecutando:
   **Consola**

   ```
   Building...
   info: Microsoft.Hosting.Lifetime[14]
         Now listening on: https://localhost:7294
   info: Microsoft.Hosting.Lifetime[14]
         Now listening on: http://localhost:5118 
   info: Microsoft.Hosting.Lifetime[0]
         Application started. Press Ctrl+C to shut down.
   info: Microsoft.Hosting.Lifetime[0]
         Hosting environment: Development  
   ```

   Si ejecuta esta aplicación en su propio equipo, puede dirigir un explorador al vínculo HTTPS que se muestra en la salida (en el caso anterior, `https://localhost:7294`) para ver la página resultante. Recuerde este puerto, ya que lo usará en todo el módulo donde se usa `{PORT}`.
   Importante

   Compruebe la salida del terminal si detecta cualquier comportamiento inesperado. Si la compilación no se realiza correctamente o se producen otros errores, la información del archivo de registro ayuda a solucionar problemas. A medida que realice cambios en el código, deberá detener la API web; para ello, seleccione CTRL+C en el teclado y vuelva a ejecutar el comando `dotnet run`.
2. Abra un explorador web y vaya a:
   **Bash**

   ```
   https://localhost:{PORT}/weatherforecast
   ```

   Debería ver una salida JSON similar a la siguiente:

   **JSON**

   ```
   [
       {
       "date": "2021-11-09T20:36:01.4678814+00:00",
       "temperatureC": 33,
       "temperatureF": 91,
       "summary": "Scorching"
       },
       {
       "date": "2021-11-09T20:36:01.4682337+00:00",
       "temperatureC": -8,
       "temperatureF": 18,
       "summary": "Cool"
       },
       // ...
   ]
   ```
3. Abra un nuevo terminal integrado desde Visual Studio Code. Para ello, seleccione  **Terminal** >**Nuevo terminal** en el menú principal y ejecute el siguiente comando:
   **CLI de .NET**

   ```
   dotnet tool install -g Microsoft.dotnet-httprepl
   ```

   El comando anterior instala la herramienta de línea de comandos .NET HTTP REPL que se va a usar para realizar solicitudes HTTP a la API web.
4. Conéctese a la API web mediante el comando siguiente:
   **CLI de .NET**

   ```
   httprepl https://localhost:{PORT}
   ```

   Como alternativa, ejecute el siguiente comando en cualquier momento mientras `HttpRepl` se ejecuta:

   **CLI de .NET**

   ```
   connect https://localhost:{PORT}
   ```

   Sugerencia

   Si la herramienta `HttpRepl` muestra la advertencia  **No se puede encontrar una descripción de OpenAPI** , la causa más probable es un certificado de desarrollo que no es de confianza. `HttpRepl` requiere una conexión de confianza. Para poder continuar, **debe**[configurar el sistema para confiar en el certificado de desarrollo](https://learn.microsoft.com/es-es/aspnet/core/security/enforcing-ssl#trust-the-aspnet-core-https-development-certificate-on-windows-and-macos) con `dotnet dev-certs https --trust`.
5. Explore los puntos de conexión disponibles ejecutando el siguiente comando:
   **CLI de .NET**

   ```
   ls
   ```

   El comando anterior detecta todas las API disponibles en el punto de conexión conectado. Debería mostrar lo siguiente:

   **Resultados**

   ```
   https://localhost:{PORT}/> ls
   .                 []
   WeatherForecast   [GET] 
   ```
6. Ejecute el comando siguiente para ir al punto de conexión `WeatherForecast`:
   **CLI de .NET**

   ```
   cd WeatherForecast
   ```

   El comando anterior muestra una salida de las API disponibles para el punto de conexión `WeatherForecast`:

   **Resultados**

   ```
   https://localhost:{PORT}/> cd WeatherForecast
   /WeatherForecast    [GET]
   ```
7. Realice una solicitud `GET` en `HttpRepl` usando el comando siguiente:
   **CLI de .NET**

   ```
   get
   ```

   El comando anterior realiza una solicitud `GET` similar a ir al punto de conexión en el explorador:

   **Resultados**

   ```
   HTTP/1.1 200 OK
   Content-Type: application/json; charset=utf-8
   Date: Fri, 02 Apr 2021 17:31:43 GMT
   Server: Kestrel
   Transfer-Encoding: chunked
   [
       {
       "date": 4/3/2021 10:31:44 AM,
       "temperatureC": 13,
       "temperatureF": 55,
       "summary": "Sweltering"
       },
       {
       "date": 4/4/2021 10:31:44 AM,
       "temperatureC": -13,
       "temperatureF": 9,
       "summary": "Warm"
       },
       // ..
   ]
   ```
8. Cierre la sesión de `HttpRepl` actual con el siguiente comando:
   **CLI de .NET**

   ```
   exit
   ```
9. Vuelva al terminal `dotnet` en la lista desplegable de Visual Studio Code. Para apagar la API web, seleccione CTRL+C en el teclado.

Ahora que ha creado la API web, la modificará para satisfacer las necesidades de la API web de pizza.

### Controladores de API web de ASP.NET Core

En el ejercicio anterior se ha creado una aplicación web que proporciona datos de previsiones meteorológicas de ejemplo y luego se ha interactuado con ella en HTTP REPL.

Antes de profundizar en la escritura de su propia clase `PizzaController`, vamos a echar un vistazo al código del ejemplo `WeatherController` para comprender cómo funciona. En esta unidad, va a aprender cómo `WeatherController` usa la clase base `ControllerBase` y algunos atributos de .NET para compilar una API web funcional en unas docenas de líneas de código. Una vez que comprenda esos conceptos, estará listo para escribir su propia clase `PizzaController`.

Este es el código de la clase `WeatherController` completa. No se preocupe si aún no tiene sentido. Lo iremos viendo paso a paso.

**C#**

```
using Microsoft.AspNetCore.Mvc;

namespace ContosoPizza.Controllers;

[ApiController]
[Route("[controller]")]
public class WeatherForecastController : ControllerBase
{
    private static readonly string[] Summaries = new[]
    {
        "Freezing", "Bracing", "Chilly", "Cool", "Mild", "Warm", "Balmy", "Hot", "Sweltering", "Scorching"
    };

    private readonly ILogger<WeatherForecastController> _logger;

    public WeatherForecastController(ILogger<WeatherForecastController> logger)
    {
        _logger = logger;
    }

    [HttpGet(Name = "GetWeatherForecast")]
    public IEnumerable<WeatherForecast> Get()
    {
        return Enumerable.Range(1, 5).Select(index => new WeatherForecast
        {
            Date = DateTime.Now.AddDays(index),
            TemperatureC = Random.Shared.Next(-20, 55),
            Summary = Summaries[Random.Shared.Next(Summaries.Length)]
        })
        .ToArray();
    }
}

```

#### La clase base: `ControllerBase`

Un controlador es una clase pública con uno o varios métodos públicos llamados  *acciones* . Por convención, se coloca un controlador en el directorio *Controllers* de la raíz del proyecto. Las acciones se exponen como puntos de conexión HTTP a través del enrutamiento. Por lo tanto, una solicitud `GET` HTTP a `https://localhost:{PORT}/weatherforecast` hace que se ejecute el método `Get()` de la clase `WeatherForecastController`.

Lo primero que hay que tener en cuenta es que esta clase hereda de la clase base `ControllerBase`. Esta clase base proporciona una gran cantidad de funcionalidad estándar para controlar solicitudes HTTP, lo que permite centrarse en la lógica de negocios específica de la aplicación.

 Nota

Si tiene experiencia con el desarrollo con Razor Pages o el desarrollo de la arquitectura Modelo-Vista-Controlador (MVC) en ASP.NET Core, ha usado la clase `Controller`. No cree un controlador de API web mediante la derivación de la clase `Controller`. `Controller` se deriva de `ControllerBase` y agrega compatibilidad con vistas, por lo que sirve para gestionar páginas web, no solicitudes de API web.

#### Atributos de la clase API Controller

Se aplican dos atributos importantes a `WeatherForecastController`, como se muestra en el código siguiente:

**C#**

```
[ApiController]
[Route("[controller]")]
public class WeatherForecastController : ControllerBase
```

`[ApiController]` habilita [comportamientos fundamentados](https://learn.microsoft.com/es-es/aspnet/core/web-api/#apicontroller-attribute-1) que facilitan la compilación de API web. Algunos comportamientos incluyen [inferencia de origen de parámetros](https://learn.microsoft.com/es-es/aspnet/core/web-api/#binding-source-parameter-inference-1), [enrutamiento de atributos como un requisito](https://learn.microsoft.com/es-es/aspnet/core/web-api/#attribute-routing-requirement-1) y [mejoras en el control de errores de validación de modelos](https://learn.microsoft.com/es-es/aspnet/core/web-api/#automatic-http-400-responses-1).

`[Route]` define el patrón de enrutamiento `[controller]`. El token `[controller]` se sustituye por el nombre del controlador (no distingue mayúsculas de minúsculas ni tiene el sufijo  *Controller* ). Este controlador controla las solicitudes a `https://localhost:{PORT}/weatherforecast`.

 Nota

La ruta podría contener cadenas estáticas, como en `api/[controller]`. En este ejemplo, este controlador controlaría una solicitud a `https://localhost:{PORT}/api/weatherforecast`.

#### Generación de resultados meteorológicos con el método `Get()`

`WeatherForecastController` incluye una acción de controlador único, designada por el atributo `[HttpGet(Name = "GetWeatherForecast")]`. Este atributo enruta las solicitudes `GET` HTTP al método `public IEnumerable<WeatherForecast> Get()`. Por eso, en el ejercicio anterior, las solicitudes a `https://localhost:{PORT}/weatherforecast` dieron lugar a la devolución de los resultados meteorológicos.

Como aprenderá más adelante en este módulo, otras acciones comunes están asociadas a una API web que realiza operaciones CRUD (`GET`, `PUT`, `POST`, `DELETE`). Pero un controlador de API solo debe implementar una acción de controlador.

En este caso, se va a obtener la lista completa de `WeatherForecast` devueltos. La operación `GET` también permite recuperar un único elemento pasando un identificador. En ASP.NET, puede lograr esto mediante el atributo `[HttpGet("{id}")]`. Implementará ese atributo en el ejercicio siguiente.

Ahora que ha aprendido los componentes fundamentales de un controlador de API web, está listo para crear su propia clase `PizzaController`.

#### Comprobación de conocimientos

**1.** ¿Cuál es el propósito del atributo `[ApiController]`?

* [ ] `[ApiController]` habilita comportamientos bien fundamentados que facilitan la compilación de las API web.
* [ ] `ApiController` es la clase base, que proporciona funcionalidad estándar para controlar solicitudes HTTP.
* [ ] `[ApiController]` enruta solicitudes HTTP a la clase del controlador asociada.

### Ejercicio: Adición de un almacén de datos

Antes de empezar a implementar una API web para pizzas, es necesario tener un almacén de datos en el que puede realizar operaciones.

Necesita una clase `model` para representar una pizza en el inventario. El modelo contiene propiedades que representan las características de una pizza. El modelo se usa para pasar datos en la API web y para conservar opciones de pizza en el almacén de datos.

En esta unidad, ese almacén de datos es un servicio de almacenamiento en caché en memoria local simple. En una aplicación real se consideraría el uso de una base de datos, como SQL Server, con Entity Framework Core.

#### Creación de un modelo de pizza

1. Ejecute el siguiente comando para crear una carpeta  *Models* :
   **Bash**

   ```
   mkdir Models
   ```

   Seleccione la carpeta *Models* en Visual Studio Code y agregue un nuevo archivo de nombre  *Pizza.cs* .

   ![Captura de pantalla de la adición de un nuevo archivo a la carpeta Models en Visual Studio Code.](https://learn.microsoft.com/es-es/training/aspnetcore/build-web-api-aspnet-core/media/add-pizza-file.png)

   La raíz del proyecto ahora contiene un directorio *Models* con un archivo *Pizza.cs* vacío. El nombre del directorio *Models* es una convención. El nombre del directorio procede de la arquitectura Modelo-Vista-*Controlador* que usa la API web.
2. Agregue el código siguiente a *Models/Pizza.cs* para definir una pizza. Guarde los cambios.
   **C#**

   ```
   namespace ContosoPizza.Models;

   public class Pizza
   {
       public int Id { get; set; }
       public string? Name { get; set; }
       public bool IsGlutenFree { get; set; }
   }
   ```

#### Incorporación de un servicio de datos

1. Ejecute el comando siguiente para crear una carpeta  *Services* .
   **Bash**

   ```
   mkdir Services
   ```

   Seleccione la carpeta en Visual Studio Code y agregue un nuevo archivo de nombre  *PizzaService.cs* .

   ![Captura de pantalla de Visual Studio Code de la incorporación de un nuevo archivo a la carpeta Services.](https://learn.microsoft.com/es-es/training/aspnetcore/build-web-api-aspnet-core/media/add-pizza-service-file.png)
2. Agregue el código siguiente a *Services/PizzaService.cs* para crear un servicio de datos de pizzas en memoria. Guarde los cambios.
   **C#**

   ```
   using ContosoPizza.Models;

   namespace ContosoPizza.Services;

   public static class PizzaService
   {
       static List<Pizza> Pizzas { get; }
       static int nextId = 3;
       static PizzaService()
       {
           Pizzas = new List<Pizza>
           {
               new Pizza { Id = 1, Name = "Classic Italian", IsGlutenFree = false },
               new Pizza { Id = 2, Name = "Veggie", IsGlutenFree = true }
           };
       }

       public static List<Pizza> GetAll() => Pizzas;

       public static Pizza? Get(int id) => Pizzas.FirstOrDefault(p => p.Id == id);

       public static void Add(Pizza pizza)
       {
           pizza.Id = nextId++;
           Pizzas.Add(pizza);
       }

       public static void Delete(int id)
       {
           var pizza = Get(id);
           if(pizza is null)
               return;

           Pizzas.Remove(pizza);
       }

       public static void Update(Pizza pizza)
       {
           var index = Pizzas.FindIndex(p => p.Id == pizza.Id);
           if(index == -1)
               return;

           Pizzas[index] = pizza;
       }
   }
   ```

   Este servicio proporciona un sencillo servicio de almacenamiento en caché de datos en memoria con dos pizzas de forma predeterminada. Nuestra API web usará ese servicio con fines de demostración. Cuando se detiene y se inicia la API web, la caché de datos en memoria se restablecerá a las dos pizzas predeterminadas del constructor de `PizzaService`.

#### Compilación del proyecto de API web

Ejecute el siguiente comando para compilar la aplicación:

**CLI de .NET**

```
dotnet build
```

La compilación se ejecuta correctamente sin advertencias. Si se produce un error en la compilación, compruebe la salida con el fin de obtener información para solucionar problemas.

En la unidad siguiente, creará un controlador que usará el modelo `Pizza` y la clase `PizzaService`.

### Ejercicio: Adición de un controlador

Un *controlador* es una clase pública con uno o varios métodos públicos llamados  *acciones* . Por convención, se coloca un controlador en el directorio *Controllers* de la raíz del proyecto. Las acciones se exponen como puntos de conexión HTTP dentro del controlador de API web.

#### Creación de un controlador

1. Seleccione la carpeta *Controladores* en Visual Studio Code y agregue un nuevo archivo denominado  *PizzaController.cs* .
   ![Captura de pantalla de Visual Studio Code de la incorporación de un nuevo archivo a la carpeta Controladores.](https://learn.microsoft.com/es-es/training/aspnetcore/build-web-api-aspnet-core/media/add-pizza-controller-file.png)
   Se crea un archivo de clase vacío de nombre *ProductsController.cs* en el directorio  *Controllers* . El nombre del directorio *Controllers* es una convención. El nombre del directorio procede de la arquitectura Modelo-Vista-*Controlador* que usa la API web.
   Nota

   Por convención, los nombres de clase de los controladores llevan el sufijo  *Controller* .
2. Agregue el código siguiente a  *Controllers/PizzaController.cs* . Guarde los cambios.
   **C#**

   ```
   using ContosoPizza.Models;
   using ContosoPizza.Services;
   using Microsoft.AspNetCore.Mvc;

   namespace ContosoPizza.Controllers;

   [ApiController]
   [Route("[controller]")]
   public class PizzaController : ControllerBase
   {
       public PizzaController()
       {
       }

       // GET all action

       // GET by Id action

       // POST action

       // PUT action

       // DELETE action
   }
   ```

   Como ha aprendido anteriormente, esta clase se deriva de `ControllerBase`, la clase base para trabajar con solicitudes HTTP de ASP.NET Core. También incluye los dos atributos estándar sobre los que ha aprendido: `[ApiController]` y `[Route]`. Como antes, el atributo `[Route]` define una asignación al token `[controller]`. Dado que esta clase de controlador se denomina `PizzaController`, este controlador controla las solicitudes a `https://localhost:{PORT}/pizza`.

#### Obtención de todas las pizzas

El primer verbo REST que hay que implementar es `GET`, con el que un cliente puede obtener todas las pizzas de la API. Se puede usar el atributo integrado `[HttpGet]` para definir un método que devuelva las pizzas del servicio.

Reemplace el comentario `// GET all action` de *Controllers/ProductsController.cs* por el siguiente código:

**C#**

```
[HttpGet]
public ActionResult<List<Pizza>> GetAll() =>
    PizzaService.GetAll();
```

La acción anterior:

* Responde solo al verbo HTTP `GET`, tal y como indica el atributo `[HttpGet]`.
* Devuelve una instancia `ActionResult` de tipo `List<Pizza>`. El tipo `ActionResult` es la clase base para todos los resultados de acción en ASP.NET Core.
* Consulta el servicio en busca de todas las pizzas y devuelve automáticamente los datos cuyo `Content-Type` es `application/json`.

#### Recuperación de una única pizza

Es posible que el cliente también quiera solicitar información sobre una pizza específica en lugar de toda la lista. Se puede implementar otra acción `GET` que requiera un parámetro `id`. Se puede usar el atributo integrado `[HttpGet("{id}")]` para definir un método que devuelva las pizzas del servicio. La lógica de enrutamiento registra `[HttpGet]` (sin `id`) y `[HttpGet("{id}")]` (con `id`) como dos rutas diferentes. A continuación, puede escribir una acción independiente para recuperar un solo elemento.

Reemplace el comentario `// GET by Id action` de *Controllers/ProductsController.cs* por el siguiente código:

**C#**

```
[HttpGet("{id}")]
public ActionResult<Pizza> Get(int id)
{
    var pizza = PizzaService.Get(id);

    if(pizza == null)
        return NotFound();

    return pizza;
}
```

La acción anterior:

* Responde solo al verbo HTTP `GET`, tal y como indica el atributo `[HttpGet]`.
* Requiere que se incluya el valor del parámetro `id` en el segmento de URL después de `pizza/`. Recuerde que el atributo `/pizza` de nivel de controlador ha definido el patrón `[Route]`.
* Consulta la base de datos en busca de una pizza que coincida con el parámetro `id` proporcionado.

Cada instancia `ActionResult` usada en la acción anterior se asigna al código de estado HTTP correspondiente en la tabla siguiente.

| Resultado de la acción``de ASP.NET Core | Código de estado HTTP | Descripción                                                                                                                                                                                                                                                        |
| ---------------------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Ok` está implícito                  | 200                    | Hay un producto que coincide con el parámetro `id` proporcionado en la caché en memoria.``El producto se incluye en el cuerpo de la respuesta en el tipo multimedia que se define en el encabezado de solicitud HTTP `accept` (JSON de forma predeterminada). |
| `NotFound`                             | 404                    | No hay ningún producto que coincida con el parámetro `id` proporcionado en la caché en memoria.                                                                                                                                                                |

#### Compilación y prueba del controlador

1. Ejecute el siguiente comando para compilar e iniciar la API web:
   **CLI de .NET**

   ```
   dotnet run
   ```
2. Abra el terminal `httprepl` existente o uno nuevo integrado desde Visual Studio Code seleccionando  **Terminal** >**Nuevo terminal** en el menú principal.
3. Conéctese a la API web mediante el comando siguiente:
   **CLI de .NET**

   ```
   httprepl https://localhost:{PORT}
   ```

   Como alternativa, ejecute el siguiente comando en cualquier momento mientras `HttpRepl` se ejecuta:

   **CLI de .NET**

   ```
   connect https://localhost:{PORT}
   ```
4. Para ver el punto de conexión de `Pizza` ya disponible, ejecute el siguiente comando:
   **CLI de .NET**

   ```
   ls
   ```

   El comando anterior detecta todas las API disponibles en el punto de conexión conectado. Debería mostrar el código siguiente:

   **Resultados**

   ```
    https://localhost:{PORT}/> ls
    .                 []
    Pizza             [GET]
    WeatherForecast   [GET]
   ```
5. Ejecute el comando siguiente para ir al punto de conexión `Pizza`:
   **CLI de .NET**

   ```
   cd Pizza
   ```

   El comando anterior muestra una salida de las API disponibles para el punto de conexión `Pizza`:

   **Resultados**

   ```
   https://localhost:{PORT}/> cd Pizza
   /Pizza    [GET]
   ```
6. Realice una solicitud `GET` en `HttpRepl` usando el comando siguiente:
   **CLI de .NET**

   ```
   get
   ```

   El comando anterior devuelve una lista de todas las pizzas de JSON:

   **Resultados**

   ```
     HTTP/1.1 200 OK
     Content-Type: application/json; charset=utf-8
     Date: Fri, 02 Apr 2021 21:55:53 GMT
     Server: Kestrel
     Transfer-Encoding: chunked

     [
         {
             "id": 1,
             "name": "Classic Italian",
             "isGlutenFree": false
         },
         {
             "id": 2,
             "name": "Veggie",
             "isGlutenFree": true
         }
     ]
   ```
7. Para consultar en busca de una sola pizza, se puede realizar otra solicitud `GET`, pero pase un parámetro `id` usando el comando siguiente:
   **CLI de .NET**

   ```
   get 1
   ```

   El comando anterior devuelve `Classic Italian` con la salida siguiente.

   **Resultados**

   ```
   HTTP/1.1 200 OK
   Content-Type: application/json; charset=utf-8
   Date: Fri, 02 Apr 2021 21:57:57 GMT
   Server: Kestrel
   Transfer-Encoding: chunked

   {
       "id": 1,
       "name": "Classic Italian",
       "isGlutenFree": false
   }
   ```
8. La API también controla situaciones en las que el elemento no existe. Llame a la API de nuevo, pero pase un parámetro `id` de pizza no válido con el siguiente comando:
   **CLI de .NET**

   ```
   get 5
   ```

   El comando anterior devuelve un error `404 Not Found` con la siguiente salida:

   **Resultados**

   ```
   HTTP/1.1 404 Not Found
   Content-Type: application/problem+json; charset=utf-8
   Date: Fri, 02 Apr 2021 22:03:06 GMT
   Server: Kestrel
   Transfer-Encoding: chunked

   {
       "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
       "title": "Not Found",
       "status": 404,
       "traceId": "00-ec263e401ec554b6a2f3e216a1d1fac5-4b40b8023d56762c-00"
   }
   ```
9. Vuelva al terminal `dotnet` en la lista desplegable de Visual Studio Code y apague la API web presionando CTRL+C en el teclado.

Ya ha terminado de implementar los verbos `GET`. En la unidad siguiente, puede agregar más acciones a `PizzaController` para admitir operaciones CRUD en datos de pizza.

### Acciones CRUD de ASP.NET Core

Nuestro servicio de pizza admite operaciones CRUD para obtener una lista de pizzas. Estas operaciones se realizan a través de verbos HTTP, que se asignan a través de atributos de ASP.NET Core. Como ha visto, el verbo HTTP `GET` se usa para recuperar uno o varios elementos de un servicio. Esta acción se anota con el atributo `[HttpGet]`.

En la tabla siguiente se muestra la asignación de las cuatro operaciones que se están implementando para el servicio de pizzas:

| Verbo de acción HTTP | Operación CRUD | Atributo de ASP.NET Core |
| --------------------- | --------------- | ------------------------ |
| `GET`               | Lectura         | `[HttpGet]`            |
| `POST`              | Crear           | `[HttpPost]`           |
| `PUT`               | Actualizar      | `[HttpPut]`            |
| `DELETE`            | Eliminar        | `[HttpDelete]`         |

Ya ha visto cómo funcionan las acciones `GET`. Vamos a obtener más información sobre las acciones `POST`, `PUT` y `DELETE`.

#### POST

Para permitir que los usuarios agreguen un nuevo elemento al punto de conexión, debe implementar la acción `POST` mediante el atributo `[HttpPost]`. Al pasar el elemento (en este ejemplo, una pizza) al método como parámetro, ASP.NET Core convierte automáticamente cualquier aplicación o JSON enviado al punto de conexión en un objeto `Pizza` de .NET rellenado.

Esta es la firma del método `Create` que va a implementar en la sección siguiente:

**C#**

```
[HttpPost]
public IActionResult Create(Pizza pizza)
{  
    // This code will save the pizza and return a result
}
```

El atributo `[HttpPost]` asignará a las solicitudes HTTP `POST` enviadas a `http://localhost:5000/pizza` mediante el método `Create()`. En lugar de devolver una lista de pizzas, como vimos con el método `Get()`, este método devuelve una respuesta `IActionResult`.

`IActionResult` permite al cliente saber si la solicitud se ha solicitado correctamente y proporciona el identificador de la pizza recién creada. `IActionResult` lo hace con códigos de estado HTTP estándar, por lo que se integra fácilmente con los clientes, independientemente del lenguaje o la plataforma en la que se ejecuten.

| Resultado de la acción``de ASP.NET Core | Código de estado HTTP | Descripción                                                                                                                                                                                                           |
| ---------------------------------------- | ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `CreatedAtAction`                      | 201                    | La pizza se ha agregado a la caché en memoria.``La pizza se incluye en el cuerpo de la respuesta del tipo de medio según la definición del encabezado de solicitud HTTP `accept` (JSON de manera predeterminada). |
| `BadRequest` está implícito.         | 400                    | El objeto `pizza` del cuerpo de la solicitud no es válido.                                                                                                                                                          |

Afortunadamente, `ControllerBase` tiene métodos de utilidad que crean los mensajes y códigos de respuesta HTTP adecuados automáticamente. Va a ver cómo funcionan en el ejercicio siguiente.

#### PUT

La modificación o actualización de una pizza del inventario es similar al método POST que implementó, aunque usa el atributo `[HttpPut]` y toma el parámetro `id` además del objeto `Pizza` que se debe actualizar:

**C#**

```
[HttpPut("{id}")]
public IActionResult Update(int id, Pizza pizza)
{
    // This code will update the pizza and return a result
}
```

Cada instancia `ActionResult` usada en la acción anterior se asigna al código de estado HTTP correspondiente en la tabla siguiente.

| Resultado de la acción``de ASP.NET Core | Código de estado HTTP | Descripción                                                                           |
| ---------------------------------------- | ---------------------- | -------------------------------------------------------------------------------------- |
| `NoContent`                            | 204                    | La pizza se ha actualizado en la caché en memoria.                                    |
| `BadRequest`                           | 400                    | El valor `Id` del cuerpo de la solicitud no coincide con el valor `id` de la ruta. |
| `BadRequest` está implícito.         | 400                    | El objeto `Pizza` del cuerpo de la solicitud no es válido.                          |

#### DELETE

Una de las acciones más fáciles de implementar es la acción `DELETE`, que toma solo el parámetro `id` de la pizza que se va a quitar de la caché en memoria:

**C#**

```
[HttpDelete("{id}")]
public IActionResult Delete(int id)
{
    // This code will delete the pizza and return a result
}
```

Cada instancia `ActionResult` usada en la acción anterior se asigna al código de estado HTTP correspondiente en la tabla siguiente.

| Resultado de la acción``de ASP.NET Core | Código de estado HTTP | Descripción                                                                                      |
| ---------------------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------- |
| `NoContent`                            | 204                    | La pizza se ha eliminado de la caché en memoria.                                                 |
| `NotFound`                             | 404                    | No hay ninguna pizza que coincida con el parámetro `id` proporcionado en la caché en memoria. |

En el ejercicio de la siguiente unidad se muestra cómo admitir cada una de estas cuatro acciones en la API web.

#### Comprobar los conocimientos

**1.** Supongamos que necesita actualizar el nombre de un producto. ¿Qué verbo de acción HTTP es la mejor opción para esta solicitud?

* [ ] `POST`
* [ ] `PUT`
* [ ] `DELETE`

**2.** ¿En qué escenario es más adecuado devolver un código de estado HTTP 404 y cómo se consigue en ASP.NET Core?

* [ ] El producto se ha actualizado correctamente en la base de datos. Llame al método `BadRequest` para generar un código 404.
* [ ] Se ha producido un error en la validación del modelo porque faltan los parámetros necesarios de la acción. Llame al método `BadRequest` para generar un código 404.
* [ ] Después de solicitar un producto por su identificador, no hay ninguna coincidencia en el almacén de datos subyacente. Llame al método `NotFound` para generar un código 404.

### Ejercicio: Implementación de operaciones CRUD

Vamos a seguir ampliando el controlador de API web para agregar la capacidad de crear (`POST`), actualizar (`PUT`) y eliminar (`DELETE`) pizzas en el inventario.

#### Incorporación de una pizza

Habilitemos una pizza para agregarla a través de la API web mediante un método `POST`.

Reemplace el comentario `// POST action` de *Controllers/PizzaController.cs* por el código siguiente:

**C#**

```
[HttpPost]
public IActionResult Create(Pizza pizza)
{  
    PizzaService.Add(pizza);
    return CreatedAtAction(nameof(Get), new { id = pizza.Id }, pizza);
}
```

La acción anterior:

* Responde solo al verbo HTTP `POST`, tal y como indica el atributo `[HttpPost]`.
* Inserta el objeto `Pizza` del cuerpo de la solicitud en la caché en memoria.

 Nota

Dado que el controlador se anota con el atributo `[ApiController]`, está implícito que el parámetro `Pizza` se encontrará en el cuerpo de la solicitud.

El primer parámetro de la llamada al método `CreatedAtAction` representa un nombre de acción. Se usa la palabra clave `nameof` para evitar codificar de forma rígida el nombre de la acción. `CreatedAtAction` usa el nombre de la acción para generar un encabezado de respuesta HTTP `location` con una dirección URL a la pizza recién creada, como se ha explicado en la unidad anterior.

#### Modificación de una pizza

Ahora, habilitemos una pizza para actualizarla a través de la API web mediante un método `PUT`.

Reemplace el comentario `// PUT action` de *Controllers/PizzaController.cs* por el código siguiente:

**C#**

```
[HttpPut("{id}")]
public IActionResult Update(int id, Pizza pizza)
{
    if (id != pizza.Id)
        return BadRequest();
   
    var existingPizza = PizzaService.Get(id);
    if(existingPizza is null)
        return NotFound();
   
    PizzaService.Update(pizza);   
   
    return NoContent();
}
```

La acción anterior:

* Responde solo al verbo HTTP PUT, tal y como indica el atributo `[HttpPut]`.
* Requiere que se incluya el valor del parámetro `id` en el segmento de URL después de `pizza/`.
* Devuelve `IActionResult` porque no se conoce el tipo de valor devuelto `ActionResult` hasta el tiempo de ejecución. Los métodos `BadRequest`, `NotFound` y `NoContent` devuelven los tipos `BadRequestResult`, `NotFoundResult` y `NoContentResult`, respectivamente.

 Nota

Como el controlador se anota con el atributo `[ApiController]`, está implícito que el parámetro `Pizza` se encontrará en el cuerpo de la solicitud.

#### Eliminación de una pizza

Por último, habilitemos una pizza para quitarla a través de la API web mediante un método `DELETE`.

Reemplace el comentario `// DELETE action` de *Controllers/PizzaController.cs* por el código siguiente:

**C#**

```
[HttpDelete("{id}")]
public IActionResult Delete(int id)
{
    var pizza = PizzaService.Get(id);
   
    if (pizza is null)
        return NotFound();
   
    PizzaService.Delete(id);
   
    return NoContent();
}
```

La acción anterior:

* Responde solo al verbo HTTP `[HttpDelete]`, tal y como indica el atributo `DELETE`.
* Requiere que se incluya el valor del parámetro `id` en el segmento de URL después de `pizza/`.
* Devuelve `IActionResult` porque no se conoce el tipo de valor devuelto `ActionResult` hasta el tiempo de ejecución. Los métodos `NotFound` y `NoContent` devuelven los tipos `NotFoundResult` y `NoContentResult`, respectivamente.
* Consulta la caché en memoria en busca de una pizza que coincida con el parámetro `id` proporcionado.

No olvide guardar el archivo *Controllers/PizzaController.cs* antes de continuar.

#### Compilación y ejecución de la API web terminada

1. Ejecute el siguiente comando para compilar e iniciar la API web:
   **CLI de .NET**Copiar

   ```
   dotnet run
   ```
2. Vuelva a abrir el terminal `httprepl` existente o uno nuevo integrado desde Visual Studio Code seleccionando  **Terminal** >**Nuevo terminal** en el menú principal.
3. Si ha abierto un nuevo terminal, conéctese a la API web ejecutando el siguiente comando:
   **CLI de .NET**

   ```
   httprepl https://localhost:{PORT}
   ```

   Como alternativa, ejecute el siguiente comando en cualquier momento mientras `HttpRepl` se ejecuta:

   **CLI de .NET**

   ```
   connect https://localhost:{PORT}
   ```
4. Ejecute el comando siguiente para ir al punto de conexión `Pizza`:
   **CLI de .NET**

   ```
   cd Pizza
   ```
5. Ejecute el siguiente comando para ver las nuevas acciones en la API Pizza:
   **CLI de .NET**

   ```
   ls
   ```

   El comando anterior muestra una salida de las API disponibles para el punto de conexión `Pizza`:

   **Resultados**

   ```
       https://localhost:{PORT}/Pizza> ls
       .      [GET|POST]
       ..     []
       {id}   [GET|PUT|DELETE]
   ```
6. Realice una solicitud `POST` para agregar una nueva pizza en `HttpRepl` usando el comando siguiente:
   **CLI de .NET**

   ```
   post -c "{"name":"Hawaii", "isGlutenFree":false}"
   ```

   El comando anterior devuelve una lista de todas las pizzas:

   **Resultados**

   ```
   HTTP/1.1 201 Created
   Content-Type: application/json; charset=utf-8
   Date: Fri, 02 Apr 2021 23:23:09 GMT
   Location: https://localhost:{PORT}/Pizza?id=3
   Server: Kestrel
   Transfer-Encoding: chunked

   {
       "id": 3,
       "name": "Hawaii",
       "isGlutenFree": false
   }
   ```
7. Actualice la nueva pizza `Hawaii` a una `Hawaiian` con una solicitud `PUT` con el siguiente comando:
   **CLI de .NET**

   ```
   put 3 -c  "{"id": 3, "name":"Hawaiian", "isGlutenFree":false}"
   ```

   El comando anterior devuelve la siguiente salida que indica que se ha hecho correctamente:

   **Resultados**

   ```
   HTTP/1.1 204 No Content
   Date: Fri, 02 Apr 2021 23:23:55 GMT
   Server: Kestrel
   ```

   Para comprobar que la pizza se ha actualizado, vuelva a ejecutar la acción `GET` con el siguiente comando:
   **CLI de .NET**

   ```
   get 3
   ```

   El comando anterior devuelve la pizza recién actualizada:
   **Resultados**

   ```
   HTTP/1.1 200 OK
   Content-Type: application/json; charset=utf-8
   Date: Fri, 02 Apr 2021 23:27:37 GMT
   Server: Kestrel
   Transfer-Encoding: chunked

   {
       "id": 3,
       "name": "Hawaiian",
       "isGlutenFree": false
   }
   ```
8. La API también puede eliminar la pizza recién creada con la acción `DELETE` si ejecuta el siguiente comando:
   **CLI de .NET**

   ```
   delete 3
   ```

   El comando anterior devuelve un resultado `204 No Content` si es correcto:

   **Resultados**

   ```
   HTTP/1.1 204 No Content
   Date: Fri, 02 Apr 2021 23:30:04 GMT
   Server: Kestrel
   ```

   Para comprobar que la pizza se ha quitado, vuelva a ejecutar la acción `GET` con el siguiente comando:
   **CLI de .NET**

   ```
   get
   ```

   El comando anterior devuelve las pizzas originales como resultados:
   **Resultados**

   ```
   HTTP/1.1 200 OK
   Content-Type: application/json; charset=utf-8
   Date: Fri, 02 Apr 2021 23:31:15 GMT
   Server: Kestrel
   Transfer-Encoding: chunked

   [
       {
           "id": 1,
           "name": "Classic Italian",
           "isGlutenFree": false
       },
       {
           "id": 2,
           "name": "Veggie",
           "isGlutenFree": true
       }
   ]
   ```

Ya se ha terminado de implementar y probar la API web recién creada compilada con ASP.NET Core.

### Resumen

En este módulo, se ha creado una API web de ASP.NET Core que se ejecuta en .NET. La API web crea, lee, actualiza y elimina pizzas desde una caché en memoria.

Ha aprendido que la creación de una API web ASP.NET Core implica lo siguiente:

1. Creación de una nueva aplicación mediante la plantilla  *API web de ASP.NET Core* .
2. Creación de clases que heredan de la clase `ControllerBase` y que contienen métodos que responden a solicitudes HTTP.

Dado que este patrón permite centrarse en una sola acción de controlador a la vez, es posible crear API web funcionales con bastante rapidez con un poco de práctica.

En este módulo se ha usado una caché en memoria. Este enfoque le ha ayudado a centrarse en el aprendizaje de conceptos de API web, pero tiene algunas limitaciones obvias para las aplicaciones del mundo real. Si la aplicación se detiene, se pierden todos los cambios.

En una aplicación real se recomienda almacenar los datos en una memoria auxiliar, como una base de datos. Puede aprender a conservar y recuperar datos relacionales mediante Entity Framework Core en [este tutorial](https://learn.microsoft.com/es-es/training/modules/persist-data-ef-core/).

#### Vídeos para obtener más información

* [.NET 101](https://learn.microsoft.com/es-es/shows/NET-Core-101/?WT.mc_id=Educationaldotnet-c9-scottha)
* [API web de ASP.NET Core 101](https://learn.microsoft.com/es-es/shows/Beginners-Series-to-Web-APIs/)
* [ASP.NET Core 101](https://learn.microsoft.com/es-es/shows/ASPNET-Core-101/?WT.mc_id=Educationaspnet-c9-niner)

#### Artículos para obtener más información

* [Tutorial: Creación de una API web con ASP.NET Core](https://learn.microsoft.com/es-es/aspnet/core/tutorials/first-web-api)
* [Creación de API web con ASP.NET Core](https://learn.microsoft.com/es-es/aspnet/core/web-api/)
* [Tipos de valor devuelto de acción del controlador en la API web de ASP.NET Core](https://learn.microsoft.com/es-es/aspnet/core/web-api/action-return-types)

## Publicación de una aplicación web en Azure con Visual Studio

Use las características de publicación de Visual Studio 2022 para implementar y administrar una aplicación web ASP.NET Core hospedada en Azure.

### Introducción

Imagine que trabaja como desarrollador de software para una estación de esquí. Va a lanzar una nueva aplicación que permitirá que los usuarios vean los mapas de pistas y puedan comprar pases para el telesilla en el sitio web o desde sus teléfonos móviles. Quiere crear una aplicación web ASP.NET para complementar y publicitar la aplicación. Al ser un desarrollador de Visual Studio, quiere usar Visual Studio 2022 para crear, implementar y administrar el sitio nuevo.

Visual Studio y Azure App Service proporcionan un mecanismo eficaz para crear, publicar y mantener aplicaciones web en Azure. Aquí, aprenderá a usar las características de publicación integradas en Visual Studio para implementar y administrar las aplicaciones web ASP.NET hospedada en Azure.

#### Objetivos de aprendizaje

Objetivos de este módulo:

* Crear una aplicación web ASP.NET Core en Visual Studio
* Publicar una aplicación en Azure mediante Visual Studio
* Actualizar una aplicación web en Visual Studio y publicar los cambios en Azure

#### Requisitos previos

* Conocimiento del entorno de nube de Azure
* Familiaridad con Visual Studio 2022
* Familiaridad con los conceptos de aplicaciones web.
* Conocimientos básicos de programación
* Conocimientos básicos de HTML
* Una instalación local de Visual Studio 2022 en Windows

### Instalación de las cargas de trabajo necesarias

El primer paso para que el nuevo sitio esté listo es preparar el entorno de desarrollo. Para crear e implementar aplicaciones web ASP.NET Core, debe tener las herramientas necesarias instaladas en el equipo local. Aquí se tratarán las herramientas de desarrollo que necesita y cómo instalarlas.

#### Configuración del entorno de desarrollo

Necesitaremos instalar unas cuantas herramientas más en Visual Studio para compilar, depurar e implementar aplicaciones web ASP.NET Core en Azure. Para instalar estas herramientas, instalaremos dos *cargas de trabajo* de Visual Studio.

#### ¿Qué son las cargas de trabajo de Visual Studio?

Una *carga de trabajo* es un paquete preconfigurado de herramientas en Visual Studio. Estos paquetes se agrupan para permitir a los desarrolladores crear determinados tipos de aplicaciones, usar determinados lenguajes de desarrollo o desarrollar para plataformas específicas.

Por ejemplo, la carga de trabajo *Desarrollo para el escritorio con C++* incluye características de Visual Studio que le permiten ejecutar y depurar aplicaciones de consola de C++. La carga de trabajo *Desarrollo para dispositivos móviles con .NET* instala todas las herramientas necesarias para crear aplicaciones móviles con .NET.

#### Cargas de trabajo de Visual Studio para desarrollo y publicación de ASP.NET Core

Visual Studio 2022 tiene dos cargas de trabajo que necesita para crear, publicar e implementar el sitio web en Azure. Estas cargas de trabajo incluyen las plantillas del sitio de ASP.NET Core y le permiten conectarse a Azure e implementar ahí su sitio.

Con Visual Studio 2022 instalado, debe asegurarse de que tiene instaladas las siguientes cargas de trabajo de Visual Studio:

* **Desarrollo de ASP.NET y web** : La carga de trabajo de desarrollo web en Visual Studio está diseñada para maximizar la productividad al desarrollar aplicaciones web mediante ASP.NET y tecnologías basadas en estándares como HTML y JavaScript.
* **Desarrollo de Azure** : La carga de trabajo de desarrollo de Azure en Visual Studio instala el último Azure SDK para .NET y herramientas para Visual Studio. Una vez que instale estos elementos, puede crear recursos mediante las herramientas de Azure Resource Manager, compilar aplicaciones para los servicios web de Azure y Cloud Services, y realizar operaciones de macrodatos mediante herramientas de Azure Data Lake.

#### Instalación de cargas de trabajo de Visual Studio

Puede usar el Instalador de Visual Studio para modificar los componentes instalados como parte de Visual Studio, incluidas las cargas de trabajo.

1. Para iniciar el instalador, en el menú Inicio de Windows, desplácese hacia abajo hasta la **V** y después seleccione  **Instalador de Visual Studio** . Como alternativa, con el menú Inicio abierto, puede simplemente escribir `Visual Studio Installer` para encontrar el vínculo del instalador. Después, seleccione  **Introducir** .
2. Aparece la ventana del instalador de Visual Studio. Seleccione el botón  **Modificar** .
3. Asegúrese de que las cargas de trabajo **Desarrollo de ASP.NET y web** y **Desarrollo de Azure** están seleccionadas en la sección **Web y nube** de la pestaña  **Cargas de trabajo** .
4. Después, seleccione el botón **Modificar** en la parte inferior derecha del instalador. El Instalador de Visual Studio descargará e instalará los componentes necesarios.
5. Cuando se complete la instalación, seleccione **Iniciar** para abrir Visual Studio.

Las cargas de trabajo se agregan a la instalación local de Visual Studio y solo debe instalarlas una vez. Puede iniciar el Instalador de Visual Studio en el futuro para agregar más cargas de trabajo, personalizar las cargas de trabajo instaladas o quitarlas.

Para completar los ejercicios de este módulo, necesitará las cargas de trabajo **Desarrollo de ASP.NET y web** y  **Desarrollo de Azure** . Si todavía no lo ha hecho, instale estas cargas de trabajo antes de pasar al siguiente ejercicio.

### Ejercicio: Creación de una aplicación ASP.NET Core

En esta unidad, creará, compilará y ejecutará una nueva aplicación web ASP.NET en el equipo local. Necesitará tener Visual Studio 2022 instalado con las cargas de trabajo **Desarrollo de ASP.NET y web** y  **Desarrollo de Azure** .

#### Crear un proyecto de ASP.NET Core

1. Abra Visual Studio 2022 en el equipo local.
2. En la página de aterrizaje de Visual Studio, en  **Introducción** , seleccione  **Crear un nuevo proyecto** .
3. En el cuadro de búsqueda, escriba  **Web** .
4. En los resultados de la búsqueda, seleccione  **Aplicación web ASP.NET Core** .
5. Seleccione **Next** (Siguiente).
6. En el cuadro de diálogo del nuevo proyecto, establezca el campo **Nombre** en  **AlpineSkiHouse** .
7. Seleccione una **ubicación** para su nueva solución.
8. Seleccione  **Siguiente** .
9. Seleccione **.NET 6.0 (Compatibilidad a largo plazo)** en la lista desplegable Marco.
10. Seleccione **Crear** para crear el proyecto.
    Nota

    En este cuadro de diálogo también puede seleccionar otras plantillas de inicio en función de los requisitos de desarrollo web. En la parte superior del cuadro de diálogo, también puede seleccionar la versión de ASP.NET Core. Debe seleccionar ASP.NET Core 6.0 si es posible, aunque otras versiones recientes de ASP.NET Core también funcionarán con este ejercicio.
11. Ahora debe tener una nueva solución de aplicación web ASP.NET Core.

#### Compilación y prueba en la máquina local

Ahora, vamos a compilar y probar su aplicación en la máquina local antes de implementarla en Azure.

1. Ejecute la aplicación:
   Presione F5 para compilar el proyecto y ejecutarlo en modo de depuración.
   Presione Ctrl+F5 para compilar el proyecto y ejecutarlo sin asociar el depurador.
   Sugerencia

   Iniciar la aplicación en modo de no depuración permite realizar cambios en el código, guardar el archivo, actualizar el explorador y ver los cambios de código. Muchos desarrolladores prefieren usar el modo de no depuración para iniciar la aplicación y ver los cambios con rapidez.
2. Visual Studio inicia el explorador web de IIS Express y carga la aplicación.
   ![La aplicación web que se ejecuta en un explorador.](https://learn.microsoft.com/es-es/training/modules/publish-azure-web-app-with-visual-studio/media/3-webapp-launch-windows.png)
   Cuando Visual Studio crea un proyecto web, se usa un puerto aleatorio para el servidor web. En la imagen anterior, el número de puerto es 44381. Al ejecutar la aplicación, es posible que vea un número de puerto diferente.
   Importante

   Puede que vea cómo la sección de la parte superior de la página web proporciona un lugar para su directiva de uso de cookies y privacidad. Seleccione **Aceptar** para consentir el seguimiento. Esta aplicación no realiza un seguimiento de la información personal. El código generado por la plantilla incluye recursos para ayudar a cumplir el Reglamento general de protección de datos (RGPD).

Ya ha creado una aplicación web con la plantilla de ejemplo y se está ejecutando localmente. El siguiente paso es implementarla en Azure.

### Exploración de Azure App Service

Ha creado un nuevo sitio. El paso siguiente consiste en implementarlo en Azure. Debemos pensar en qué servicios de Azure vamos a aprovechar. Azure App Service proporciona un servicio de hospedaje web muy escalable y con aplicación de revisiones automática para las aplicaciones.

Aquí veremos cómo usar Visual Studio para publicar la aplicación web ASP.NET Core en un plan de Azure App Service.

#### ¿Qué es Azure App Service?

Azure App Service es un servicio para hospedar aplicaciones web, API REST y servicios de back-end. App Service admite código escrito en .NET Core, .NET Framework, Java, Ruby, Node.js, PHP y Python. App Service es recomendable para la mayoría de los sitios web, especialmente si no se necesita un control estricto sobre la infraestructura de hospedaje.

#### ¿Qué es el plan de App Service?

El plan de App Service define los recursos de proceso que usará la aplicación, dónde se encuentran esos recursos, cuántos recursos adicionales puede usar el plan y el tipo de plan de tarifa que se está usando. Estos recursos de proceso son análogos a la granja de servidores de un hospedaje web convencional. Puede configurar una o varias aplicaciones para que se ejecuten en el mismo plan de App Service.

Al implementar las aplicaciones, puede crear un plan de App Service o seguir agregando aplicaciones a un plan existente. Sin embargo, las aplicaciones del mismo plan de App Service comparten los mismos recursos de proceso. Para determinar si la nueva aplicación tiene los recursos necesarios, debe reconocer la capacidad del plan de App Service existente y la carga prevista para la nueva aplicación. La sobrecarga de un plan de App Service puede provocar un rendimiento reducido o tiempo de inactividad en las aplicaciones nuevas y existentes.

Puede definir un plan de App Service de antemano en Azure Portal con PowerShell o la CLI de Azure, o configurar uno mientras publica la aplicación en Visual Studio.

Cada plan de App Service define:

* Región (oeste de EE. UU., este de EE. UU., etc.)
* Número de instancias de VM
* Tamaño de las instancias de máquina virtual (pequeño, mediano, grande)
* Plan de tarifa (Gratis, Compartido, Básico, Estándar, Premium V2, Aislado)

#### Seleccione una región.

Al crear un plan de App Service, tiene que definir la región o ubicación donde se va a hospedar ese plan. Normalmente, se elige una región próxima geográficamente a los clientes previstos.

#### Niveles de precios y confiabilidad

 **Proceso compartido** : los dos planes básicos, **Gratis** y  **Compartido** , ejecutan una aplicación en la misma VM de Azure que otras aplicaciones de App Service, incluidas las aplicaciones de otros clientes. Estos planes asignan cuotas de CPU a cada aplicación que se ejecuta en los recursos compartidos, y los recursos no pueden escalarse horizontalmente.

Los planes Gratis y Compartido son ideales para proyectos personales a pequeña escala con demandas de tráfico limitadas, con un límite establecido de 165 MB de datos salientes cada 24 horas.

 **Proceso dedicado** : los planes **Básico, Estándar, Premium y V2** ejecutan aplicaciones en VM de Azure dedicadas. Solo las aplicaciones del mismo plan de App Service comparten los mismos recursos de proceso. Cuanto mayor sea el plan, más instancias de VM estarán disponibles para la escalabilidad horizontal.

El plan de servicio Estándar es ideal para cargas de trabajo de producción activas, donde se van a publicar aplicaciones comerciales para clientes.

Los planes de servicio Premium admiten aplicaciones web de alta capacidad donde no se quieren los costos adicionales de un plan dedicado (aislado).

 **Aislado** : este plan ejecuta VM de Azure dedicadas en instancias dedicadas de Azure Virtual Network, lo que proporciona aislamiento de red, además de aislamiento de proceso, a las aplicaciones. Proporciona las máximas posibilidades de escalabilidad horizontal. Solo se seleccionaría un plan de servicio Aislado en el caso de tener una necesidad concreta de los niveles más altos de seguridad y rendimiento.

Aísle la aplicación en un nuevo plan de App Service en los siguientes casos:

* La aplicación consume muchos recursos
* Quiere escalar la aplicación independientemente de las demás aplicaciones del plan existente
* La aplicación necesita recursos de otra región geográfica

Puede escalar el plan de App Service o reducir verticalmente en cualquier momento. Puede elegir un plan de tarifa inferior al principio y escalar verticalmente más adelante cuando necesite más características de App Service.

#### Especificación del grupo de recursos

Un grupo de recursos es un contenedor lógico en el que se implementan y administran recursos de Azure como aplicaciones web, bases de datos y cuentas de almacenamiento. Es un mecanismo para organizar los recursos con el fin de administrarlos, supervisarlos y facturarlos. Puede usar un grupo de recursos existente o crear uno directamente desde Visual Studio.

### Ejercicio: Publicación de una aplicación ASP.NET desde Visual Studio

Para completar este módulo, se necesita un espacio aislado. Un [espacio aislado](https://learn.microsoft.com/en-us/training/support/faq?pivots=sandbox) te da acceso a recursos gratuitos. La suscripción personal no se te cobrará. El espacio aislado solo se puede usar para realizar los cursos de Microsoft Learn. Está prohibido el uso con cualquier otro fin y puede dar lugar a la pérdida permanente del acceso al espacio aislado.

Microsoft proporciona esta experiencia de laboratorio y contenido relacionado con fines educativos. Toda la información presentada es propiedad de Microsoft y está destinada únicamente a aprender sobre los productos y servicios cubiertos en este módulo de Microsoft Learn.

Tiene una aplicación web ASP.NET Core que se ejecuta localmente. En este ejercicio, publicará la aplicación en Azure App Service

#### Publicación de la aplicación web ASP.NET Core en Azure

1. En el Explorador de soluciones, haga clic con el botón derecho en el proyecto **AlpineSkiHouse** y seleccione  **Publicar** .
2. En el cuadro de diálogo que aparece, seleccione **Azure** como destino de publicación y, después, seleccione **Siguiente** para continuar.
3. Seleccione **Azure App Service (Windows)** y después **Siguiente** para continuar.
   Sugerencia

   Las aplicaciones ASP.NET Core son multiplataforma. Esto significa que admiten la ejecución en la versión para Linux de App Service sin cambios de código. Pero la versión de Linux no es compatible con un modelo de hospedaje compartido, por lo que para este ejercicio se usará App Service de Windows.
4. En la lista desplegable  **Suscripción** , seleccione  **Suscripción de Concierge** .
5. Cerca del borde inferior del cuadro de diálogo, seleccione el vínculo **Crear una instancia de Azure App Service** para abrir el cuadro de diálogo  **App Service (Windows)** .

#### Configuración de la nueva instancia de Azure App Service

1. Si aún no ha iniciado sesión, inicie sesión en Visual Studio con la cuenta que está usando con Microsoft Learn.
2. Escriba la información necesaria sobre el plan de App Service.

   * **Nombre** : el nombre de la aplicación. El nombre determina la URL de la aplicación publicada, que será https://<NombreDeLaAplicación>.azurewebsites.net. Debe ser un valor único. Puede ser que tenga que probar varios nombres hasta encontrar uno que sea único.
   * **Suscripción** : la suscripción de Azure en la que quiere implementar la aplicación. Seleccione  **Suscripción de Concierge** , que se proporciona mediante el espacio aislado.
   * **Grupo de recursos:** seleccione el grupo de recursos [nombre del grupo de recursos del espacio aislado] existente.
   * **Plan de hospedaje** : el plan de hospedaje especifica la ubicación, el tamaño y las características de la granja de servidores web que hospeda la aplicación. Para este ejercicio, cree un plan de hospedaje.
     Seleccione **Nuevo** junto al plan de hospedaje. En la ventana Configurar un plan de hospedaje que aparece, cambie **Tamaño** a **Compartido** y seleccione  **Aceptar** .
3. Seleccione **Crear** para crear el recurso de App Service en Azure. Esta acción tardará varios segundos en completarse.
4. Transcurridos unos segundos, desaparecerá la ventana del cuadro de diálogo  **App Service (Windows)** . La nueva instancia de App Service se muestra en la lista de recursos de App Service en el cuadro de diálogo  **Publicar** . Seleccione **Finalizar** para terminar de crear el perfil de publicación. El cuadro de diálogo **Publicar** desaparecerá.
5. El nuevo perfil de publicación aparece en la lista desplegable situada junto a la parte superior de la página de propiedades. Seleccione **Publicar** para publicar la aplicación web en App Service.
6. Enhorabuena. Cuando vea un mensaje *Publicar correctamente* en la ventana  **Salida** , la aplicación web de ASP.NET Core ahora está publicada y activa. La dirección URL final del sitio está en la salida de la compilación y también en la página de publicación en Visual Studio.
7. Para probar el sitio web, vaya a la dirección URL indicada. Visual Studio también puede iniciar automáticamente esta dirección URL.
   ![Sitio activo.](https://learn.microsoft.com/es-es/training/modules/publish-azure-web-app-with-visual-studio/media/5-webpagelive.png)
   Nota

   Si no puede encontrar la dirección URL de la salida, vaya a https://<NombreDeLaAplicación>.azurewebsites.net, donde <NombreDeLaAplicación> es el nombre que ha proporcionado antes. Por ejemplo,  **"https://alpineskihouse123.azurewebsites.net/"** .

Ahora tiene una aplicación web activa. Se ha creado un plan de Azure App Service, y la aplicación está en ejecución y lista para aceptar actualizaciones.

### Exploración del proyecto de aplicación de Visual Studio

Ha creado correctamente la aplicación web y la ha publicado en Azure pero, ¿qué ocurre cuando quiere realizar cambios? Visual Studio recuerda dónde se ha publicado la aplicación, de modo que actualizarla o modificarla es un proceso sencillo.

#### Exploración de la estructura del proyecto

Ha creado una aplicación web de ASP.NET Core en Visual Studio y ahora tendrá que editar y personalizar el sitio web. Se examinará la estructura del proyecto para ver lo que Visual Studio ha creado.

#### Dependencias

La carpeta de dependencias incluye los aspectos internos de ASP.NET Core para que la aplicación funcione. A menos que vaya a agregar paquetes de terceros específicos, no tendrá que pasar mucho tiempo en esta carpeta.

#### Propiedades

La carpeta de propiedades contiene datos de configuración de donde se va a hospedar la aplicación web. Si expande ahora la carpeta  **PublishProfiles** , verá la dirección URL del sitio de Alpine Ski Hill. Cada perfil de publicación es un archivo .xml que contiene información de configuración de publicación, como la dirección de Azure que usa Visual Studio para cargar los archivos.

#### wwwroot

El archivo wwwroot contiene todos los recursos estáticos del sitio, como css, js, imágenes y archivos lib. Cuando esté listo para cambiar el estilo y agregar más funcionalidad a su sitio, trabajará aquí.

#### Páginas

En la carpeta **Pages** se incluyen plantillas de ***Razor*** para las páginas del sitio. Razor es una sintaxis de marcado para insertar código de servidor en páginas web de ASP.NET. Incluye HTML y tiene convenciones especiales para mostrar datos y ejecutar lógica en el sitio.

Cada página del sitio se representa con dos archivos de código:

* Un archivo `.cshtml`, que es el archivo de marcado de Razor. Este archivo contiene el código HTML de visualización y algo de lógica de C#.
* Un archivo `.cs`, que es el código subyacente de C# que hereda de la clase `PageModel`. Este archivo permite interceptar solicitudes HTTP y realizar cierto procesamiento en ellas antes de pasar los datos al archivo de Razor.

#### appsetting.json

Es un archivo de configuración de ASP.NET Core.

#### Program.cs

El archivo Program.cs configura e inicia el host web del sitio.

#### Introducción a las plantillas de Razor

Queremos hacer algunos cambios básicos en nuestro sitio web. Deberá tener un conocimiento básico de cómo sacar provecho de las plantillas de Razor para personalizar la aplicación web.

#### ¿Qué es Razor?

Razor es una sintaxis ASP.NET que se usa para crear páginas web dinámicas con C#. Cuando un servidor lee una página de Razor, el código de C# se ejecuta antes de representar el HTML. Esto le permite generar contenido dinámico rápidamente.

Razor usa directivas `@` para indicar a ASP.NET cómo procesar una página.

Por ejemplo, eche un vistazo al código de la página `Privacy.cshtml`:

**ASP.NET (C#)**

```
@page
@model PrivacyModel
@{
    ViewData["Title"] = "Privacy Policy";
}
<h1>@ViewData["Title"]</h1>

<p>Use this page to detail your site's privacy policy.</p>
```

* Por ejemplo, la directiva `@page` le dice a ASP.NET que procese este archivo como una página de Razor.
* La directiva `@model` le dice a ASP.NET que enlace esta página de Razor con una clase de C# llamada `PrivacyModel`.

Razor usa también el símbolo `@` para realizar la transición entre el código y HTML. Si examina el fragmento de código anterior, observará `@{ ... }`. Se trata de un  **bloque de código de Razor** , que se  *ejecuta pero no se representa* .

Para representar el resultado de una instrucción de código, se usa `@` delante de una expresión de C#. Hay un ejemplo en el bloque de código anterior, en la etiqueta `<h1>`.

La creación y publicación de un sitio web son solo los primeros pasos para crear un buen sitio web. Una vez que empiece a agregar contenido, deberá actualizar el sitio. Una vez que haya publicado el sitio en Azure, podrá actualizarlo en cualquier momento.

### Ejercicio: Publicación de una actualización en el sitio

La aplicación web Alpine Ski House está lista y en ejecución, pero ahora se la debe mostrar a su jefe. Va a tener que actualizar el sitio y publicar esas actualizaciones en Azure.

#### Actualización de la aplicación web

#### Reemplazar el código reutilizable

1. En la carpeta  **Páginas** , abra el archivo  **Privacy.cshtml** .
2. En la parte inferior del código, busque `<p>Use this page to detail your site's privacy policy.</p>`.
3. Reemplace el texto reutilizable por `<p>Welcome to the Alpine Ski House!</p>`.
4. Guarde el archivo.
5. Abra el archivo  **Index.cshtml** .
6. Reemplace el contenido de las etiquetas `<p>` para que indique **Alpine Ski House is the premier ski hill in Northeast!**
7. Guarde el archivo.

#### Publicar las actualizaciones

1. En el Explorador de soluciones, haga clic con el botón derecho en el proyecto.
2. Seleccione  **Publicar** . Se debería abrir una nueva pestaña denominada  **AlpineSkiHouse** .
3. Seleccione el botón **Publicar** para implementar los cambios más recientes.

#### Ver los cambios

Una vez que haya publicado los cambios, Visual Studio abrirá el sitio en el explorador. Ahora debería ver los nuevos mensajes en la página principal y la de privacidad.

Enhorabuena, la aplicación web se ha actualizado correctamente desde Visual Studio 2022.

### Resumen

En este módulo, ha creado una aplicación web ASP.NET desde cero y, después, la ha publicado directamente en Azure desde Visual Studio. Ha creado una aplicación de App Service, la ha actualizado y ha publicado los cambios, todo desde Visual Studio.

Visual Studio y Azure App Service proporcionan un mecanismo eficaz para crear, publicar y mantener aplicaciones web en Azure. Con esta combinación de simplicidad y capacidad de administración, mantener actualizadas las aplicaciones web en Azure se convierte en un proceso sencillo.

#### Limpieza

El espacio aislado limpia los recursos automáticamente cuando haya terminado con este módulo.

Al trabajar en una suscripción propia, se recomienda identificar al final de un proyecto si aún necesita los recursos creados. Los recursos que deja en ejecución pueden costar dinero. Puede eliminar los recursos de forma individual o eliminar el grupo de recursos para eliminar todo el conjunto de recursos.

## Introducción a .NET

Comience a obtener información sobre .NET. Conozca primero en qué consiste .NET y cómo funciona y cree rápidamente una aplicación pequeña en un entorno de .NET basado en Web.

### Introducción

Si no está familiarizado con el lenguaje de programación C#, es posible que no esté seguro de cómo se relaciona con .NET. Después de todo, parece que el término *.NET* se aplica a muchas cosas. ¿Qué es .NET? ¿C# forma parte de .NET? ¿Cómo funciona .NET? ¿Por qué es necesario obtener información sobre .NET?

En este módulo, obtendrá información sobre lo siguiente:

* .NET y su ecosistema
* Aspectos técnicos del sistema
* El rol de cada parte para ayudarlo a crear e implementar el software
* El ecosistema de .NET en conjunto, incluidos los recursos que pueden ayudarlo a aprender
* Cómo contribuir a este ecosistema

Por último, escribirá código de C# mediante un editor basado en Web para ver cómo funcionan juntos los elementos de .NET para crear una aplicación .NET.

Al final de este módulo, se habrá hecho una idea de qué es .NET, lo que le ayudará a llevar a cabo los pasos siguientes para crear aplicaciones .NET.

#### Objetivos de aprendizaje

Al término de este módulo, podrá hacer lo siguiente:

* Describa las partes principales de .NET y su ecosistema.
* Explique cómo funcionan de forma conjunta los lenguajes de .NET y el compilador, el entorno de ejecución y las bibliotecas de .NET para crear una aplicación en ejecución.
* Decida cuándo tiene sentido usar .NET para compilar aplicaciones.

#### Requisitos previos

* Ya debe haber escritas las primeras líneas de código de C#.
* Debe ser capaz de reconocer cómo usar `Console.WriteLine()` para enviar texto a una ventana de salida.
* Debe ser capaz de reconocer problemas poco importantes en el código y corregirlos.

Si aún no ha escrito una aplicación "Hola mundo" sencilla en C# , revise el primer módulo de la ruta de aprendizaje [Escritura de código de C# por primera vez](https://learn.microsoft.com/es-es/training/modules/csharp-write-first/).

### ¿Qué es .NET?

Cuando una persona usa el término  *.NET* , lo que quiere decir depende en gran medida del contexto. En esta unidad, obtendrá información sobre .NET, abordándolo como un ecosistema. En otras palabras, descubrirá que .NET es una colección de muchos elementos y personas que, de forma conjunta, crean un entorno eficaz para la compilación de aplicaciones.

#### .NET es un ecosistema para el desarrollo de aplicaciones

El término *ecosistema* describe las facetas múltiples de un entorno de desarrollo de aplicaciones y la comunidad que lo rodea. Estas diversas facetas son una razón de peso para invertir en el aprendizaje de .NET y la compilación de aplicaciones .NET.

#### Uso de lenguajes y compiladores de .NET para ejecutar aplicaciones en el entorno de ejecución de .NET

Los desarrolladores de software usan lenguajes de .NET, como C# y F#, para escribir código fuente. Cada línea de código que escriben expresa una instrucción o un comando que el equipo debe ejecutar mientras el programa se está ejecutando.

Antes de que los desarrolladores de software puedan ejecutar su código, deben compilarlo primero. El *compilador de .NET* es un programa que convierte el código fuente en un lenguaje especial denominado *lenguaje intermedio* (IL). El compilador de .NET guarda el código IL en un archivo denominado conocido como un  *ensamblado de .NET* . Al compilar el código en un formato "intermedio", se puede usar la misma base de código independientemente de dónde se ejecute el código, ya sea en Windows o Linux, o en hardware de equipo de 32 o 64 bits.

El *entorno de ejecución de .NET* es un entorno de ejecución diseñado para el ensamblado .NET compilado. En otras palabras, es lo que ejecuta y administra la aplicación cuando se ejecuta en un sistema operativo host. En breve veremos con más detalle lo que hace el entorno de ejecución de .NET.

Por suerte, al igual que le sucede a un desarrollador de software cuando empieza a usar .NET, no tiene que saber desde el principio cómo funcionan estos mecanismos. Al adquirir experiencia, entenderá mejor y apreciará más la eficacia subyacente de los lenguajes, los compiladores y el entorno de ejecución de .NET.

 Sugerencia

A veces, las personas piensan equivocadamente que el lenguaje de programación C# *es* .NET. Sin embargo, C# y .NET son distintos. C# es una sintaxis de lenguaje de programación. Como parte de la sintaxis, puede hacer referencia y llamar a métodos definidos en bibliotecas de código .NET, o  *ensamblados* . Además, para crear un ensamblado a partir del código de C#, se usa el compilador de C# que se instala con el SDK de .NET. El entorno de ejecución de .NET ejecuta ensamblados de .NET. Entender estas distinciones le ayudará a asimilar conceptos importantes conforme vaya aprendiendo más sobre .NET y C#.

#### Uso de marcos de aplicaciones y bibliotecas de .NET para aprovechar la funcionalidad predefinida

Todo el software se crea en capas, lo que significa que hay software que se ejecuta en distintos niveles de abstracción en un equipo:

* En el nivel más bajo, el software se comunica directamente con el hardware del equipo. Controla el flujo de datos en la placa base, los procesadores, la memoria y las unidades de disco duro.
* En el siguiente nivel, el software permite al usuario final proporcionar instrucciones a través de un sistema operativo.
* En el siguiente nivel, el software como .NET proporciona una manera de desarrollar y ejecutar aplicaciones.
* En el siguiente nivel, los marcos de trabajo de la aplicación y las bibliotecas de funcionalidad permiten crear rápidamente aplicaciones enriquecidas con menos esfuerzo que los métodos de desarrollo más antiguos permitidos.

Una biblioteca de código encapsula la funcionalidad para un fin específico en un único ensamblado. Para .NET, hay miles de bibliotecas disponibles. Estas bibliotecas pueden ser propias o de terceros, y pueden ser comerciales o de código abierto. Las bibliotecas proporcionan una amplia gama de funcionalidades que puede usar en sus aplicaciones. Simplemente debe hacer referencia a esos ensamblados y llamar a los métodos necesarios. De esta manera, como desarrollador, se basa en el trabajo de otros desarrolladores de software. Ahorra tiempo y esfuerzo, ya que no tiene que compilar y mantener todas las características.

Un marco de trabajo de aplicación combina varias bibliotecas relacionadas, junto con proyectos de inicio, plantillas de archivo, generadores de código y otras herramientas. Puede usar estos recursos para compilar aplicaciones completas con un fin específico. Estos marcos de trabajo de la aplicación se conocen como  *modelos de aplicación* . Por ejemplo, hay marcos de trabajo de aplicaciones de .NET populares disponibles para modelos de aplicación, como el desarrollo web, el desarrollo móvil y de escritorio, y desarrollo de juegos.

Puede instalar el SDK de .NET directamente o con la instalación de Visual Studio 2022. El SDK de .NET preinstala un conjunto completo de bibliotecas y marcos de trabajo de aplicaciones denominados  *biblioteca de clases base* . Puede usar esta biblioteca de código en sus programas, independientemente de los modelos de plataforma o aplicación que desee compilar.

En el caso de las bibliotecas de terceros, los desarrolladores usan administradores de paquetes como NuGet para buscar e integrar bibliotecas de código desde repositorios de paquetes, como la galería de NuGet.

#### ¿Cuáles son los principales modelos de aplicación?

Probablemente se preguntará qué modelos de aplicaciones admite cada marco de trabajo. Use la tabla siguiente para asignar un modelo de aplicación a un marco de trabajo de .NET.

| Modelo de aplicación | Marco                                 | Notas                                                                                                                                                                                                                                                                                                |
| --------------------- | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Web                   | ASP.NET Core                          | Marco para compilar lógica del lado servidor.                                                                                                                                                                                                                                                       |
| Web                   | ASP.NET Core MVC                      | Marco para compilar lógica del lado servidor para páginas web o API web.                                                                                                                                                                                                                           |
| Web                   | ASP.NET Core, Razor Pages             | Marco para compilar HTML generado por el servidor.                                                                                                                                                                                                                                                   |
| Cliente web           | Blazor                                | Blazor forma parte de ASP.NET Core. Sus dos modos permiten la manipulación de Document Object Model (DOM) a través de sockets como un vehículo de comunicación para ejecutar código del lado servidor, o bien como una implementación WebAssembly para ejecutar C# compilado en un explorador. |
| Escritorio            | WinForms                              | Marco para compilar aplicaciones clásicas de estilo Windows.                                                                                                                                                                                                                                        |
| Escritorio            | Windows Presentation Foundation (WPF) | Marco de trabajo para compilar aplicaciones de escritorio dinámicas que se ajustan a distintos factores de forma. WPF permite que los elementos de formulario realicen movimientos, atenuaciones, deslizamientos y otros efectos con la ayuda de una biblioteca completa de animaciones.            |
| Móvil                | Xamarin                               | Permite a los desarrolladores de .NET compilar aplicaciones para dispositivos iOS y Android.                                                                                                                                                                                                         |

Además, .NET habilita entornos conocidos de desarrollo de juegos de terceros y de código abierto y motores como Unity.

#### Use herramientas de .NET para compilar aplicaciones de .NET

Los desarrolladores de software emplean herramientas para escribir código, agregar referencias a bibliotecas de código, compilar código y depurarlo. En esta sección se describen varias herramientas de .NET que se usarán para compilar aplicaciones .NET.

*Visual Studio 2022* es el entorno de desarrollo insignia de Microsoft. Millones de desarrolladores lo usan para compilar aplicaciones .NET. Una interfaz gráfica de usuario (que incluye menús, ventanas, diseñadores visuales, cuadros de diálogo y asistentes) guía a los desarrolladores por el proceso de desarrollo de aplicaciones. Visual Studio 2022 está disponible en tres ediciones: Community, Professional y Enterprise. Cada edición incluye herramientas distintas y tiene licencia para propósitos diferentes.

Los desarrolladores que prefieran un flujo de trabajo de línea de comandos pueden usar una combinación de  *Visual Studio Code* , el editor de código más popular del mundo, y la interfaz de línea de comandos de .NET, también conocida como  *CLI de .NET* .

Además, puede elegir entre numerosas herramientas propias y de terceros para muchos casos de uso avanzados de .NET. Entre las opciones se incluyen generadores de perfiles de código, ejecutores de pruebas unitarias y analizadores de cobertura de código.

Puede encontrar otras herramientas de .NET para otros escenarios. Por ejemplo, más adelante en este módulo, trabajará con  *Try .NET* . Usará esta interfaz basada en el explorador para escribir aplicaciones sencillas que le ayudarán a conocer lenguaje de programación C#.

#### Búsqueda de soluciones y respuestas en la documentación y los tutoriales

Microsoft proporciona activamente un completo conjunto de documentación, tutoriales y aprendizaje. Encontrará materiales de aprendizaje en las modalidades populares que le ayudarán en cada paso del proceso de aprendizaje.

En la tabla siguiente se muestran algunos de los excelentes recursos que podrían convertirse en favoritos para volver a utilizarlos.

| Resource                                                                                     | Propósito                                                                                                                                                                                                                                                                                                                                             |
| -------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [Microsoft Learn](https://learn.microsoft.com/es-es/)                                           | Proporciona tutoriales de inicio rápido y documentación de referencia definitiva.                                                                                                                                                                                                                                                                    |
| [Patrones y prácticas](https://learn.microsoft.com/es-es/azure/architecture/)                  | Ayuda a los desarrolladores y arquitectos de software a encontrar soluciones que satisfagan necesidades comunes de desarrollo de aplicaciones. A menudo, los recursos superan los detalles de bajo nivel de escritura de código y profundizan en la elección de productos y servicios que permiten arquitecturas escalables aparentemente infinitas. |
| [Vídeos de .NET](https://dotnet.microsoft.com/learn/videos)                                    | Proporciona tutoriales de vídeo del equipo de .NET. Estos vídeos guían a los desarrolladores en los escenarios de uso comunes.                                                                                                                                                                                                                      |
| [Microsoft Learn](https://learn.microsoft.com/es-es/training/paths/get-started-c-sharp-part-1/) | Proporciona laboratorios prácticos que le ayudarán a desarrollar sus habilidades mediante una combinación de instrucciones, ejercicios, elementos multimedia, pruebas de conocimientos y un método para llevar un seguimiento del progreso.                                                                                                        |

#### Interactuar con la comunidad de .NET para aprender y compartir soluciones

El ecosistema de .NET va más allá de los lenguajes, las bibliotecas y las herramientas, para incluir también a los usuarios. Tiene la libertad de aprender de la comunidad y contribuir a ella.

* **Aprenda** : los miembros de la comunidad de .NET celebran eventos en línea en directo y reuniones en persona. Compilan software de código abierto, participan en foros de preguntas y respuestas y graban tutoriales en vídeo. Escriben libros y entradas de blog que le ayudarán a aprender y a superar los obstáculos cuando no sepa por dónde avanzar.
* **Contribuya** : es de código abierto y se puede encontrar en [GitHub](https://github.com/dotnet). Los proyectos de este repositorio se administran mediante .NET Foundation. una organización independiente dedicada a la expansión de un ecosistema de confianza de código abierto y fácil de obtener en el mercado, creado en torno a la plataforma de desarrollo de .NET. En este repositorio, puede compartir su perspectiva y opinión personal para ayudar a que otros aprendan.

#### ¿En qué se diferencia .NET de otros ecosistemas?

Si está familiarizado con el mundo del desarrollo de software, es posible que se pregunte en qué se diferencia .NET de otros ecosistemas. Para ser sinceros, otros ecosistemas pueden hacer algunas o muchas de las cosas que hemos mencionado hasta ahora en esta unidad.

Pero una de las características más distintivas de .NET es que su desarrollo y soporte técnico continuos se deben no solo a las contribuciones de un líder en el sector de la tecnología sino también de la comunidad. Se desarrollaron partes significativas de .NET con recursos de código abierto. Las aportaciones y las contribuciones de la comunidad no solo se reciben positivamente, sino que se alientan. De hecho, el 87 % de los colaboradores son ajenos a Microsoft. Según los comentarios de la comunidad, Microsoft apoya activamente la plataforma, ya que contribuye a su progreso con mejoras de características y de rendimiento, así como con correcciones de errores. Se han aceptado más de 100 000 solicitudes de incorporación de cambios de la comunidad.

Además, el ecosistema de .NET es muy dinámica:

* Hay más de cinco millones de desarrolladores de .NET.
* Los resultados de una encuesta de Stack Overflow realizada en 2019 y 2020 revelaron que .NET Core es el marco de trabajo más apreciado.
* A los alumnos les encanta .NET. El 40 % de los desarrolladores nuevos en .NET son estudiantes.
* Los repositorios de GitHub para .NET y ASP.NET están incluidos entre los 30 primeros proyectos de software de código abierto (OSS) de mayor velocidad.
* GitHub muestra C# en los cinco principales lenguajes de programación y el lenguaje aumenta en popularidad según el índice de la comunidad de programación TIOBE de 2020.
* .NET tiene el marco web más rápido del planeta según las [pruebas de TechEmpower](https://www.techempower.com/benchmarks/#section=data-r19&hw=ph&test=plaintext&a=2?azure-portal=true), un conjunto independiente de código abierto de pruebas comparativas de rendimiento web que evalúan docenas de lenguajes y marcos de trabajo de aplicaciones.

#### Breve historia de .NET

La versión original de .NET Framework se lanzó por primera vez a principios de 2002. Desde entonces, se han realizado muchas actualizaciones y también se han incorporado más funcionalidades. Tras años de mejoras y nuevas características, la versión original de .NET Framework, en especial las principales bibliotecas de código, mejoró significativamente.

Después 2002, Microsoft trabajó para crear una versión de .NET que ofreciera una compatibilidad multiplataforma. El objetivo era permitir a los desarrolladores escribir una base de código y usarla en los sistemas operativos macOS, Linux y Windows.

Gracias a estos esfuerzos, se presentó .NET Core en torno al año 2014. Microsoft ha mantenido la versión original de .NET Framework, pero las nuevas características y mejoras se reservan para .NET Core. Más adelante, se suprimió *Core* en el nombre. Las siguientes versiones principales son .NET 5, .NET 6, .NET 7, etc. Las versiones suelen publicarse cada noviembre.

¿Por qué es importante mencionar el historial de .NET? Porque puede que encuentre entradas de blog, vídeos y código fuente que tengan como destino la versión original de .NET Framework. En algunos casos, las instrucciones o el código siguen funcionando, pero en otros es posible que necesite realizar ajustes para adaptarse a la nueva versión de .NET.

### Cómo usar .NET

Esta unidad se centra en los aspectos *técnicos* de la compilación de una aplicación. Usaremos lenguajes, herramientas y marcos de trabajo de .NET para describir el flujo de trabajo general que los desarrolladores de software usan para compilar aplicaciones .NET.

#### Cómo usan .NET los desarrolladores para compilar aplicaciones

En esta sección se describe el flujo de trabajo de desarrollo de aplicaciones en .NET. Incluye detalles sobre cómo empezar a crear una aplicación en .NET.

#### Configurado su entorno de desarrollo

La primera decisión que toman los desarrolladores es seleccionar las herramientas que usarán para crear sus aplicaciones. En otras palabras, seleccionan su  *entorno de desarrollo* . La decisión suele basarse en si prefieren un flujo de trabajo más visual que incluya una interfaz gráfica de usuario, o bien una interfaz de la línea de comandos en la que se basarán casi exclusivamente en el teclado para navegar por el entorno de desarrollo y emitir comandos.

 Nota

Al final de este módulo, encontrará vínculos que le ayudarán a empezar a configurar el entorno de desarrollo. Puede elegir Visual Studio 2022 o Visual Studio Code y el kit de desarrollo de software (SDK) de .NET.

Para los desarrolladores que prefieren un entorno visual, Visual Studio 2022 es la mejor opción. Como puede imaginar, debido a la naturaleza exhaustiva y visual de Visual Studio 2022, se requiere más tiempo, ancho de banda y espacio en disco para descargar e instalar el programa. Sin embargo, algunos principiantes consideran que es la forma más fácil de empezar. En función de la velocidad de la conexión a Internet, la instalación puede tardar 15 minutos o más.

El Instalador de Visual Studio 2022 ofrece opciones en forma de cargas de trabajo. Una *carga de trabajo* es una colección de marcos, bibliotecas y otras herramientas que funcionan conjuntamente para compilar un modelo de aplicación específico. Según lo que aprendió en la unidad anterior, querrá asegurarse de que instala la carga de trabajo **Desarrollo multiplataforma de .NET Core** para compilar nuevas aplicaciones.

La carga de trabajo **Desarrollo multiplataforma de .NET Core** instala el SDK de .NET. El SDK de .NET contiene todas las bibliotecas, herramientas y plantillas que necesita para empezar a escribir código.

Si prefiere un entorno de línea de comandos, descargue e instale Visual Studio Code y el SDK de .NET por separado. Esta opción es popular para principiantes que desean empezar a trabajar rápidamente. Ambas herramientas requieren menos ancho de banda para su descarga.

#### Introducción

Normalmente, los proyectos de desarrollo de software comienzan con un conjunto de requisitos. Estos requisitos afectan a las opciones del modelo de aplicación. El modelo de aplicación que elija puede ser una aplicación web, de escritorio o móvil o un proceso en segundo plano, por ejemplo.

Tanto si usa Visual Studio 2022 como la CLI de .NET, por lo general empezará creando un proyecto basado en una plantilla de proyecto. Puede elegir entre muchas plantillas de proyecto. Plantillas del proyecto:

* Genere carpetas y archivos basados en plantillas y el nombre del proyecto que defina.
* Agregue referencias a las bibliotecas más usadas y a las bibliotecas que requiere el marco de trabajo del modelo de aplicaciones.
* Proporcione el código necesario que le permita ejecutar la aplicación y ver un pequeño ejemplo para asegurarse de que el código se compila.
* A veces, incluya instrucciones en el código. Estas instrucciones le guían para modificar la aplicación de ejemplo y personalizarla.

En Visual Studio 2022, el cuadro de diálogo **Nuevo proyecto** le ayuda a elegir visualmente un modelo de aplicación entre un conjunto de plantillas instaladas. También puede elegir entre muchas contribuciones de la comunidad. En la CLI de .NET, elija una nueva plantilla de proyecto mediante una combinación de un comando y marcas.

#### Funcionalidad de compilación

Después, empiece a escribir la lógica de la aplicación. Agregue referencias a las bibliotecas de código cuando necesite hacer tareas especiales, como las siguientes:

* Conectarse a recursos de red
* Acceder a una base de datos para almacenar o recuperar datos
* Convertir datos de un formato a otro
* Agregar registro para diagnosticar problemas con la aplicación

En algunos casos, las bibliotecas de código que quiere usar ya existen en el disco duro local porque se instalaron con el SDK de .NET.

En otros casos, los desarrolladores usan el administrador de paquetes NuGet para descargar y crear referencias a las bibliotecas de ensamblados. Para obtener estos recursos, en función del entorno de desarrollo, puede usar el cuadro de diálogo **Administrador de paquetes NuGet** de Visual Studio o la interfaz de línea de comandos de la CLI de .NET.

#### Compilación y ejecución de la aplicación

Al compilar una nueva funcionalidad, crea el código que se ejecuta con frecuencia. Este flujo de trabajo permite evaluar qué funciona correctamente y qué es necesario revisar. Tanto el enfoque visual como el enfoque de línea de comandos usan comandos simples que facilitan el seguimiento del flujo de trabajo.

La sintaxis del código se considera incorrecta cuando esta no sigue las reglas del lenguaje. Cuando la sintaxis es incorrecta, el compilador de .NET para su lenguaje produce un  *error de compilación* . El compilador no continuará hasta que se corrija el problema de sintaxis.

A veces, el código puede compilarse porque sigue las reglas de sintaxis, pero la lógica de la aplicación tiene problemas. Si la lógica evita que el entorno de ejecución de .NET ejecute un comando, el programa "se bloquea". El entorno de ejecución de .NET quita el programa de la memoria del equipo. Esto son los llamados *errores en tiempo de ejecución* o  *excepciones* .

 Sugerencia

Afortunadamente, se puede evitar mediante programación que los usuarios reciban estos desagradables mensajes de error. Busque tutoriales y documentación sobre el "control estructurado de excepciones" para obtener más información.

Algunos errores lógicos no provocan "bloqueos". Pero tampoco generan los resultados que esperan los usuarios. Solo puede solucionar estos errores si prueba y depura la aplicación.

#### Depuración de la aplicación

Mientras compila el software, ejecute la aplicación para comprobar si cumple sus requisitos y expectativas. Puede que detecte un error en la aplicación, pero que no sepa *por qué* se produce o *cómo* solucionarlo.

Al depurar, verá la aplicación mientras se ejecuta para comprender lo que está ocurriendo. Puede establecer puntos de interrupción que pausan la aplicación y permiten realizar un seguimiento del código mientras se ejecuta. Puede observar el valor almacenado en variables, controlar la ruta de acceso en ejecución mediante el código para omitir o volver a ejecutar líneas, cambiar el valor de las variables, etc.

Las herramientas de depuración visual y de línea de comandos permiten observar y controlar la ejecución de la aplicación. Use esta funcionalidad para ver lo que está ocurriendo en su aplicación mientras se ejecuta.

#### Distribuya la aplicación

Cuando la aplicación esté lista para su lanzamiento, debe crear una versión de lanzamiento de la compilación. En una versión de lanzamiento, quite el código necesario para la depuración. Una vez más, tanto en la depuración visual como de línea de comandos, puede compilar una versión de lanzamiento.

Para ejecutar la versión de lanzamiento, debe instalar el entorno de ejecución de .NET en el equipo de destino. Este equipo ejecutará el ensamblado .NET compilado.

#### Cómo funciona .NET en tiempo de ejecución

Una vez que el ensamblado .NET de la aplicación y el entorno de ejecución de .NET estén instalados en el equipo de destino, puede ejecutar la aplicación.

El *entorno de ejecución de .NET* es como una burbuja de protección que proporciona un entorno de ejecución para las aplicaciones. Entorno de ejecución de .NET:

* Compila el código intermedio en un formato binario la primera vez que se ejecuta el programa. El formato binario es específico de la plataforma y la arquitectura (por ejemplo, Windows de 64 bits) en el equipo en el que se ejecuta.
* Busca el punto de entrada del programa y empieza a ejecutar cada instrucción en el orden adecuado.
* Administra recursos del equipo, como la memoria y el acceso a la red. Cuando escucha que el entorno de ejecución de .NET "administra la memoria", significa que funciona con el sistema operativo para aprovisionar memoria para la aplicación. Cuando la aplicación ya no necesita los datos almacenados en memoria, una característica de recopilación de elementos no utilizados libera la memoria del sistema operativo sin instrucciones del desarrollador de software.
* Protege el equipo del usuario del software que puede tener intenciones malintencionadas. También proporciona un nivel de aislamiento entre las aplicaciones.

### Compilación de la primera aplicación con Try .NET

Al principio de este módulo, asumimos que ya había escrito una aplicación "Hola mundo" con C#. De lo contrario, revise el primer módulo de esta ruta de aprendizaje, [Escritura de código de C# por primera vez](https://learn.microsoft.com/es-es/training/modules/csharp-write-first/).

Para simplificar, se volverá a escribir la aplicación "Hola mundo". Esta vez vamos a adoptar una perspectiva de .NET sobre lo que sucede en segundo plano.

#### Compilación de una aplicación sencilla con C#

Anteriormente, aprendió que Try .NET proporciona una manera sencilla de experimentar con C# y .NET. Puede usarlo sin necesidad de instalar ningún software en el equipo local.

 Nota

En este módulo, se usa una versión integrada de Try .NET. Si desea experimentar con la aplicación después de finalizar este ejercicio, vaya a `https://try.dot.net`. Try .NET es una excelente manera de probar pequeños ejemplos de código sin necesidad de instalar nada en el equipo local.

#### Paso 1: escritura del código

En el editor de .NET, en el lado derecho de esta página web, escriba el siguiente ejemplo de código. O copie el ejemplo de código y péguelo en el editor de .NET.

**C#**

Ejecutar

```
Console.WriteLine("Hello world!");
```

Como bien ha aprendido en el módulo de requisitos previos, "Hola mundo" es un ejemplo de código simple y canónico que los desarrolladores escriben para comprender la sintaxis básica de los nuevos lenguajes de programación. Podría aprender mucho sobre la sintaxis de C# en este sencillo ejemplo. Pero por ahora, lo usaremos para obtener más información sobre .NET específicamente.

#### Paso 2: ejecución del código

Haga clic en el botón verde **Ejecutar** situado a la derecha del editor de .NET. Suponiendo que insertó el código de C# correctamente, las palabras "Hola mundo" aparecen en el panel **Salida** siguiente.

 Importante

Si ve algún error mientras ejecuta este código, copie el código y péguelo en el editor de .NET. Después intente ejecutar el código de nuevo.

#### ¿Qué ocurre con el código que se escribe?

La versión en el explorador de Try .NET oculta parte del código que se ve al compilar una aplicación completa mediante Try .NET, Visual Studio 2022 o Visual Studio Code.

Al incluir el código oculto, este es el aspecto del ejemplo:

**C#**

```
using System;

public class Program
{
  public static void Main()
  {
    Console.WriteLine("Hello world!");
  }
}
```

A pesar de ello, el entorno de Try .NET en el explorador usa los mismos pasos que aprendió anteriormente. La única diferencia es que parte del código se oculta para simplificar la experiencia.

Si se centra en esa vista ampliada del código, puede ver una serie de llaves `{ }`. C# utiliza un par de llaves para definir un  *bloque de código* . Se utilizan diferentes tipos de bloques de código para distintos propósitos.

El código `public static void Main()` y su conjunto de llaves definen un tipo de bloque de código que se conoce como un  *método* . Un método contiene una agrupación de código que funciona para un único propósito o responsabilidad en el sistema de software.

En este caso, el método contiene una sola línea de código. Su finalidad es mostrar un mensaje. Los programas más grandes pueden tener cientos o miles de métodos.

Los métodos se organizan dentro de otros bloques de código denominados clases. Una *clase* puede contener uno o más métodos. Lo ideal es que todos los métodos de una clase tengan un propósito relacionado en el sistema. En el código anterior, la clase se denominaba `Program`.

En la línea de código insertada, `Console.WriteLine()`*llama* al método `WriteLine()` o lo ejecuta. El método `WriteLine()` está contenido en la clase `Console`.

¿Dónde está este código? Se encuentra en la biblioteca de clases base. En realidad, su nombre completo es `System.Console.WriteLine()`. En el código anterior, verá que la primera línea es:

**C#**

```
using System;
```

La palabra `System` se omite en la llamada a `Console.WriteLine()`. Sin embargo, la primera línea de código `using System;` indica al compilador de C# que busque en la biblioteca de clases base si no encuentra la definición del método en el código.

 Nota

No se preocupe por términos específicos de C#, como método, clase, sistema y uso. Obtendrá más información al respecto más adelante. Ahora nos enfocaremos en el proceso de compilar y ejecutar el código.

#### ¿Qué ocurre con el código después de insertarlo en el método Main()?

La parte más importante de este ejercicio es lo que ocurre después de que el código que escriba se inserte en un método `Main()`. Tenga en cuenta que este proceso se produce en un servidor en su nombre.

1. Un comando para compilar el código nuevo invoca al compilador de C#.
2. El compilador de C# garantiza que el código se pueda compilar y esté libre de errores de sintaxis. Si no puede compilar el código, el compilador se detiene y envía un mensaje de error al panel  **Salida** .
3. Si el compilador de C# se ejecuta correctamente, el entorno de ejecución de .NET abre el ensamblado de .NET recién compilado. De forma predeterminada, busca en una clase denominada `Program` para buscar un método llamado `Main()` para empezar a ejecutar las instrucciones.
4. Instrucción por instrucción, el entorno de ejecución de .NET evalúa cada línea de código. Ejecuta la instrucción y se mueve a la siguiente línea de código.
5. En este caso, cuando finaliza la instrucción para imprimir las palabras "Hola mundo", la ruta de acceso en ejecución continúa hasta la línea siguiente, pero no encuentra nada. La ruta de acceso finaliza y el entorno de ejecución de .NET quita el programa de su memoria. Mientras tanto, la salida de la instrucción `WriteLine()` se devuelve al explorador web.

Esta secuencia de eventos, y la división básica de responsabilidades entre un lenguaje de programación, un compilador y un entorno de ejecución son los conceptos más importantes de entender para empezar.

### Cuándo se debe usar .NET

En esta unidad, aprenderá cuándo es recomendable usar .NET. ¿Cuándo tiene sentido optar por .NET? ¿Qué se puede compilar con .NET?

#### .NET sirve para proyectos grandes y pequeños.

Puede preguntarse si .NET es un ecosistema en el que compensa invertir tiempo de aprendizaje. Millones de desarrolladores utilizan .NET cada día para hacer cosas sorprendentes. Proporciona herramientas para crear los tipos de aplicaciones que les importan.

#### Elija .NET cuando la productividad sea importante

Una vez que haya aprendido a compilar una aplicación basada en un modelo de aplicación, puede aplicar fácilmente lo aprendido para compilar lo que quiera, aunque sea un modelo de aplicación diferente. Por ejemplo, una vez haya aprendido a compilar una aplicación web, puede aprovechar sus conocimientos de .NET para compilar una aplicación móvil.

Al readaptar sus conocimientos, se reduce el tiempo y el esfuerzo que implica el aprendizaje de un nuevo lenguaje o modelo de programación. Su empresa ahorra tiempo y gastos cuando se le plantean nuevos desafíos.

#### Elija .NET para aplicaciones a escala empresarial

.NET es popular en las empresas por diversos motivos. Entre las ventajas se incluyen su ecosistema y su integración con otros productos de Microsoft, incluidos los servicios en la nube de Azure y los productos de servidor locales. Además, .NET es un sistema fuertemente tipado, por lo que evita muchos de los errores que pueden surgir en sistemas débilmente tipados. Los desarrolladores pueden optar por usar un paradigma basado en objetos en C# o un paradigma basado en la funcionalidad en F# . Usan el lenguaje que mejor se adapte a los tipos de problemas que necesitan resolver.

#### Elección de .NET para prototipos, startups y aplicaciones a pequeña escala

.NET es también una opción popular para proyectos pequeños debido a su largo historial de mejoras en el diseño de los lenguajes, las API y las herramientas, gracias a los comentarios de los clientes y la telemetría. Puede usarlo para desarrollar rápidamente nuevo software con todas las características para crear prototipos. Además, .NET puede ejecutarse en servicios de hardware y en la nube económicos. También supera a otras plataformas populares, por lo que es una buena opción para startups.

#### Elija .NET para aplicaciones de IA y en la nube

El SDK de Azure para .NET permite a los desarrolladores aprovisionar y administrar recursos de Azure. Como alternativa, Azure App Service y Azure Functions pueden hospedar aplicaciones compiladas con lenguajes .NET.

ML.NET es una biblioteca de aprendizaje automático gratuita para los lenguajes .NET. Habilita las funcionalidades de análisis y predicción de Machine Learning basadas en modelos.

#### Elija .NET para compilar aplicaciones de IoT

Puede usar .NET para compilar aplicaciones de IoT para escenarios y dispositivos IoT. Las aplicaciones de IoT suelen interactuar con sensores, pantallas y dispositivos de entrada que requieren el uso de pines de E/S de uso general (GPIO), puertos serie o hardware similar. Por ejemplo, puede encontrar bibliotecas que funcionan con paneles populares, como Raspberry Pi y Hummingboard.

### Prueba de conocimientos

**1.** Imagine que usó código de C# para crear una aplicación. Después de ejecutar el código, detecta un error en la lógica. ¿Cómo se puede encontrar el error?

* [ ] El compilador de C# le ayudará a encontrar el error en la lógica.
* [ ] El entorno de ejecución de .NET le ayudará a encontrar el error en la lógica.
* [ ] Una clase de la biblioteca de .NET le ayudará a encontrar el error en la lógica.
* [ ] Las características de depuración de Visual Studio o la CLI de .NET pueden ayudarle a encontrar el error en la lógica.

**2.** ¿Cuál de los siguientes términos describe un marco de trabajo de aplicación que combina varias bibliotecas relacionadas, junto con proyectos de inicio, plantillas de archivo, generadores de código y otras herramientas para que los desarrolladores puedan compilar una aplicación con un fin específico?

* [ ] Carga de trabajo
* [ ] Modelo de aplicación
* [ ] Un ensamblado
* [ ] Entorno

**3.** ¿Cuál de los siguientes términos describe mejor el instalador necesario para crear proyectos, escribir código, llamar a métodos en bibliotecas, compilar código y compilar, depurar y ejecutar aplicaciones?

* [ ] Entorno de ejecución de .NET
* [ ] Bibliotecas base de .NET
* [ ] SDK de .NET
* [ ] Ensamblado .NET

### Resumen

El objetivo de este módulo era presentar .NET. En este momento, ha empezado a comprender en qué consiste .NET y las partes principales del ecosistema de .NET. Ha obtenido información sobre el flujo de trabajo que usan los desarrolladores, las herramientas en las que se basan para compilar aplicaciones y los escenarios en los que tiene sentido usar .NET. Ha creado una aplicación "Hola mundo" sencilla para ilustrar el flujo de trabajo y cómo funcionan conjuntamente los componentes de .NET.

#### Recursos

Si quiere usar una interfaz gráfica de usuario para compilar aplicaciones con C#, [descargue e instale Visual Studio 2022](https://visualstudio.microsoft.com/vs/). Como ya ha aprendido anteriormente en el módulo, el proceso de instalación puede tardar unos minutos y requerir mucho ancho de banda de Internet.

 Nota

Si no es un usuario con licencia (de pago) de Visual Studio, descargue la  *edición Community* , que contiene todas las características que necesita para empezar.

Si quiere empezar a usar una interfaz de línea de comandos, descargue e instale el [SDK de .NET](https://dotnet.microsoft.com/download) y [Visual Studio Code](https://code.visualstudio.com/).

Por último, si necesita obtener más información sobre C# antes de continuar, consulte la ruta de aprendizaje [Primeros pasos con C#](https://learn.microsoft.com/es-es/training/paths/get-started-c-sharp-part-1/).

## Creación de un proyecto de .NET y trabajo con dependencias

Use las dependencias del registro de NuGet para desarrollar más rápido aplicaciones de .NET. Obtenga información sobre cómo administrar las dependencias del proyecto.

### Introducción

Cuando trabaja en una aplicación, escribe código para cumplir los requisitos empresariales. Por motivos de velocidad y confiabilidad, usted y el equipo no escribirán todo el código por su cuenta, Recurrirá a código externo, es decir, bibliotecas escritas por otra persona.

Una manera de enfocar la compilación de la aplicación con bibliotecas externas consiste en usar las bibliotecas existentes de las que puede realizar descargas y, posiblemente, pueda ampliar. Mediante el uso de estas bibliotecas, podrá acabar de compilar la aplicación antes y comercializarla mucho antes que la competencia. Otra ventaja de usar bibliotecas puede ser para garantizar que la aplicación siga los procedimientos recomendados para la autenticación y la autorización. Al fin y al cabo, la protección de los datos propios y los de los clientes es un aspecto muy importante.

En este módulo, usará la herramienta de línea de comandos de .NET y el registro de paquetes NuGet para agregar bibliotecas al código de la aplicación. También aprenderá a administrar actualizaciones y mitigar problemas.

### Objetivos de aprendizaje

Después de completar este módulo, podrá:

* Inicializar proyectos de .NET.
* Agregar y eliminar paquetes de un proyecto de .NET.
* Administrar las dependencias de paquete y actualizarlas de forma predecible.

### Requisitos previos

* Instalaciones locales del [SDK de .NET](https://dotnet.microsoft.com/download) y [Visual Studio Code](https://code.visualstudio.com/)
* [Extensión de C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp) para Visual Studio Code
* Experiencia con el uso de la línea de comandos

### Incorporación de paquetes al proyecto de .NET

.NET incluye muchas bibliotecas principales que lo controlan todo, desde la administración de archivos y HTTP hasta la compresión de archivos. Existe un ecosistema enorme de bibliotecas de terceros. Puede usar NuGet, el administrador de paquetes de .NET, para instalar estas bibliotecas y usarlas en la aplicación.

En .NET y en su ecosistema se usa mucho la palabra  *dependencia* . Una dependencia de paquete es una biblioteca de terceros. Se trata de un fragmento de código reutilizable que lleva a cabo una tarea y se puede agregar a la aplicación. La biblioteca de terceros es algo de lo que la aplicación *depende* para funcionar, de ahí la palabra  *dependencia* .

Puede considerar la biblioteca de terceros como un paquete y se almacena en un repositorio. Un paquete consta de una o varias bibliotecas que se pueden agregar a la aplicación para aprovechar sus características.

Nos centraremos en las dependencias de paquetes. Un proyecto de .NET puede tener otros tipos de dependencias, como marcos de trabajo, analizadores, referencias de proyecto y dependencias de proyecto compartidas, junto con dependencias de paquetes.

### Determinación de la necesidad de un paquete

¿Cómo puede saber si necesita un paquete para el proyecto? Esta es una pregunta complicada que implica varios factores:

* **Obtención de código mejor** : Pregúntese si se trata de un área como la seguridad, por ejemplo, y si intenta implementar la autenticación y la autorización. Es muy importante *tenerlo claro* para proteger los datos personales y los de los clientes. Muchos desarrolladores usan los patrones estándar y las bibliotecas que están disponibles. Estas bibliotecas implementan características que probablemente siempre necesitará y los problemas se corrigen a medida que se producen. Debería usar estas bibliotecas en lugar de crear una propia. Probablemente no escriba el código tan bien personalmente, ya que hay muchos casos extremos que debería tener en cuenta.
* **Ahorro de tiempo** : Probablemente pueda compilar por su cuenta la mayoría de los elementos, como bibliotecas de utilidades o de componentes de interfaz de usuario, pero esto lleva tiempo. Aunque el resultado es comparable a lo que ya está disponible, no vale la pena perder tiempo en replicar el trabajo de escribir este código si no tiene que hacerlo.
* **Mantenimiento** : tarde o temprano, debe realizarse un mantenimiento de todas las bibliotecas y aplicaciones. El mantenimiento implica agregar nuevas características y corregir errores. ¿El mantenimiento de una biblioteca es un uso correcto de su tiempo o el de su equipo? ¿O es mejor permitir que un equipo de software de código abierto lo controle?

### Evaluación de un paquete

Antes de instalar una biblioteca, es posible que le interese inspeccionar las dependencias en las que se basa. Estas dependencias pueden animarlo a usar el paquete, o bien podrían disuadirlo de hacerlo. Estos son algunos factores que tener en cuenta al seleccionar una dependencia para el proyecto:

* **Tamaño** : El número de dependencias puede crear una superficie de memoria grande. Si dispone de ancho de banda limitado o tiene otras limitaciones de hardware, este factor puede suponer un problema.
* **Licencias** : Debe asegurarse de que la licencia concedida para la biblioteca cubre el uso previsto, tanto si se trata de un uso comercial, personal o académico.
* **Mantenimiento activo** : Si el paquete se basa en una dependencia que está en desuso o que no se ha actualizado desde hace mucho tiempo, puede ser un problema.

Para obtener más información sobre un paquete antes de instalarlo, vaya a `https://www.nuget.org/packages/<package name>`. Esta dirección URL le llevará a una página con los detalles del paquete. Seleccione la lista desplegable **Dependencias** para ver de qué paquetes depende para funcionar.

Puede que el número de dependencias mostradas no sea del todo ilustrativo. Si descarga un paquete, podría acabar con una dependencia de paquete que contiene docenas de paquetes. ¿A qué se debe? Cada paquete tiene una lista de dependencias. Para asegurarse de poder usar un paquete, todas las dependencias se rastrean y se descargan cuando se ejecuta el comando `dotnet add package <package name>`.

### Instalación de un paquete

Hay varias maneras de instalar paquetes. Visual Studio y Visual Studio para Mac tienen integrada una interfaz de usuario gráfica y una línea de comandos para un administrador de paquetes. Puede agregar manualmente referencias de paquetes al archivo de proyecto o puede instalarlas a través de una herramienta de interfaz de línea de comandos (CLI), como Paket o la CLI de .NET Core.

En este módulo, vamos a usar la CLI de .NET Core integrada para instalar paquetes. Puede agregar un paquete al proyecto de .NET mediante la invocación de un comando en el terminal. Un comando de instalación típico es similar a este: `dotnet add package <name of package>`. Al ejecutar el comando `add package`, la herramienta de línea de comandos se conecta a un registro global, captura el código y lo almacena en una ubicación de carpeta en la memoria caché que puedan usar todos los proyectos.

Después de que el proyecto se instale y se compile, se agregan las referencias a las carpetas Debug o Release. El directorio del proyecto tendrá un aspecto similar a este:

**Bash**

```
-| bin/
---| Debug/
------| net3.1
--------| <files included in the dependency>
```

### Búsqueda de un paquete

Es posible que desarrolladores individuales usen el registro global de NuGet.org para buscar y descargar los paquetes que necesitan para sus aplicaciones. Es posible que una empresa aplique una estrategia para saber qué paquetes se pueden usar y dónde buscarlos.

![Captura de pantalla de NuGet.org en la que se muestra una lista de paquetes populares.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/finding-nuget.png)

Los paquetes se podrían encontrar en muchos lugares diferentes. Algunos de estos orígenes podrían estar disponibles públicamente, mientras que otros tal vez estén restringidos y solo estén disponibles para los empleados de una empresa específica. Estos son algunos lugares donde podrían estar los paquetes:

* **Registros** : Un ejemplo podría ser un registro global, como el de NuGet.org. Puede hospedar registros propios, ya sean privados o públicos. Hay registros privados disponibles a través de servicios como GitHub y Azure DevOps.
* **Archivos** : Puede instalar un paquete desde una carpeta local. La instalación desde un paquete es habitual cuando se intentan desarrollar bibliotecas propias de .NET y se quiere probar el paquete de forma local, o bien cuando no se quiere usar un registro por el motivo que sea.

![Diagrama en el que se ilustra la relación entre los creadores, los hosts y los consumidores de paquetes.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/nuget-roles.png)

### Registro de NuGet y herramienta dotnet

Al ejecutar `dotnet add package <name of dependency>`, .NET va a un registro global, denominado registro de NuGet.org, y busca el código que se va a descargar. Se encuentra en `https://nuget.org`. También puede buscar paquetes en esta página si accede a ella con un explorador. Cada paquete tiene un sitio web dedicado que puede visitar.

![Captura de pantalla de la página de aterrizaje de un paquete NuGet.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/nuget-info.png)

En estos sitios, puede obtener más información sobre dónde reside el código fuente. También puede encontrar información como las métricas de las descargas e información sobre el mantenimiento.

![Captura de pantalla con información y métricas de un paquete NuGet.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/nuget-downloads.png)

### Comandos .NET

Hasta ahora, ha obtenido información sobre cómo puede instalar dependencias con la CLI de .NET Core. Pero esta herramienta puede hacer mucho más.

La CLI de .NET Core tiene bastantes comandos. Los comandos le ayudan con tareas como la instalación o la creación de paquetes, y la inicialización de proyectos de .NET. No es necesario conocer todos los comandos en detalle. Cuando empiece a usar .NET, es probable que emplee solo un subconjunto de los comandos. A medida que aumente el uso de .NET, es posible que cada vez use más comandos de diversas categorías.

Para ayudarle a recordar qué hacen los comandos, puede considerarlos como pertenecientes a categorías:

* **Administración de dependencias** : Los comandos de esta categoría cubren la instalación, eliminación, limpieza después de las instalaciones de paquetes y la actualización de paquetes.
* **Ejecución de programas** : La herramienta de .NET Core puede ayudarle a administrar flujos en el desarrollo de la aplicación. Como ejemplos de flujos de aplicación podrían citarse la ejecución de pruebas, la compilación de código y la ejecución de comandos de migración para actualizar proyectos.
* **Creación y publicación de paquetes** : Hay varios comandos que pueden ayudarle con tareas como la creación de un paquete comprimido y su inserción en un registro.

Si quiere obtener una lista detallada de todos los comandos, escriba `dotnet --help` en el terminal.

### Procedimiento para instalar un paquete

Use el comando `dotnet add package <dependency name>` para instalar una dependencia normal diseñada para usarse como parte de la aplicación.

 Nota

Puede instalar algunos paquetes  *globalmente* . Estos paquetes no están pensados para importarse en el proyecto. Por este motivo, muchos paquetes globales son herramientas de la CLI o plantillas. También puede instalar estas herramientas globales desde un repositorio de paquetes. Instale las herramientas con el comando `dotnet tool install <name of package>`. Instale las plantillas con el comando `dotnet new -i <name of package>`.

### Después de la instalación

Los paquetes instalados se indican en la sección `dependencies` del archivo .csproj. Si quiere ver qué paquetes hay en la carpeta, puede escribir `dotnet list package`.

**Resultados**

```
Project 'DotNetDependencies' has the following package references
   [net5.0]:
   Top-level Package      Requested   Resolved
   > Humanizer            2.7.9       2.7.9
```

Este comando solo muestra los paquetes de nivel superior, no las dependencias de dichos paquetes que denominamos  *transitivos* . Esto es muy útil para una vista rápida. Si desea una vista más detallada, puede enumerar todos los paquetes transitivos. Al hacerlo, el comando `list` tiene el aspecto siguiente:

**CLI de .NET**

```
dotnet list package --include-transitive
```

La inclusión de los transitivos le permitirá ver las dependencias junto con todos los paquetes que haya instalado. Si ejecuta `dotnet list package --include-transitive`, es posible que obtenga este resultado:

**Resultados**

```
Project 'DotNetDependencies' has the following package references
   [net5.0]:
   Top-level Package      Requested   Resolved
   > Humanizer            2.7.9       2.7.9

   Transitive Package               Resolved
   > Humanizer.Core                 2.7.9
   > Humanizer.Core.af              2.7.9
   > Humanizer.Core.ar              2.7.9
   > Humanizer.Core.bg              2.7.9
   > Humanizer.Core.bn-BD           2.7.9
   > Humanizer.Core.cs              2.7.9
   ...
```

### Restauración de dependencias

Al crear o clonar un proyecto, las dependencias incluidas no se descargan ni se instalan hasta que se compila el proyecto. Mediante la ejecución del comando `dotnet restore`, puede restaurar manualmente las dependencias y las herramientas específicas del proyecto que se especifican en el archivo de proyecto. En la mayoría de los casos, no es necesario usar explícitamente el comando. La restauración de NuGet se ejecuta implícitamente, si es necesario, cuando se ejecutan comandos como `new`, `build` y `run`.

### Limpieza de las dependencias

Tarde o temprano, es probable que se dé cuenta de que ya no necesita un paquete, o es posible que se dé cuenta de que el paquete que instaló no es el que necesita. Puede que haya encontrado uno que realizará mejor una tarea. Sea cual sea el motivo, debe quitar las dependencias que no use. Al hacerlo, todo se mantiene limpio. Además, las dependencias ocupan espacio.

Para quitar un paquete del proyecto, use el comando `remove` de la siguiente manera: `dotnet remove package <name of dependency>`. Este comando quitará el paquete del archivo .csproj del proyecto.

### Ejercicio: Instalación de paquetes

Los desarrolladores de Tailwind Traders asumen que están a punto de invertir una gran cantidad de recursos en el desarrollo de aplicaciones para la plataforma .NET. Estas aplicaciones mostrarán muchos datos legibles para los usuarios, como fechas, horas y números.

.NET tiene funciones para hacerlo, pero los desarrolladores están seguros de que alguien ya habrá resuelto este problema. Necesitan un marco. Tras realizar una búsqueda, han encontrado Humanizer en el registro de paquetes NuGet. Por lo que ven, se usa ampliamente y promete cumplir todas sus necesidades relacionadas con .NET, como manipular y mostrar cadenas, enumeraciones, fechas, horas, intervalos, números y cantidades.

En este punto, los desarrolladores desean que instale Humanizer, que escriba un par de manipulaciones de datos y que las ejecute para ver si Humanizer cumple las expectativas.

 Nota

En este módulo se usan la CLI (interfaz de la línea de comandos) de .NET y Visual Studio Code para el desarrollo local. Cuando complete este módulo, podrá aplicar los conceptos mediante Visual Studio (Windows), Visual Studio para Mac (macOS), o seguir con el desarrollo mediante Visual Studio Code (Windows, Linux y macOS).

En este módulo se usa el SDK de .NET 6.0. Asegúrese de que tiene instalado .NET 6.0 mediante la ejecución del siguiente comando en el terminal que prefiera:

**CLI de .NET**

```
dotnet --list-sdks
```

Verá un resultado similar al siguiente:

**Consola**

```
3.1.100 [C:\program files\dotnet\sdk]
5.0.100 [C:\program files\dotnet\sdk]
6.0.100 [C:\program files\dotnet\sdk]
```

Asegúrese de que aparece una versión que comienza por `6`. Si no aparece ninguna o no se encuentra el comando, [instale el SDK más reciente de .NET 6.0](https://dotnet.microsoft.com/download).

#### Creación de un proyecto de .NET de ejemplo

Para configurar un proyecto de .NET para que funcione con dependencias, usaremos Visual Studio Code. Visual Studio Code incluye un terminal integrado que facilita la creación de un proyecto. Si no quiere usar otro editor de código, puede ejecutar los comandos de este módulo en un terminal.

1. En Visual Studio Code, seleccione  **Archivo** > **Abrir carpeta** .
2. Cree una carpeta denominada **DotNetDependencies** en la ubicación que prefiera y, después, seleccione  **Seleccionar carpeta** .
3. Abra el terminal integrado desde Visual Studio Code; para ello, seleccione  **Ver** >**Terminal** en el menú principal.
4. En la ventana del terminal, copie y pegue el siguiente comando.
   **CLI de .NET**

   ```
   dotnet new console -f net6.0
   ```

   Este comando crea un archivo **Program.cs** en la carpeta con un programa "Hola mundo" básico que ya está escrito, junto con un archivo de proyecto de C# denominado  **DotNetDependencies.csproj** .

   Ahora debería tener acceso a estos archivos.

   **Bash**

   ```
   -| obj
   -| DotNetDependencies.csproj
   -| Program.cs
   ```
5. En la ventana del terminal, copie y pegue el siguiente comando para ejecutar el programa "Hola mundo".
   **CLI de .NET**

   ```
   dotnet run
   ```

En la ventana del terminal se muestra "Hola mundo" como salida.

![Captura de pantalla de Visual Studio Code con una nueva aplicación de consola.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/new-dotnet-project.png)

#### Configuración de Visual Studio Code para la depuración de .NET

Abra Program.cs. La primera vez que abra un archivo de C# en Visual Studio Code, recibirá un aviso para instalar las extensiones recomendadas para C#. Seleccione el botón **Instalar** en el mensaje.

![Captura de pantalla del mensaje de extensiones recomendadas de Visual Studio Code.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/install-recommended-extensions.png)

Visual Studio Code instala la extensión de C#. Muestra un aviso adicional para agregar los recursos necesarios para compilar y depurar el proyecto. Seleccione  **Sí** .

![Captura de pantalla del mensaje de recursos necesarios de Visual Studio Code.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/install-required-assets.png)

Puede cerrar la pestaña **Extensión: C#** para centrarse en el código que va a escribir.

#### Adición de un paquete NuGet mediante la herramienta de .NET Core

1. Abra  **Program.cs** . Debería ser parecido a este:
   **C#**

   ```
   Console.WriteLine("Hello, World!");
   ```

   La función anterior se ejecuta al principio de la aplicación y genera una cadena en la consola. Vamos a agregar Humanizer y a manipular los datos y escribirlos en la consola.
2. Ejecute el siguiente comando para instalar la biblioteca de Humanizer:
   **CLI de .NET**

   ```
   dotnet add package Humanizer --version 2.7.9
   ```

   Abra el archivo **DotNetDependencies.csproj** y busque la sección `ItemGroup`. Ahora debería tener una entrada similar a la siguiente:

   **XML**

   ```
   <ItemGroup>
       <PackageReference Include="Humanizer" Version="2.7.9" />
   </ItemGroup>
   ```
3. Agregue el siguiente contenido en la parte superior del archivo Program.cs para inicializar Humanizer:
   **C#**

   ```
   using Humanizer;
   ```

   El archivo **Program.cs** ahora debería ser similar al siguiente:

   **C#**

   ```
   using Humanizer;

   Console.WriteLine("Hello, World!");
   ```
4. Agregue el contenido siguiente al archivo Program.cs en la parte inferior del archivo, debajo de `Console.WriteLine("Hello, World!");`:
   **C#**

   ```
   static void HumanizeQuantities()
   {
       Console.WriteLine("case".ToQuantity(0));
       Console.WriteLine("case".ToQuantity(1));
       Console.WriteLine("case".ToQuantity(5));
   }

   static void HumanizeDates()
   {
       Console.WriteLine(DateTime.UtcNow.AddHours(-24).Humanize());
       Console.WriteLine(DateTime.UtcNow.AddHours(-2).Humanize());
       Console.WriteLine(TimeSpan.FromDays(1).Humanize());
       Console.WriteLine(TimeSpan.FromDays(16).Humanize());
   }
   ```
5. Reemplace `Console.WriteLine("Hello, World!");` por el código siguiente:
   **C#**

   ```
   Console.WriteLine("Quantities:");
   HumanizeQuantities();

   Console.WriteLine("\nDate/Time Manipulation:");
   HumanizeDates();
   ```
6. Guarde el archivo ( **Archivo** >**Guardar** o CTRL + S). Escriba el siguiente comando en el terminal para ejecutar la aplicación:
   **CLI de .NET**

   ```
   dotnet run
   ```

   Debería obtener la siguiente salida:

   **Resultados**

   ```
   Quantities:
   0 cases
   1 case
   5 cases

   Date/Time Manipulation:
   yesterday
   2 hours ago
   1 day
   2 weeks
   ```

¡Enhorabuena! Ha instalado correctamente Humanizer como una dependencia y ha escrito lógica para el código de la aplicación con el objetivo de que los datos sean más legibles. Parece que Humanizer está a la altura de las expectativas y que probablemente en Tailwind Traders estarán satisfechos con el resultado de esta evaluación.

### Administración de actualizaciones de dependencias en el proyecto de .NET

Tarde o temprano, querrá actualizar a una nueva versión de una biblioteca. Tal vez una función se haya marcado como en desuso o puede que haya una nueva característica en una versión posterior de un paquete que está usando.

Tenga en cuenta estas consideraciones antes de intentar actualizar una biblioteca:

* **El tipo de actualización** : ¿qué tipo de actualización está disponible? ¿Se trata de una pequeña corrección de errores? ¿Agrega una característica nueva que necesita? ¿Interrumpirá el código? Puede comunicar el tipo de actualización mediante un sistema denominado  *versionamiento semántico* . La manera en que se expresa el número de versión de la biblioteca indica al desarrollador el tipo de actualización con el que trata.
* **Si el proyecto está configurado correctamente** : el proyecto de .NET se puede configurar de forma que solo obtenga los tipos de actualizaciones que le interesen. Solo se realizará una actualización si hay disponible un tipo de actualización específico. Este es el enfoque recomendado para evitar sorpresas.
* **Problemas de seguridad** : la administración de las dependencias del proyecto a lo largo del tiempo conlleva tener en cuenta los problemas que puedan producirse. Por ejemplo, pueden surgir problemas cuando se detectan vulnerabilidades. Si todo va bien, se publicarán revisiones que se pueden descargar. La herramienta de .NET Core ayuda a ejecutar una *auditoría* en las bibliotecas para averiguar si tiene paquetes que se deban actualizar. También le ayuda a realizar las acciones adecuadas para solucionar un problema.

#### Uso del versionamiento semántico

Existe un estándar del sector denominado  *versionamiento semántico* . El versionamiento semántico es la forma de expresar el tipo de cambio que usted u otro desarrollador introducen en una biblioteca. El versionamiento semántico garantiza que un paquete tenga un número de versión dividido en estas secciones:

* **Versión principal** : número situado más a la izquierda. Por ejemplo, es el 1 en 1.0.0. Un cambio en este número significa que puede esperar cambios importantes en el código. Es posible que tenga que volver a escribir parte del código.
* **Versión secundaria** : número del medio. Por ejemplo, es el 2 en 1.2.0. Un cambio en este número significa que se han agregado características. El código debería seguir funcionando. Por lo general, es seguro aceptar la actualización.
* **Versión de revisión** : número más a la derecha. Por ejemplo, es el 3 en 1.2.3. Un cambio en este número significa que se ha aplicado un cambio que corrige una parte del código que debería haber funcionado. Debería ser seguro aceptar la actualización.

En esta tabla se muestra cómo cambia el número de versión de cada tipo de versión:

| Tipo                  | ¿Qué sucede?       |
| --------------------- | -------------------- |
| Versión principal    | 1.0.0 cambia a 2.0.0 |
| Versión secundaria   | 1.1.1 cambia a 1.2.0 |
| Versión de revisión | 1.0.1 cambia a 1.0.2 |

Muchas empresas y desarrolladores han adoptado este sistema. Si tiene previsto publicar paquetes e insertarlos en el registro de NuGet, se espera que siga el versionamiento semántico. Incluso si solo descarga paquetes del registro de NuGet, lo más probable es que sigan el versionamiento semántico.

Los cambios en un paquete pueden presentar riesgos, como el hecho de que un error pueda perjudicar su negocio. Algunos riesgos podrían requerir que vuelva a escribir parte del código. La reescritura de código lleva tiempo y cuesta dinero.

#### Enfoque de actualización

Como desarrollador de .NET, puede comunicar a .NET el comportamiento de actualización de su preferencia. Piense en la actualización en términos del riesgo. Estos son algunos enfoques:

* **Versión principal** : estoy de acuerdo con la actualización a la versión principal más reciente en cuanto se publique. Acepto el hecho de que es posible que tenga que cambiar el código.
* **Versión secundaria** : me parece bien que se incorpore una característica nueva. No me gusta que el código se interrumpa.
* **Versión de revisión** : las únicas actualizaciones que me interesan son las correcciones de errores.

Si va a administrar un proyecto de .NET nuevo o más pequeño, puede permitirse cierta flexibilidad en el modo de definir la estrategia de actualización. Por ejemplo, siempre puede actualizar a la última versión. En el caso de proyectos más complejos, existen más matices, pero se describirán en un módulo futuro.

Por lo general, cuanto menor sea la dependencia que se va a actualizar, menos dependencias tendrá y más probabilidades de que el proceso de actualización sea fácil.

#### Configuración del archivo de proyecto para la actualización

Al agregar una o varias dependencias, piense en configurar el archivo del proyecto de modo que obtenga un comportamiento predecible al restaurar, compilar o ejecutar el proyecto. Puede comunicar el enfoque que quiere adoptar para un paquete. NuGet tiene los conceptos de intervalos de versiones y versiones flotantes.

Veamos primero los intervalos de versiones. Se trata de una notación especial que se usa para especificar intervalos de versiones concretos que quiere que se resuelvan.

| Notación | Regla aplicada  | Descripción                                                    |
| --------- | --------------- | --------------------------------------------------------------- |
| 1.0       | x >= 1.0        | Versión mínima, incluida                                      |
| (1.0,)    | x > 1.0         | Versión mínima, excluida                                      |
| [1.0]     | x == 1.0        | Coincidencia de versión exacta                                 |
| (,1.0]    | x ≤ 1.0        | Versión máxima, incluida                                      |
| (,1.0)    | x < 1.0         | Versión máxima, excluida                                      |
| [1.0,2.0] | 1.0 ≤ x ≤ 2.0 | Intervalo exacto, ambos incluidos                               |
| (1.0,2.0) | 1.0 < x < 2.0   | Intervalo exacto, ambos excluidos                               |
| [1.0,2.0) | 1.0 ≤ x < 2.0  | Versión mínima incluida y versión máxima excluida mezcladas |
| (1.0)     | no válido      | no válido                                                      |

NuGet también admite el uso de una notación de versión flotante para las partes de sufijo de versión principal, secundaria, de revisión y versión preliminar del número. Esta notación es un asterisco (*). Por ejemplo, la especificación de la versión 6.0.* indica "use la versión 6.0.x más reciente". En otro ejemplo, 4.* significa "use la versión 4.x más reciente". El uso de una versión flotante reduce los cambios en el archivo del proyecto, a la vez que se mantiene al día con la última versión de una dependencia.

 Nota

Se recomienda instalar una versión específica, en lugar de usar cualquiera de las notaciones flotantes. Instalar una versión específica garantiza que las compilaciones se puedan repetir, a menos que se solicite explícitamente una actualización de una dependencia.

Cuando se usa una versión flotante, NuGet resuelve la última versión de un paquete que coincide con el patrón de versión. En el ejemplo siguiente, 6.0.* obtiene la última versión de un paquete que empieza por 6.0. Esa versión es 6.0.1.

![Captura de pantalla de la elección de la última versión cuando se solicita una versión flotante.](https://learn.microsoft.com/es-es/training/modules/dotnet-dependencies/media/floating-version.png)

Estos son algunos ejemplos que se pueden configurar para la versión principal, secundaria o de revisión:

**XML**

```
<!-- Accepts any version 6.1 and later. -->
<PackageReference Include="ExamplePackage" Version="6.1" />

<!-- Accepts any 6.x.y version. -->
<PackageReference Include="ExamplePackage" Version="6.*" />
<PackageReference Include="ExamplePackage" Version="[6,7)" />

<!-- Accepts any later version, but not including 4.1.3. Could be
     used to guarantee a dependency with a specific bug fix. -->
<PackageReference Include="ExamplePackage" Version="(4.1.3,)" />

<!-- Accepts any version earlier than 5.x, which might be used to prevent pulling in a later
     version of a dependency that changed its interface. However, we don't recommend this form because determining the earliest version can be difficult. -->
<PackageReference Include="ExamplePackage" Version="(,5.0)" />

<!-- Accepts any 1.x or 2.x version, but not 0.x or 3.x and later. -->
<PackageReference Include="ExamplePackage" Version="[1,3)" />

<!-- Accepts 1.3.2 up to 1.4.x, but not 1.5 and later. -->
<PackageReference Include="ExamplePackage" Version="[1.3.2,1.5)" />
```

#### Búsqueda y actualización de paquetes obsoletos

El comando `dotnet list package --outdated` muestra los paquetes obsoletos. Este comando puede ayudarle a aprender cuándo hay disponibles versiones más recientes de los paquetes. Esta es una salida típica del comando:

**Resultados**

```
Top-level Package      Requested   Resolved   Latest
> Humanizer            2.7.*       2.7.9      2.8.26
```

Estos son los significados de los nombres de las columnas en la salida:

* `Requested`: versión o intervalo de versiones que ha especificado.
* `Resolved`: versión real que se ha descargado para el proyecto que coincide con la versión especificada.
* `Latest`: versión más reciente disponible para la actualización desde NuGet.

El flujo de trabajo recomendado es ejecutar los siguientes comandos, en este orden:

1. Ejecute `dotnet list package --outdated`. Este comando enumera todos los paquetes obsoletos. Proporciona información en las columnas `Requested`, `Resolved` y `Latest`.
2. Ejecute `dotnet add package <package name>`. Si ejecuta este comando, se intentará actualizar a la última versión. Opcionalmente, puede pasar `--version=<version number/range>`.

### Ejercicio: Administración de actualizaciones de dependencias en el proyecto de .NET

Las dependencias que se usan en las aplicaciones se pueden actualizar con frecuencia y pueden contener nuevas características, correcciones de errores y actualizaciones de seguridad críticas. La aplicación que ha creado es pequeña y solo tiene una dependencia. Debería ser fácil actualizarla. Vea si puede actualizar la aplicación para aprovechar las características más recientes.

#### Actualización de las dependencias de la aplicación

1. En el archivo  **DotNetDependencies.csproj** , observe `dependencies`. Debería ser similar a este código:
   **XML**

   ```
   <ItemGroup>
       <PackageReference Include="Humanizer" Version="2.7.9" />
   </ItemGroup>
   ```
2. Para ver las dependencias instaladas, ejecute este comando:
   **CLI de .NET**

   ```
   dotnet list package
   ```

   Esto debería generar la versión solicitada y la versión final resuelta (es decir, instalada).

   **Resultados**

   ```
   Top-level Package      Requested   Resolved
   > Humanizer            2.7.9        2.7.9
   ```
3. Para ver qué dependencias están obsoletas, ejecute este comando:
   **CLI de .NET**

   ```
   dotnet list package --outdated
   ```

   La salida debería ser similar a la siguiente. Es posible que obtenga otros valores en la columna `Latest`.

   **Resultados**

   ```
   Project `DotNetDependencies` has the following updates to its packages
      [net6.0]:
      Top-level Package      Requested   Resolved   Latest
      > Humanizer            2.7.9       2.7.9      2.11.10
   ```

   De forma predeterminada, este comando buscará la última versión estable. Para buscar paquetes de versión preliminar, anexe `--include-prerelease` al comando anterior:
   **CLI de .NET**

   ```
   dotnet list package --outdated --include-prerelease
   ```
4. Puede actualizar a la versión `Latest`, con cierto nivel de confianza. De este modo, se asegurará de que las dependencias obtengan las características y revisiones más recientes de esa versión principal. Para instalar la versión más reciente, ejecute el siguiente comando:
   **CLI de .NET**

   ```
   dotnet add package Humanizer 
   ```

   Debería obtener una salida similar a la siguiente:

   **Resultados**

   ```
   info : PackageReference for package 'Humanizer' version '2.11.10' updated in file 'C:\Users\username\Desktop\DotNetDependencies\DotNetDependencies.csproj'.
   ```

   En la salida se indica que las dependencias del proyecto se han actualizado.
   Si quiere actualizar a una versión específica de la dependencia, puede anexar el parámetro `--version` e indicar la versión concreta.
   **CLI de .NET**

   ```
   dotnet add package Humanizer --version 2.11.10
   ```

   Por último, también puede instalar el paquete de versión preliminar más reciente. Para ello, anexe el parámetro `--prerelease`.
   **CLI de .NET**

   ```
   dotnet add package Humanizer --prerelease
   ```

   Es posible que los resultados sean ligeramente distintos. La versión indicada debe corresponderse con la última versión disponible del paquete.

¡Enhorabuena! Ha actualizado la dependencia de la aplicación. Buen trabajo.

### Prueba de conocimientos

Elija la mejor respuesta para cada pregunta y, después, seleccione  **Comprobar las respuestas** .

#### Comprobación de conocimientos

**1.** ¿Cómo se instala un marco como Humanizer?

* [ ] Ejecute `dotnet add Humanizer`:
* [ ] Ejecute `dotnet add package Humanizer`:
* [ ] Mediante la ejecución de `dotnet install Humanizer`.
* [ ] Mediante la ejecución de `dotnet download package Humanizer`.

**2.** ¿Qué cambio de versión indicaría una versión secundaria cuando un paquete usa la versión semántica?

* [ ] 1.1.1 cambia a 1.2.0
* [ ] 1.0.1 cambia a 1.0.2
* [ ] 1.0.0 cambia a 2.0.0

**3.** ¿Cómo se configura un archivo de proyecto para que solo obtenga actualizaciones de revisión (corrección de errores)?

* [ ] Se busca la entrada en el archivo de proyecto y se establece la entrada de modo que tenga el aspecto siguiente: `<PackageReference Include="<package>" Version="*"/>`.
* [ ] Se busca la entrada en el archivo de proyecto y se establece la entrada de modo que tenga el aspecto siguiente: `<PackageReference Include="<package>" Version="2.*"/>`.
* [ ] Se busca la entrada en el archivo de proyecto y se establece la entrada de modo que tenga el aspecto siguiente: `<PackageReference Include="<package>" Version="2.7.*"/>`.
* [ ] Se busca la entrada en el archivo de proyecto y se establece la entrada de modo que tenga el aspecto siguiente: `<PackageReference Include="<package>" Version="[6,7)"/>`.

**4.** ¿Cómo se comprueba si hay disponible una nueva versión de un marco?

* [ ] Ejecute `dotnet list outdated`:
* [ ] Ejecute `dotnet list package outdated`:
* [ ] Ejecute `dotnet list --outdated`:
* [ ] Ejecute `dotnet list package --outdated`:

### Resumen

En primer lugar, ha aprendido a instalar dependencias que la aplicación puede usar. El uso de dependencias en la aplicación le permite crear la aplicación más rápido porque el código ya está escrito. Además, es recomendable recurrir a bibliotecas probadas en lugar de escribir algo propio. El uso de estas bibliotecas es especialmente recomendable cuando se agrega autenticación y autorización a la aplicación.

En este módulo se ha explicado cómo usar la CLI de .NET Core para instalar dependencias de manera local.

Después, ha aprendido a actualizar las dependencias. Las dependencias se actualizan por varias razones en forma de correcciones de errores, características nuevas o cambios más grandes. En el archivo de proyecto, puede configurar los tipos de actualizaciones que le interesan por cada dependencia. Si trabaja en un entorno empresarial, se recomienda considerar cuidadosamente el enfoque relacionado con los tipos de actualizaciones que acepta.

#### Recursos adicionales

* Revise la [documentación de NuGet](https://learn.microsoft.com/es-es/nuget/) oficial.
* Revise la [documentación oficial de la CLI de .NET](https://learn.microsoft.com/es-es/dotnet/core/tools/).
* Examine los paquetes disponibles en [NuGet](https://www.nuget.org/).
* Consulte el [sitio web de .NET](https://dot.net/) para informarse sobre todo lo relacionado con .NET.
* Pruebe [Visual Studio Code](https://code.visualstudio.com/) para editar texto y archivos de código.
