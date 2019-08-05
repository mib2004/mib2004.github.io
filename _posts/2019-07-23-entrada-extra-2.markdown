---
layout: post
title: "Entrada extra 2: scoping"
date: "2019-07-23 19:58:47 -0500"
---

Este es el tema que la mayoria de personas tienden a olvidar como es, pero si prestas basstante atencion se te quedara grabado. Como habras notado, las funciones usan variables, estas variables se usan unicamente para esas funciones, es decir, si ya exista la variable a y luego llamas una funcion que usa una variable llamada a, la original no cambia.

```python

a = 30

def funcion1(a):
  return a + 2

funcion1(8)
print a
```
```python
> 10
> 30
```

Luego esta la otra parte de scoping que es cuando hay una funcion dentro de una funcion. Esto no se ve muy frecuente ya que es un tema mas avanzado para ejemplos muy especificos, pero lo vamos a ver de todas formas porque es teoria

Aqui un ejemplo:

```python
def funcion1(a):
  def funcion2(a):
    return a + 2
  funcion2(a * 2)
funcion1(5)
```
en este caso "a" comienza siendo 5 en funcion1, luego "a" pasa a ser 10 en funcion2 y luego todo el codigo devolveria 12. Este es un caso bastante sencillo de scoping, pero luego cuando empiezas a programar con funciones mas avanzadas o mas complejas que requieren mas de 5 funciones dentro de si mismas, tiene el mismo principio solo que con cosas mas elaboradas.
