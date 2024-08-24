NAME: Jesus David Bernal Gonzalez

1) diferencia entre un IDE y un archivo de texto 


El editor de texto, como su nombre lo indica 
es para editar texto: crearlo, modificarlo, guardarlo, etc. El IDE, es un entorno de desarrollo, o sea, se compone de más 
herramientas necesarias para esta labor. Una de estas herramientas es el editor de código; pero adicional, trae compilador/interprete, 
visualizador, complementos, etc. Un ejemplo claro: un editor de texto es como el bloc de notas, allí puedes escribir 
código pero no lo puedes ejecutar ni visualizar su resultado. No tienes herramientas como autocompletar o comprobar si existe 
alguna variable o similar. En cambio, una IDE como Intellij te permite crear/escribir código, correrlo 
(ejecutarlo, ver que funcione), al hacer click encima de una variable ver en dónde más está, autocompleta o sugiere a 
medida que vas escribiendo código,si estás trabajando con web te permite desplegar servidores para testear, etc

2) Tipos de lenguajes de programación (tipados y no tipados).

tipos de lenguajes
TIPADO / NO TIPADO

LENGUAJE TIPADO
Los lenguajes tipados requieren declarar variables con un tipo de dato por lo cual no permite violaciones al tipo de datos.

Aunque es vas verboso es menos propenso a presentar errores de sintaxis ya que el compilador los detecta.
Al usar funciones se tiene la total certeza de que tipo de dato devueleve
No se puede cambiar el tipo de dato despues de declarar una variable

LENGUAJE NO TIPADO
Los lenguajes no tipados son aquellos que no requieren declarar variables con un tipo de dato por lo cual permite la modificación del tipo de dato.
Código mas legible y ruta de aprendizaje mas sencilla
se puede cambiar el tipo de dato despues de haber declarado la variable

3) Tipos de datos en Java:

NUMERICOS: 

Nombre	bytes	Rango
long	8	9,223,372,036,854,775,808 a 9,223,372,036,854,775,807
int	    4	2,147,483,648 a 2,147,483,647
short	2	32,768 to 32,767
byte	1	128 to 127
En la mayoria de los casos usaremos el tipo de dato int para números positivos.

Ejemplos

byte diasMes = 31; //Aproximadamente
short diasLustro = (12 * 31) * 5;
int velocidadLuz = 299792458;
long añoLuz = velocidadLuz * 365;


CADENAS

Declaración y Creación:

Las cadenas se pueden declarar usando literales o el constructor de la clase String.
Inmutabilidad:

Las cadenas son inmutables, lo que significa que una vez creadas, no se pueden modificar.
Concatenación:

Las cadenas se pueden concatenar utilizando el operador + o métodos como concat().
Longitud:

La longitud de una cadena se puede obtener utilizando el método length().
Comparación:

Las cadenas se comparan utilizando el método equals() para verificar la igualdad de contenido.
Acceso a Caracteres:

Los caracteres dentro de una cadena se pueden acceder usando el método charAt().
Subcadenas:

Puedes obtener una subcadena de una cadena usando los métodos substring().
Conversión de Mayúsculas y Minúsculas:

Las cadenas se pueden convertir a mayúsculas con toUpperCase() o a minúsculas con toLowerCase().
Eliminación de Espacios en Blanco:

Eliminar espacios en blanco al inicio y al final de una cadena usando el método trim().
Formateo e Interpolación:

Puedes formatear cadenas usando String.format() y, en versiones recientes de Java, usar interpolación de cadenas.


FECHAS
Este paquete java.time incluye muchas clases, pero las básicas son:

LocalDate: representa a fechas sin la hora y nos facilita su manejo para declararlas, sumar y restar fechas y compararlas.

LocalTime: es idéntica a la anterior pero para el manejo de horas, sin ninguna fecha asociada, pudiendo así compararlas, sumar o restar tiempo a las mismas...

LocalDateTime: como puedes suponer, es una combinación de las dos anteriores, que permite hacer lo mismo con fechas y horas simultáneamente.

Instant: es muy parecida a la anterior pero a la vez muy diferente. Se usa para almacenar un punto determinado en el tiempo, o sea con fecha y hora, pero guarda su valor como un timestamp de UNIX, es decir, en nanosegundos desde el epoch de UNIX (1/1/1970 a las 00:00) y usando la zona horaria UTC. Es muy útil para manejar momentos en el tiempo de manera neutra e intercambiarlo entre aplicaciones y sistemas, por lo que lo verás utilizado muy a menudo.

ZonedDateTime: esta clase es como la LocalDateTime pero teniendo en cuenta una zona horaria concreta, ya que las anteriores no la tienen en cuenta.

Period: esta clase auxiliar nos ayuda a obtener diferencias entre fechas en distintos periodos (segundos, minutos, días...) y también a añadir esas diferencias a las fechas.

Duration: esta es muy parecida a la anterior pero para manejo de horas exclusivamente.

