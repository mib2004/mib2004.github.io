---
layout: post
title: "Entrada extra 3: algoritmo evolutivo"
date: "2019-07-26 19:38:47 -0500"
---
Este es un algoritmo un poco avanzado que se usa en los objetos para que puedan mejorar mientras más tiempo corra el programa. Este algoritmo consta de 3 pasos. Antes de comenzar con los pasos a seguir seria bueno primero explicar en que forma funciona este algoritmo. Este algoritmo consta de tener varios objetos que tengan un mismo objetivo, lanzarlos para ver quien esta más cerca, los más cercanos vendrían a ser como los "padres" que se juntan entre ellos para que tengan como un "hijo", el cual va a seguir lo que hicieron sus padres. Este proceso se repetiría muchísimas veces, creando asi muchas generaciones cada una mejor que la otra, hasta que se perfeccione o se llegue bastante cerca a la perfección de llegar al objetivo.


Ahora si comenzamos con los pasos. El primer paso vendría siendo el crear una población que tengan un objetivo en común. En un comienzo la población debería tratar de llegar al objetivo de forma al azar, siendo unos más efectivos que otros dependiendo de que tanta suerte tengan.



El segundo paso pasaría a ser la selección. Este se refiere a seleccionar a aquellos objetos de la población que estuvieron más cerca a el objetivo, estos luego se agregarían a una lista en la cual dependiendo de que tan cerca estén del objetivo se agrega a la lista una o múltiples veces. Este crearía una probabilidad a todos los objetos pero los que estuvieron más cerca tendrían una probabilidad mucho más alta que los demás dependiendo de que tan lejos llegaron. Luego se sacarían 2 objetos al azar de esa probabilidad y ellos se convertirían en los "padres"



El tercer paso es la variación, una vez los "padres" son escogidos, ellos se fucionan, es decir una parte de ellos se junta con otra parte del otro. Esto se puede hacer de forma al azar o solo la mitad con la otra mitad. Estas dos partes se unirían para formar un objeto "hijo" el cual tiene parte de cada uno de sus "padres" significando que él ha heredado lo que sus "padres" han hecho. Luego, posible variación en esto, el programador puede poner que haya una pequeña posibilidad de que algún aspecto de el "hijo" mute y sea al azar. Esto se usa para darle variación a la población y crea posibles caminos que no se consiguieron en un inicio en la población inicial.



Ahora un ejemplo para poder entender de mejor manera. Digamos que un mono está tecleando 9 letras al azar, cual seria la probabilidad de que escriba la palabra "programar". Si el mono solo tecleara letras de la "a" a la "z" tendríamos 27 posibles resultados por cada letra, esto significaría que la probabilidad de que el mono tecleara "programar" es de 1 en 27 ^ 9, que es, 1 en 7 625 597 484 987. Si él intentara 100 veces por minuto, teniendo en cuenta que no va a repetirse nunca, el mono teóricamente tomaría 145 083 años en escribir "programar". Ahora esto es mucho tiempo, pero usando el algoritmo evolutivo se puede acortar bastante.



En este caso vamos a tomar como población 1000 palabras al azar que escribió el mono en un comienzo. Estas palabras por cada letra que tengan bien tendrán +1 en posibilidad. Por cada punto de posibilidad se va a agregar el objeto 1 vez a una lista. Al terminar de colocar los objetos en la lista, digamos que hubieron 50 que tuvieron solo una letra bien, hubieron 10 que tuvieron 2 y 2 que tuvieron 3. Ahora a partir de esa lista se funcionarían y se crearían 1000 palabras más y este proceso se repitiría hasta llegar a "programar"
