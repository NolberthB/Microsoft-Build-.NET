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
