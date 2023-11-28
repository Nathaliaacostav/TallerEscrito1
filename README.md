# TallerEscrito1

Taller de nivelación
Nathalia Acosta Vélez
 
1.	¿Qué es la lógica en el contexto de la programación? Y explicar por qué es importante en el Desarrollo Web Frontend.

R/ La lógica en la programación Frontend se refiere a cómo organizamos las instrucciones para que las páginas web respondan a las acciones de los usuarios. Es como decirle a la computadora qué hacer y cuándo hacerlo. En el desarrollo web, la lógica es crucial porque nos permite hacer que las páginas sean interactivas. Manejamos cosas como hacer clic en botones, validar información en formularios y cambiar lo que se muestra en la pantalla. También utilizamos la lógica para controlar cómo fluye el programa y para gestionar el estado de la aplicación. En resumen, la lógica es como las reglas que le damos a la computadora para que nuestra página web funcione de la manera que queremos, permitiendo una experiencia de usuario suave y atractiva.

 
2.	Definir el concepto de “algoritmo” y proporcionar un ejemplo sencillo de un algoritmo relacionado con la lógica de programación.

R/ Un algoritmo es un conjunto de pasos bien definidos y ordenados que llevan a cabo una tarea específica o resuelven un problema. Es una secuencia lógica de instrucciones diseñada para realizar una tarea de manera efectiva.
Ejemplo sencillo de un algoritmo relacionado con la lógica de programación:
Problema: Sumar dos números.
Algoritmo:
Inicio: Inicia el algoritmo.
Ingresar números: Pide al usuario que ingrese dos números.
Sumar: Suma los dos números ingresados.
Mostrar resultado: Muestra el resultado de la suma.
Fin: Finaliza el algoritmo.
Este algoritmo es simple pero ilustra los pasos necesarios para realizar una tarea específica: la suma de dos números. En un lenguaje de programación, este algoritmo podría ser implementado en código para que una computadora lo ejecute y proporcione el resultado de la suma.


 
3.	¿Qué son estructuras de control en la programación?, ¿Cuáles son los tipos de estructuras de control y las estructuras más comunes de cada tipo? Describir al menos dos tipos de estructura de control, explicar por qué son importantes y proporcionar ejemplos de cada uno de cómo se utilizan en el desarrollo web Frontend.

R/ 
Estructuras de Control en Programación:

Las estructuras de control dirigen el flujo de ejecución de un programa. Dos tipos clave son:

1. Estructuras Condicionales:

if-else: Ejecuta código si se cumple una condición.
switch: Selecciona bloques de código basándose en el valor de una expresión.
Ejemplo en desarrollo web:

let edad = 18;

if (edad >= 18) {
   console.log("Mayor de edad");
} else {
   console.log("Menor de edad");
}

2. Bucles:

for: Repite un bloque de código un número definido de veces.
while: Ejecuta código mientras se cumple una condición.
Ejemplo en desarrollo web:

// Imprimir números del 1 al 5 con un bucle for
for (let i = 1; i <= 5; i++) {
   console.log(i);
}

Importancia:

Eficiencia: Optimizan el código y evitan repetición.
Interactividad: Cruciales para manejar eventos del usuario en aplicaciones web.

4. Describir cómo se declaraban variables y constantes en JavaScript antes de la introducción de ECMAScript 6 (ES6). Explicar cómo ES6 mejoró la declaración de variables y constantes, y mencionar los problemas que esta mejora resuelve en el desarrollo web Frontend.

Antes de ECMAScript 6 (ES5):

Antes de ES6, las variables se declaraban utilizando la palabra clave var, y las constantes no tenían una declaración específica. Por ejemplo:

var edad = 25;

Con ECMAScript 6 (ES6):

Con la introducción de ES6, se agregaron nuevas formas de declarar variables y constantes:

Variables con let y const:

let edad = 25; // Variable
const PI = 3.14159; // Constante

let se usa para variables que pueden ser reasignadas.
const se utiliza para declarar constantes, cuyo valor no puede cambiar una vez asignado.
Block Scope:
ES6 introdujo el ámbito de bloque con let y const, lo que significa que la variable o constante solo está disponible dentro del bloque en el que se declara.

Mejoras y Problemas Resueltos:

Bloqueo de Ámbito (Block Scope):

Mejora: Evita problemas de fugas de variables al limitar su alcance al bloque en el que se declaran.
Problema Resuelto: Ayuda a evitar confusiones y errores relacionados con el ámbito de las variables.
const para Constantes:

Mejora: Proporciona una forma clara de declarar constantes, antes era común usar mayúsculas con var para indicar que una variable no debería cambiarse.
Problema Resuelto: Mejora la legibilidad y mantenimiento del código.
let para Variables:

Mejora: Introduce una forma más predecible de declarar variables, evitando problemas relacionados con la elevación (hoisting) de var.
Problema Resuelto: Facilita la comprensión del código y reduce errores.
En el desarrollo web frontend, estas mejoras ayudan a escribir código más claro, predecible y menos propenso a errores, mejorando la mantenibilidad y la calidad del software. Además, el bloqueo de ámbito con let y const es especialmente útil en entornos donde se trabaja con múltiples archivos y módulos, proporcionando un mejor control sobre la visibilidad de las variables.


 
5. ¿Cómo se declaran las funciones en JavaScript y cuál es la diferencia entre una declaración de función, una expresión de función y una función de flecha (arrow function)? Proporcionar ejemplos de cada una.

Declaración de Función:
En JavaScript, la declaración de una función sigue la sintaxis tradicional:

javascript
Copy code
function suma(a, b) {
  return a + b;
}

// Uso de la función
let resultado = suma(3, 5);
console.log(resultado); // Resultado: 8
Expresión de Función:
Las expresiones de función se asignan a variables y pueden ser anónimas o nombradas:

javascript
Copy code
let resta = function(a, b) {
  return a - b;
};

// Uso de la función
let resultadoResta = resta(8, 3);
console.log(resultadoResta); // Resultado: 5
Función de Flecha (Arrow Function):
Las funciones de flecha, introducidas en ES6, ofrecen una sintaxis más concisa:

javascript
Copy code
let multiplicacion = (a, b) => a * b;

// Uso de la función
let resultadoMultiplicacion = multiplicacion(4, 6);
console.log(resultadoMultiplicacion); // Resultado: 24
Diferencias Clave:

Sintaxis:

Declaración de función: function nombreFuncion() {}
Expresión de función: let variable = function() {}
Función de flecha: (param1, param2) => expresion
Contexto de this:

Las funciones de flecha heredan el this del contexto en el que se encuentran, a diferencia de las funciones normales (function).
Brevedad:

Las funciones de flecha son más cortas y proporcionan una sintaxis más concisa.
Ejemplos:

javascript
Copy code
// Declaración de función
function cuadrado(x) {
  return x * x;
}

// Expresión de función
let cubo = function(x) {
  return x ** 3;
};

// Función de flecha
let doble = (x) => x * 2;

console.log(cuadrado(4)); // Resultado: 16
console.log(cubo(3)); // Resultado: 27
console.log(doble(5)); // Resultado: 10
 
6. ¿Por qué es necesario el uso de funciones en el desarrollo web Frontend? Enumerar al menos tres razones fundamentales y proporcionar ejemplos de situaciones en las que las funciones son esenciales. Además, mencionar la ventaja de las funciones flecha en el contexto de estas razones.

Reutilización de Código:
Razón: Las funciones permiten encapsular piezas de código para ser reutilizadas en diferentes partes de una aplicación.
Ejemplo: Una función que valida formularios puede ser utilizada en varias páginas del sitio web.
Organización y Mantenimiento del Código:

Razón: Las funciones ayudan a organizar el código, dividiéndolo en bloques lógicos y facilitando su mantenimiento.
Ejemplo: Una función que maneja la creación y actualización de elementos del DOM mejora la legibilidad y mantenibilidad del código.
Manejo de Eventos y Asincronía:

Razón: Las funciones son esenciales para manejar eventos del usuario y realizar operaciones asíncronas, como llamadas a APIs o manipulación de datos en segundo plano.
Ejemplo: Una función que responde a clics de botones para cargar datos adicionales en una página.
Ventajas de las Funciones Flecha:

Sintaxis Concisa:

Ventaja: Las funciones flecha proporcionan una sintaxis más breve y limpia, especialmente útil para funciones pequeñas.
Ejemplo:
javascript
Copy code
// Función normal
function suma(a, b) {
  return a + b;
}

// Función flecha
let sumaFlecha = (a, b) => a + b;
this Lexical:

Ventaja: Las funciones flecha no tienen su propio this, tomando prestado el this del contexto en el que están definidas. Evita problemas comunes con this en funciones tradicionales.
Ejemplo:
javascript
Copy code
function Persona() {
  this.edad = 0;

  // Función normal
  setInterval(function crecer() {
    this.edad++;
    console.log(this.edad); // 'this' no es la instancia de Persona
  }, 1000);

  // Función flecha
  setInterval(() => {
    this.edad++;
    console.log(this.edad); // 'this' es la instancia de Persona
  }, 1000);
}

let persona = new Persona();
En resumen, las funciones son fundamentales en el desarrollo web frontend para la reutilización del código, la organización del mismo y el manejo de eventos asíncronos. Las funciones flecha, con su sintaxis concisa y manejo de this lexical, ofrecen ventajas adicionales en términos de legibilidad y evitan problemas asociados con las funciones tradicionales.


 
7. ¿Cuál es la diferencia entre parámetro y argumento?

8. Definir el concepto deCallback y proporcionar un ejemplopráctico.


9. ¿Qué es el hoisting en JavaScript y cómo afecta a las variables y funciones? Proporcionar ejemplos de hoisting en declaraciones de variables y funciones.
10. Definir brevemente el concepto de objeto en JavaScript y cuál es la visión genera sobre este concepto. Indicar, también cómo se declaran estas estructuras de datos.

11. ¿Qué son propiedades?, y¿Cuál es la diferencia entre una propiedad y un método en un objeto?

12. Explicar las dos formas de acceder a una propiedad de objetos e indicar las situaciones en que conviene usar una manera sobre la otra.

13. ¿Existe alguna forma de recorrer las propiedades de un objeto?En caso negativo, explicar por qué no es posible y en caso positivo proporcionar un ejemplo.Mencionar una situación en la cual sea muy útil recorrer las propiedades de un objeto.

14. ¿Por qué son útiles los objetos en la programación web y qué tipos de datos pueden almacenar?

15. ¿Qué es un array en JavaScript y por qué son esenciales?

16. ¿Cómo acceder a un elemento dentro de un array? Explicar con un ejemplo.

17. Mencionar al menos tres funciones de arrays y describir su utilidad en la programación web.

18. Proporcionar un ejemplo de cómo se utiliza una función de array para transformar y filtrar datos en un array.

Preguntas prácticas
1. Escribir un programa con JavaScript que resuelva el siguiente problema: Dada una lista (o array) de números enteros, encontrar el número más grandede la lista y mostrarlo en consola. No se debe usar la función Math.max(), ni .forEach().

2. Escribir una función en JavaScript que tome dos númeroscomo argumentosy devuelva su suma. Luego, escribir la misma función utilizando una función flecha (arrow function) y comparar ambas declaraciones. Llamar a ambas funciones con valores de ejemplo y mostrar los resultados en la consola del navegador.

3. Escribir una función en JavaScript que reciba un array de números como argumento y utilizarla función de array para calcular la suma de todos los números pares en el array.Luego, llamar a la función con un array de ejemplo y mostrar el resultado en la consola del navegador.






MÓDULO SOBRE HTML, CSS Y RESPONSIVE DESIGN
Preguntas teóricas
1. ¿Quésignifica HTML y cuál es su función en el desarrollo web?
2. ¿Cuál es la estructura básica de un documento HTML? Describir las etiquetas esenciales.
3. ¿Qué es CSS y cuál es su propósito en el desarrollo web?
4. ¿Qué son selectores CSS, cuáles son los principales tipos de selectores y porqué es importante entender la especificidad en el contexto de las hojas de estilo en cascada (CSS)?Describir al menos tres tipos de selectores CSS y cómo la especificidad afecta a la aplicación de estilos en un proyecto de desarrollo web Frontend. Proporcionar ejemplos de situaciones en las que se utiliza la especificidad de selectores para resolver conflictos de estilos.
5. Explicar las diferencias entre los estilos en línea (inline), estilos internos (embedded) y estilos externos (external) en CSS. Indicar cuál de los tres estiloses el recomendado usar y por qué.
6. ¿Qué es flexbox y cómo se utiliza para el diseño de páginas web?
7. Explicar cómo se empleanlas propiedades flexbox y explicar la función de las principales propiedades en la creación de diseños flexibles.
8. ¿Qué es CSS Grid Layout y en qué se diferencia de flexbox?
9. Proporcionar un ejemplo de cómo crear una cuadrícula sencilla con CSS Grid.
10. ¿Qué significa el diseño responsivo en el contexto del desarrollo web?
11. Enumerar al menos tres técnicas o estrategias utilizadas para lograr el diseño responsivo en una página web.

Preguntas prácticas
1. Crear un documentoHTML llamado index.html que incluya encabezados, párrafos, enlaces y una lista no ordenada. Aplicarla práctica recomendada deestilo CSS para cambiar el color y la fuente de los elementos.
2. Diseñar una sección de la páginaweb en index.html que contenga tres elementos (por ejemplo, tarjetas). Utilizar flexbox para alinearlos horizontalmente y distribuir el espacio de manera uniforme.
3. Crear una cuadrícula de imágenes(o galería de imágenes)utilizando CSS Grid. Asegurarse de que las imágenes se ajusten automáticamente a diferentes tamaños de pantalla.
4. Modificar la página web para que sea responsiva. Asegurarse de que los elementos se reorganicen y se ajusten correctamente cuando el tamaño de pantalla del navegador cambie.
5. Agregar media queries a la página para personalizar el diseño en dispositivos móviles. Lograr que los estilos cambien cuando la pantalla sea más estrecha.

MÓDULO SOBRE DOM E INTERACCIÓN CON EL DOM
Preguntas teóricas
1. ¿Qué es el DOM (Modelo de Objeto de Documento) en el contexto de la programación web?
2. ¿Cuál es la diferencia entre el DOM y el HTML en una página web?
3. ¿Porqué es importante entender y manipular el DOM en el desarrollo web Frontend?
4. ¿Qué son los eventos del DOM y cuáñ es su función en una página web?
5. Proporcionar ejemplos de eventos prácticos y comunes, como “click”, “submit”y “load o DOMContentLoad”.
6. ¿Por qué es importante manejar eventos en la interacción usuario-web y cómo se añaden controladores de eventos a los elementos del DOM?
7. Describir al menos tres métodos para seleccionar elementos del DOM en JavaScript.
8. ¿Cómo se crea un nuevo elemento HTML y se agrega al DOM utilizandoJavaScript?
9. ¿Cuál es la importancia de la manipulación del DOM en la creación de aplicaciones webdinámicas e interactivas?
10. Explicar brevemente los conceptos “eventbubbling”y “eventdelegation”en el contexto de eventos del DOM.


11. ¿Por qué son relevantes los conceptos “eventbubbling”y “eventdelegation”enla gestión de eventos en páginas web con múltiples elementos interactivos?

Preguntas prácticas
1. Escribir una función en JavaScript que tome un botón en el DOM y, al hacer click en él, cambie el color de fondo de un elemento específico en la página. Luego, agregar el botón y el elemento objetivo en el DOM y asociar la función al evento “click”.
2. Crearuna lista no ordenada de elementos (por ejemplo, elementos de lista) en el DOM. Implementarla delegación de eventos(eventdelegation)para que, al hacer clic en cualquier elemento de la lista, se muestre un mensaje en la consola que indique qué elementode la listase ha hecho clic.
3. Agregarun formulario a tu página web con un campo de entrada y un botón "Enviar". Implementaruna función que sea llamada al enviar el formulario y que valide el campo de entrada (por ejemplo, si está vacío),muestre un mensaje de error accesible si es necesarioy en caso de que el formulario esté correctamente diligenciadomuestre en consola un objeto con el dato que ha ingresado el usuario en el campo de entrada y unalert con el siguiente mensaje: “Formulario correctamente diligenciado”.

MÓDULO SOBRE COMUNICACIÓNCON EL SERVIDOR (STORAGE, PROMESAS,ASINCRONÍASY PETICIONES HTTPS)
Preguntas teóricas
1. Definir brevemente el concepto de localStorage y sessionStorage. 
2. Describir las diferencias claves entre localStorage y sessionStorage.
3. ¿Por qué son útiles para almacenar datos en el navegador y cuáles su límite de capacidad?
4. ¿Qué son las promesas en JavaScript y para qué se utilizan en el desarrollo web?
5. Explica el concepto de asincronía en programación y cómo las promesas ayudan a manejar operaciones asincrónicas.
6. Proporciona un ejemplo de cómo se utiliza una promesa para realizar una operación asincrónica, como una solicitud de red.
7. ¿Qué es JSON Server y cómo se utiliza en el desarrollo web?
8. ¿Por qué es útil simular una API REST falsa con JSON Server en el desarrollo frontend?
9. ¿Cuáles son las diferencias claves entre los métodos del objetopromesa.then().catch()y las palabras claves async/await?
10. Proporciona un ejemplo de cómo configurar una API falsa con JSON Server y realizar solicitudes(GET, POST, PUT, PATCH y DELETE)a través de ella.
11. Describe las diferencias entre Fetch y Axios como métodos para realizar solicitudes HTTP en JavaScript.
12. ¿Por qué es importante considerar las peticiones HTTP en aplicaciones web modernas?
13. Proporciona ejemplos de cómo se utilizan Fetchy Axios para realizar solicitudes GET y POST.
14. Explica la importancia del manejo de errores al trabajar con promesas en el desarrollo web.
15. Describe cómo se manejan los errores en las promesas, incluyendo el uso de catch.
16. ¿Cuáles son las diferencias claves entre los métodos del objetopromesa.then().catch()y la estructura try/catch?


17. Proporciona un ejemplo de cómo se puede manejar un error en una promesa al realizar una solicitud de red.

Preguntas prácticas
1. En una sección de la página web construida en los módulos anteriores, permitir a un usuario almacenar y recuperar datos utilizando localStoragey sessionStorage. Demostrar cómo se puede guardar y recuperar datos de estas áreasde almacenamiento del navegador.
2. Escribir una función que utilice una promesa para simular una operación asincrónica, como,por ejemplo,una solicitud de datos. Luego, mostrar los resultados de la promesa en una sección en la página web.
3. Crear una API falsa con JSON Server y realizar una solicitud GET y POST con FetchoAxios y mostrar los resultados en una sección de la página web.
4. Crearun repositorio remoto en GitHub con la estructura de carpetas y archivos dela página web creada para darle respuesta a las preguntas anteriores.
5. La respuesta a las preguntas teóricas debeestar resueltas en un archivo README.md en el repositorio creado en el ítem anterior.
6. Desplegar la página web en GitHub pages.





