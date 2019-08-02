---
layout: post
title: "Entrada Extra 1: Algoritmos Guess and Check y Bisection Search"
date: "2019-07-22 19:58:47 -0500"
---
Al haber visto los bucles, ahora puede abarcar el tema de dos algoritmos bastante utiles para encontrar numeros,

* Guess and Check: Que consiste en tratar de adivinar y verificar si es correcto y repetirlo hasta que se alcanze el resultado

```python
x = int(raw_input("Introduce un numero"))
ans = 0
while ans ** 3 < x:
  ans = ans + 1
if ans ** 3 != x:
  print str(x) + "no es un cubo perfecto"
else:
  print "la raiz cubica de " + str(x) + " es " + str(ans)
```
> != significa no es igual

* Bisection search: Que consiste en primero establecer dos limites que sabes que el resultado no va a pasar, luego ir partiendolo por la mitad, cada vez modificando los limites hasta llegar a un aproximado bastante cercano al resultado

```python
x =int(raw_input("introduce un numero"))
aproximado = 0.001
minimo = 0.0
maximo = x
ans = (maximo + minimo) / 2
while abs(ans ** 2 - x) >= aproximado:
  if ans ** 2 < x:
    minimo = ans
  else:
    maximo = ans
  ans = (maximo + minimo) / 2
print "la raiz cuadrada de " + str(x) + "es aproximadamente" + str(ans)
```
> abs(x) significa el valor absoluto de x

 Estos dos algoritmos pueden servir bastante para poder encontrar numeros bastante facil, un ejemplo de su uso seria para encontrar raices de numero como se puede ver en los ejemplos.
