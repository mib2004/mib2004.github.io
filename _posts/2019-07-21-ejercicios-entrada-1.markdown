---
layout: post
title: "Ejercicios Entrada 1"
date: "2019-07-21 19:58:47 -0500"
---

> str(variable) se usa para convertit un valor numerico en un string,esto se usa para juntar numeros con strings, de no usarlo, saldría un error

> la forma de hacer una potecia en python es usando ** x siendo x el exponente

# Ejercicio 1
```python
a = 25
b = " años"
c = str(a) + b
```
Pregunta: ¿Cual sería el valor de "c" tras ejecutar el codigo anterior?
* A) 25años
* B) 25
* C) 25 años
* D) años

# Ejercicio 2
```python
a = 5.00
a /= 2
a *= 4
```
Pregunta: ¿Cual sería el valor de "a" tras ejecutar el codigo anterior?
* A) 10
* B) 7.50
* C) error
* D) 10.00

# Ejercicio 3
```python
a = 5
b = 10.50
c = a + b
print str(c)
```
Pregunta: ¿Que tipo de variable devolveria este codigo tras ejecutarlo?
* A) int
* B) float
* C) string
* D) boolean

# Ejercicio 4
```python
b = 3.00
a = b ** 3
b = 9
```
Pregunta: ¿Cual sería el valor de "a" tras ejecutar el codigo anterior?
* A) 27.00
* B) 729
* C) 27
* D) 9
# Ejercicio 5
```python
a = " hola"
b = a + " como estas"
c = a + b
```
¿Cual sería el valor de "c" tras ejecutar el codigo anterior?
* A) hola como estas
* B)  hola hola como estas
* C) hola hola como estas
* D) holahola como estas
# Ejercicio 6
```python
word1 = "Hello"
word2 = "World"
```
Pregunta: Pensar en un codigo que junte ambas palabras (teniendo en cuenta el espacio entre ellas) e imprimirlas, deben quedar en una sola linea

# Ejercicio 7
```python
num = 4
```
Pregunta: Pensar en un codigo que Aumente la variable num en uno e imprimir el resultado

# Respuestas

#### Ejercicio 1

C) 25 años
#### Ejercicio 2

D) 10.00
#### Ejercicio 3

C) string
#### Ejercicio 4

A)  27.00
#### Ejercicio 5

B)  hola hola como estas
#### Ejercicio 6
```python
print word1 + " " + word2
```
#### Ejercicio 7
```python
num += 1
print num
```
