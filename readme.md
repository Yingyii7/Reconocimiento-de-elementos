# **Reconocimiento de Elementos en el Desarrollo de un Programa Informático**

> **Palabra del día:** compañeros

## **🎯 Objetivo**

Evaluar la capacidad de los alumnos para reconocer los elementos y herramientas que intervienen en el desarrollo de un programa informático, diferenciando los conceptos de **código fuente, código objeto y código ejecutable**, así como clasificando los lenguajes de programación en **imperativos y declarativos**.

---

# **Parte 1: Análisis teórico de conceptos**

## **1\. Conceptos básicos**

### **Código fuente**

El **código fuente** es el conjunto de instrucciones que escribe un programador utilizando un lenguaje de programación. Es legible y modificable por las personas.

Ejemplo en Python:

print("Hola, mundo")

### **Código objeto**

El **código objeto** es el resultado de traducir el código fuente a instrucciones que pueden ser procesadas posteriormente por el ordenador. Normalmente es generado por un compilador.

Código fuente → Compilador → Código objeto

Puede aparecer en archivos como `.o` o `.obj`.

### **Código ejecutable**

El **código ejecutable** es el programa preparado para ser ejecutado por el sistema operativo.

Por ejemplo, en Windows:

programa.exe

El proceso general es:

Código fuente  
      ↓  
Compilación  
      ↓  
Código objeto  
      ↓  
Enlazado  
      ↓  
Código ejecutable  
      ↓  
Ejecución en el procesador

---

## **2\. Fases por las que pasa un programa**

### **1\. Escritura del código fuente**

El programador escribe las instrucciones utilizando un lenguaje como **C, C++, Java o Python**.

### **2\. Análisis léxico**

El compilador analiza los caracteres del código y los agrupa en elementos llamados **tokens**.

Por ejemplo:

int edad \= 20;

Los elementos `int`, `edad`, `=` y `20` son identificados como diferentes componentes del código.

### **3\. Análisis sintáctico**

Se comprueba que las instrucciones cumplen las reglas gramaticales del lenguaje.

Por ejemplo:

int edad \=

Esta instrucción produciría un error de sintaxis.

### **4\. Análisis semántico**

Se comprueba que el código tenga un significado válido y que las operaciones sean coherentes con los tipos de datos utilizados.

### **5\. Compilación**

El compilador transforma el código fuente en código objeto o en una representación intermedia.

Código fuente → Compilador → Código objeto

### **6\. Enlazado**

El enlazador combina el código objeto con las bibliotecas y otros componentes necesarios.

Código objeto \+ Bibliotecas → Enlazador → Ejecutable

### **7\. Carga y ejecución**

El sistema operativo carga el programa en memoria y el procesador comienza a ejecutar sus instrucciones.

Ejecutable → Memoria → Procesador → Resultado

---

# **Parte 2: Clasificación de lenguajes de programación**

## **1\. Según el nivel de abstracción**

### **Lenguajes de alto nivel**

Son lenguajes cercanos al lenguaje humano y permiten desarrollar programas sin tener que controlar directamente muchos detalles del hardware.

**Ejemplos:**

* **Python:** tiene una sintaxis sencilla y permite desarrollar programas rápidamente.

* **Java:** proporciona un alto nivel de abstracción y permite desarrollar aplicaciones para diferentes plataformas mediante la máquina virtual de Java.

### **Lenguajes de nivel medio**

Combinan características de alto y bajo nivel. Permiten trabajar con estructuras propias de lenguajes de alto nivel y también acceder a determinadas características de la memoria y del hardware.

**Ejemplos:**

* **C:** permite utilizar estructuras de alto nivel y trabajar directamente con memoria mediante punteros.

* **C++:** proporciona abstracciones de alto nivel, pero también permite un control bastante directo sobre los recursos del sistema.

### **Lenguajes de bajo nivel**

Están muy próximos al funcionamiento interno del procesador y del hardware.

**Ejemplos:**

* **Lenguaje ensamblador:** utiliza instrucciones relacionadas directamente con las operaciones de la CPU.

* **Código máquina:** está formado por instrucciones que el procesador puede interpretar directamente.

---

## **2\. Según el paradigma de programación**

### **Programación imperativa**

La programación **imperativa** indica al ordenador **cómo debe realizar una tarea**. El programa especifica una serie de instrucciones y operaciones.

**Ejemplos:**

* **C:** utiliza instrucciones, variables, condiciones y bucles.

* **Java:** permite describir mediante instrucciones el proceso que debe seguir el programa.

Ejemplo:

total \= 0

for numero in numeros:  
    total \= total \+ numero

Aquí se indican explícitamente los pasos para calcular el total.

### **Programación declarativa**

La programación **declarativa** se centra principalmente en indicar **qué resultado se quiere obtener**, sin especificar todos los pasos internos.

**Ejemplos:**

* **SQL:** permite indicar qué información queremos obtener de una base de datos.

* **Prolog:** permite definir hechos y reglas para encontrar soluciones.

Ejemplo:

SELECT nombre  
FROM empleados  
WHERE edad \> 30;

Aquí se indica qué información queremos obtener, mientras que el sistema determina cómo realizar la consulta.

---

# **Parte 3: Actividad práctica y de análisis**

## **Identificación de paradigmas**

### **Fragmento 1**

> Un programa recorre una lista de números sumándolos uno por uno hasta obtener el total.

**Clasificación:** Imperativo.

**Justificación:** se describe el procedimiento paso a paso: recorrer la lista, tomar cada número y sumarlo al total. Se está indicando **cómo** realizar la operación.

---

### **Fragmento 2**

> Una consulta a una base de datos busca empleados mayores de 30 años y devuelve solo sus nombres.

**Clasificación:** Declarativo.

**Justificación:** se indica el resultado que queremos obtener, sin especificar cómo debe recorrer o procesar internamente la base de datos.

---

### **Fragmento 3**

> Un programa calcula el factorial de un número `n`, definiendo que el factorial de 0 es 1 y, para números mayores, multiplicando el número por el factorial del número anterior.

**Clasificación:** Declarativo.

**Justificación:** la solución se expresa mediante una definición matemática recursiva:

0\! \= 1  
n\! \= n × (n-1)\!

La definición establece la relación necesaria para obtener el resultado sin describir una secuencia detallada de instrucciones.

---

### **Fragmento 4**

> Un programa filtra productos con precios superiores a 10 dólares recorriendo una lista y comprobando cada producto uno por uno.

**Clasificación:** Imperativo.

**Justificación:** se explican los pasos que debe realizar el programa: recorrer la lista, comprobar cada producto y seleccionar aquellos cuyo precio sea superior a 10 dólares.

---

# **Parte 4: Actividad en grupo**

## **Actividad cotidiana: preparar una receta**

Para realizar esta actividad, los **compañeros** pueden escoger una tarea cotidiana y explicarla desde los dos paradigmas.

### **Descripción imperativa**

En el enfoque imperativo se indican detalladamente los pasos que deben realizarse.

Por ejemplo, para preparar un bocadillo:

1. Sacar dos rebanadas de pan.

2. Colocar una rebanada sobre un plato.

3. Añadir los ingredientes.

4. Colocar la segunda rebanada encima.

5. Cortar el bocadillo.

6. Servirlo.

El procedimiento explica **cómo** conseguir el resultado.

### **Descripción declarativa**

En el enfoque declarativo se indica principalmente el resultado que se desea conseguir:

> Preparar un bocadillo con los ingredientes seleccionados y dejarlo listo para comer.

No se especifican todos los pasos necesarios para prepararlo.

---

## **Comparación entre los dos enfoques**

| Característica | Imperativo | Declarativo |
| ----- | ----- | ----- |
| Se centra en | Cómo realizar una tarea | Qué resultado obtener |
| Instrucciones | Detalladas | Más generales |
| Control del proceso | Alto | Menor |
| Ejemplo | C, Java | SQL, Prolog |
| Ventaja | Permite controlar el proceso paso a paso | Puede simplificar la descripción del problema |
| Desventaja | Puede requerir más código y detalles | Se tiene menos control sobre cómo se realiza internamente |

---

# **Conclusiones**

El desarrollo de un programa informático implica diferentes fases y herramientas. El **código fuente** representa las instrucciones escritas por el programador, mientras que el **código objeto** es el resultado de su traducción y el **código ejecutable** es el programa preparado para ser ejecutado por el sistema.

Los lenguajes de programación pueden clasificarse según diferentes criterios. Según su nivel de abstracción pueden ser de **alto, medio o bajo nivel**, mientras que según su paradigma pueden ser **imperativos o declarativos**.

La principal diferencia entre los paradigmas imperativo y declarativo es que el primero se centra en explicar **cómo** realizar una tarea, mientras que el segundo se centra principalmente en indicar **qué resultado se desea obtener**.

---

# **Entrega**

La actividad debe entregarse en una **presentación de 5 a 10 páginas** que contenga:

* Las respuestas de la Parte 1\.

* La explicación de código fuente, código objeto y código ejecutable.

* Las fases por las que pasa un programa.

* La clasificación de los lenguajes de programación.

* Ejemplos de lenguajes de alto, medio y bajo nivel.

* Ejemplos de lenguajes imperativos y declarativos.

* La clasificación y justificación de los cuatro fragmentos de la Parte 2\.

* La descripción de la actividad realizada en grupo.

* La comparación entre las descripciones imperativa y declarativa.

---

# **Criterios de evaluación**

## **RA1**

**Reconoce los elementos y herramientas que intervienen en el desarrollo de un programa informático, analizando sus características y las fases en las que actúan hasta llegar a su puesta en funcionamiento.**

### **Indicadores**

* **c)** Se han diferenciado los conceptos de **código fuente, código objeto y código ejecutable**.

* **e)** Se han clasificado los **lenguajes de programación**.

