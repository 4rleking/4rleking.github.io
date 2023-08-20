---
layout: single
title: Introducción a la Programación (Fundamentos)
excerpt: "La programación para muchos nos ha parecido un sueño imposible, o quizás no sabemos por dónde empezar, aquí explicaré todo lo necesario para aprender programación desde cero a experto, ojo (aquí solo es la Introducción, poco a poco se irá profundizando en cada lenguaje que vaya recopilando)."
date: 2023-07-19
classes: wide
header:
  teaser: /assets/images/20230719/Introduccion.jpg
  teaser_home_page: true
categories:
  - Programacion
tags:
  - Fundamentos
---

![](/assets/images/20230719/Introduccion.jpg)

La mayoría de los dispositivos que utilizamos en nuestros días, contienen un software o aplicación que le indica que funciones debe de realizar, que acciones debe de hacer en cada cierto tiempo, o si el usuario presiona o selecciona un botón. 

Desde el software de una Smart Tv, consola de videojuegos, calculadoras científicas, automóviles autónomos, celulares, computadoras, servidores, microondas, lavadoras, por nombrar algunos.

Es demasiado sencillo para el usuario operar este tipo de aplicaciones o dispositivos, pero que hay por detrás de esto.

La *programación* es la actividad mediante la cual las personas le indican a una computadora el procedimiento o conjunto de instrucciones para que, al ejecutarlas, ésta pueda resolver cierto problema deseado.

La programación, aunque no lo parezca es un proceso creativo, es decir, en la mayoría de las ocasiones la tarea puede cumplirse siguiendo distintos caminos y el programador es el que debe imaginar cuáles son y elegir uno (el mejor). Algunos de estos caminos pueden ser mejores que otros, pero en cualquier caso la computadora se limitará a seguir las instrucciones ideadas por el programador (aunque estas instrucciones estén mal planeadas).

Desafortunadamente, las computadoras solo entienden ciertos lenguajes artificiales compuestos por una serie de expresiones; es por ello que a la hora de programar tenemos que ser muy específicos. Es necesario respetar las reglas de lenguaje de programación y ser claros en las indicaciones escritas.

## Algoritmo

La programación consiste en escribir las indicaciones que debe de seguir un computador para completar una tarea, problema o necesidad, pero para poder escribir este tipo de indicaciones, el primer paso es pensar detalladamente cuál puede ser la forma de resolverlo, es decir, crear un *algoritmo*.

Un algoritmo es una estrategia consistente de un conjunto de pasos ordenados que nos lleva a la solución de un problema o alcance de un objetivo.

Para poder resolver un problema computacional debemos de realizar dos actividades hasta el momento:

* Diseño del algoritmo: Diseña o elige un algoritmo que ya exista para resolver el problema deseado (ojo, si vas a seleccionar un algoritmo ya hecho, asegúrate de que no tenga errores o trata de mejorarlo, añade un plus a esa creación).
* Codificación: Expresa el algoritmo en un lenguaje de programación pata que el ordenador lo pueda interpretar y ejecutar.

Al aprender programación estamos destinados a enfrentarnos a problemas con diferentes grados de dificultad, mientras que la codificación se trata de aprender las múltiples reglas de cada uno de los lenguajes de programación.

### Diseño algorítmico

Cotidianamente, utilizamos los algoritmos para realizar casi todas las actividades diarias: preparar el desayuno, sacar a pasear la mascota, encender la tv y poner una película, etc. Cada una de estas tareas requiere llevar acciones de forma ordenada, aunque no hagamos un listado de las mismas y procedamos casi sin pensar.

Sin embargo, cuando pensamos en la solución de un problema que va a resolver una computadora, debemos ser claros y concretos, para asegurarnos de que los pasos del algoritmo llegue a la solución y para que quien tenga que codificarlo, nosotros mismos u otras personas, lo pueda entender sin problemas. 

Por eso, el primer paso es idear un algoritmo para su solución y expresarlo por escrito, por ejemplo, en español, pero adaptando el lenguaje humano a *formas lógicas* que se acerquen a las tareas que puede realizar una computadora. 

En programación, el lenguaje artificial e informal que usan los desarrolladores en la confección de algoritmos recibe el nombre de **pseudocódigo**. Es la herramienta que utilizamos para describir los algoritmos mezclando el lenguaje común con instrucciones de programación.

El pseudocódigo, como cualquier otro lenguaje, está compuesto por:

* Léxico: conjunto de palabras o frases válidas para escribir las instrucciones.
* Sintaxis: reglas que establecen cómo se pueden combinar las distintas partes.
* Semántica: significado que se les da a las palabras o frases.

El pseudocódigo sigue una *estructura secuencial* (define una acción o instrucción que sigue a otra en secuencia). Esta estructura puede representarse de la siguiente forma:

```
ALGORITMO: "Ejemplo"
COMENZAR
    Acción 1
    Acción 2
    ...
    Acción N
FIN
```

Se comienza con un título que describa el problema que el algoritmo resuelve, seguido por la palabra *COMENZAR*. Luego se detallan las acciones o instrucciones a seguir y se concluye con la palabra *FIN*.

Es importante destacar la presencia de sangrías (sangrado) en el ejemplo anterior, que facilitan la lectura. Los algoritmos suelen ser representados también mediante *diagramas de flujo*.

## Codificación

Si bien hay distintos lenguajes de programación, una computadora en definitiva es un aparato que sólo sabe hablar en binario, es decir, sólo interpreta señales eléctricas con dos estados posibles, los cuales son representados por los dígitos binarios 0 y 1. Este sistema de código con ceros y unos que la computadora interpreta como instrucciones o conjuntos de datos se llama lenguaje de máquina (o código de máquina).

a principios de la década de 1950 se inventaron los lenguaje ensambladores, que usan palabras para representar simbólicamente las operaciones que debe realizar la computadora. Cada una de estas palabras reemplaza un código de máquina binario, siendo un poco más fácil programar.

En programación, la idea de simplificar un proceso complejo ignorando algunas de sus partes para comprender mejor lo que hay que realizar y así resolver un problema se conoce como abstracción3. Esto quiere decir que los lenguajes de programación pueden tener distintos niveles de abstracción:

* Lenguajes de bajo nivel de abstracción: permiten controlar directamente el hardware de la computadora, son específicos para cada tipo de máquina, y son más rígidos y complicados de entender para nosotros. El lenguaje ensamblador entra en esta categoría.

* Lenguajes de alto nivel de abstracción: diseñados para que sea fácil para los humanos expresar los algoritmos sin necesidad de entender en detalle cómo hace exactamente el hardware para ejecutarlos. El lenguaje que utilizaremos en este taller, R, es de alto nivel. Son independientes del tipo de máquina.

* Lenguajes de nivel medio de abstracción: son lenguajes con características mixtas entre ambos grupos anteriores.

Si bien podemos programar usando un lenguaje de alto nivel para que nos resulte más sencillo, alguien o algo debe traducirlo a lenguaje de máquina para que la computadora, que sólo entiende de ceros y unos, pueda realizar las tareas. Esto también es necesario incluso si programáramos en lenguaje ensamblador. Para estos procesos de traducción se crearon los compiladores e intérpretes.

Un compilador es un programa que toma el código escrito en un lenguaje de alto nivel y lo traduce a código de máquina, guardándolo en un archivo que la computadora ejecutará posteriormente (archivo ejecutable). Para ilustrar el rol del compilador, imaginemos que alguien que sólo habla español le quiere mandar una carta escrita en español a alguien que vive en Alemania y sólo habla alemán. Cuando esta persona la reciba, no la va a entender. Se necesita de un intermediario que tome la carta en español, la traduzca y la escriba en alemán y luego se la mande al destinatario, quien ahora sí la podrá entender. Ese es el rol de un compilador en la computadora. Ahora bien, el resultado de la traducción, que es la carta escrita en alemán, sólo sirve para gente que hable alemán. Si se quiere enviar el mismo mensaje a personas que hablen otros idiomas, necesitaremos hacer la traducción que corresponda. De la misma forma, el código generado por un compilador es específico para cada máquina, depende de su arquitectura.

Además de los compiladores, para realizar este pasaje también existen los intérpretes. Un intérprete es un programa que traduce el código escrito en lenguaje de alto nivel a código de máquina, pero lo va haciendo a medida que se necesita, es decir, su resultado reside en la memoria temporal de la computadora y no se genera ningún archivo ejecutable. Siguiendo con el ejemplo anterior, es similar a viajar a Alemania con un intérprete que nos vaya traduciendo en vivo y en directo cada vez que le queramos decir algo a alguien de ese país. En su implementación por defecto, el lenguaje R es interpretado, no compilado.

Concluyendo, gracias al concepto de la abstracción podemos escribir programas en un lenguaje que nos resulte fácil entender, y gracias al trabajo de los compiladores e intérpretes la computadora podrá llevar adelante las tareas necesarias.

Cada una de las acciones que componen al algoritmo son codificadas con una o varias instrucciones, expresadas en el lenguaje de programación elegido, y el conjunto de todas ellas constituye un programa. El programa se guarda en un archivo con un nombre generalmente dividido en dos partes por un punto, por ejemplo: mi_primer_programa.R. La primera parte es la raíz del nombre con la cual podemos describir el contenido del archivo. La segunda parte es indicativa del uso del archivo, por ejemplo, .R indica que contiene un programa escrito en el lenguaje R. El proceso general de ingresar o modificar el contenido de un archivo se denomina edición.