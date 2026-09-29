Parte 1: Análisis teórico de conceptos
Explicación de los conceptos básicos
1.1. Describe en tus propias palabras qué es el código fuente, código objeto y código ejecutable. 

Código fuente: son las instrucciones en lenguaje de programación que explica y ayuda a entender cómo se comporta un sistema.
Código objeto: son las instrucciones del código fuerte pero pasado a lenguaje de máquina,que es más fácil de entender para el ordenador. 
Código ejecutable: es el programa final para ser ejecutado por un sistema.

1.2. Explica las fases por las que pasa un programa desde que es escrito en un lenguaje de programación hasta que es ejecutado en el procesador. 

Análisis léxico: dividen y leen el texto letra por letra para comprobar si está bien escrito, es la fase donde se encuentran palabras o letras extrañas que no existen en este lenguaje de programación que se está usando. 

Análisis sintáctico: sabemos que no hay ninguna palabra que no exista en el lenguaje, ahora hay que ver si están en el orden correcto. Por ejemplo cuando se escribe una palabra que debería de estar delante de otro pero le han cambiado de orden y no estaría bien  gramaticalmente. 

Análisis semántico: vamos a revisar que las cosas programadas tengan los datos sean compatibles, evitando poner cosas sin sentido. 

Generación de código intermedio: esta fase es opcional. Después de todas las fases de análisis se supone que el código no tiene ningún error, por lo tanto se puede generar una representación intermedia que es independiente del procesador en el que se va a ejecutar el programa.

Optimización de código intermedio: al igual que el otro, se trata de una fase opcional. Intenta mejorar el código generado para tener un mejor rendimiento.
Generación de código final: generamos código que dependerá del conjunto de instrucciones de la CPU utilizada. Traduce todo a ceros y unos, código máquina.

1.3. Usa ejemplos concretos para cada concepto, mencionando en qué fase interviene cada uno en el desarrollo de un programa.
Análisis léxico: 
nonbre = yingyi.
nonbre → error → nombre

Análisis sintáctico:
edad - 2026= edad nacimiento → error
2026 - edad= edad nacimiento → correcto

Análisis semántico:
¿Es edad nacimiento un número? → Sí

Generación de código final:
Suma= número + 1
La suma sería del número + 1 ( número es una variable)
Clasificación de lenguajes de programación
2.1. Investiga y clasifica los lenguajes de programación en función del nivel de abstracción y el paradigma de programación.

Lenguajes de Bajo Nivel:

Lenguaje Máquina: Instrucciones formadas exclusivamente por número binarias (0 y 1) que el procesador interpreta directamente.
Lenguaje Ensamblador: Sustituye las cadenas binarias por mnemónicos legibles por humanos, pero sigue manteniendo ciertas características del lenguaje de la CPU.

Lenguajes de Nivel Medio:
Ofrecen construcciones de control de flujo típicas del alto nivel (bucles, funciones, estructuras), pero conservan capacidades de bajo nivel.

Por ejemplo: C y C + +.

Lenguajes de Alto Nivel:
No se conserva nada de las características del bajo nivel. Utilizan compiladores para realizar la traducción y suelen incluir recolección de basura.

Por ejemplo: Java y Python

2.2. Da al menos dos ejemplos de lenguajes para cada categoría y explica brevemente por qué pertenecen a esa clasificación. 
Lenguajes de Bajo Nivel:

Lenguaje Máquina: 10111000 = 184 (el número se representa en binario)

Lenguaje Ensamblador: registros como EAX o EBX

Lenguajes de Nivel Medio:

C = usa estructuras de control (if, while)

C + + = mantiene todo el acceso directo a bajo nivel pero añade capas de abstracción.

Lenguajes de Alto Nivel:

Java =
 public class Main {
 public static void main(String[] args) {
        System.out.println (5 + 3);
    }
}

Python = 
precio = 100
printf ("Precio final con descuento: {precio}")
 Parte 2: Actividad práctica y de análisis
Identificación de paradigma de programación a partir de ejemplos. 
Fragmento 1: Un programa recorre una lista de números sumado uno por uno hasta obtener el total. Pista: se describe cómo se realiza la suma paso a paso.

Paradigma imperativo: porque describe el procedimiento exacto paso a paso de cómo se realiza la tarea, recorrer la lista número por número e ir acumulando la suma en la memoria para obtener el resultado.
Fragmento 2: Una consulta a una base de datos busca empleados mayores de 30 años y devuelve solo sus nombres. Pista: se especifica qué resultado se quiere obtener sin detallar cómo se procesa internamente.

Paradigma declarativo: porque indica únicamente el resultado deseado que son los nombres de los empleados mayores de 30 años. Dejando que el motor de la base de datos decida la forma más eficiente de buscar, sin explicárselo paso a paso.
Fragmento 3: Un programa calcula el factorial de un número definiendo que el factorial de 0 es 1 y que, para números mayores, es el número multiplicado por el factorial del número anterior. Pista: la lógica se define recursivamente sin especificar los pasos detallados.

Paradigma declarativo: porque define el problema basándose en una regla matemática sin utilizar variables, asignaciones de memoria ni bucles como “for” o “while" para guiar la ejecución.

Fragmento 4: Un programa filtra productos con precios superiores a 10 dólares recorriendo una lista y comprobando cada producto uno por uno. Pista: se describen detalladamente los pasos del proceso.

Paradigma imperativo: porque usa un bucle de control que coge la lista, recorre elemento por elemento y después evalúa la condición de precio que sea superior a los 10$.
Elige una actividad cotidiana (preparar una receta, organizar un evento, montar un mueble) y describe de dos maneras. Comenta las ventajas y desventajas de cada enfoque.

Plato asiatico: salteado de huevos con tomate

Enfoque imperativo:
Coger dos huevos y un tomate.
Romper los huevos en un bol y batirlos.
Añadir un poco de sal al bol de huevos.
Cortar el tomate en trozos pequeños.
Saltear los huevos y ponerlos en el bol de nuevo.
Salteamos el tomate y ponemos el bol de huevo.
Ponemos sal y azúcar.
¡Plato listo!

Enfoque declarativo:
Le pedimos al chef de un restaurante chino, que nos haga un plato de huevos salteados con tomate, te la elabora y te lo sirven. Sin necesidad de hacerlo nosotros mismos, y sin dar ninguna instrucción. 
