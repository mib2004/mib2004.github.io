---
layout: post
title: "Ejercicios Entrada 2"
date: "2019-07-22 19:58:47 -0500"
---
# Ejercicio 1

```python
a = 12
if a < 10:
  x = True
else:
  x = False
```


Pregunta: ¿cual es el valor de x?
* A) True
* B) False

# Ejercicio 2

```python
num = 18
if num < 5:
  print str(num) + " es menor a 5"
elif num < 10:
  print str(num) + " es menor a 10"
elif num < 15:
  print str(num) + " es menor a 15"
elif num < 20:
  print str(num) + " es menor a 20"
else:
  print str(num) + " es mayor a 20"   
```


Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) 18 es menor a 20
* C) (nada)
* D) 18 es mayor a 20
* E) 18 es menor a 5

# Ejercicio 3

```python
num = 7
if num % 2 == 0:
  print str(num) + " es divisible entre 2"
elif num % 3 == 0:
  print str(num) + " es divisible entre 3"
elif num % 5 == 0:
  print str(num) + " es divisible entre 5"
else:
  print str(num) + " no es divisible por 2, 3 ni 5"
```
> cabe resaltar que = se usa para definir una variable y == para comparar si dos variables son iguales

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) 7 no es divisible por 2, 3 ni 5
* C) (nada)
* D) 7 es divisible entre 3

# Ejercicio 4

```python
a = 0
b = "10"
while a < 10:
	a += 1
	b = b + ", " + str(a + 10)
print b
```


Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) 12345678910
* B) 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
* C) 1, 2, 3, 4, 5, 6, 7, 8, 9, 10

# Ejercicio 5

```python
a = 0
for i in range(10):
  a += i
print a
```


Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) 12345678910
* B) 45
* C) 55

# Ejercicio 6
Piensa en un codigo que usando bucles imprima los 100 primeros numeros



# Ejercicio 7
Piensa en un codigo que imprima si un numero "num" sea par o impar

(TIP: usa num = raw_input("Introduce un numero: ") en el comienzo del codigo para simular una pregunta a un usuario preguntandole por un numero

> la operacion a % b tiene como resultado el resto o remainder de la operacion a / b
>
Ten en cuenta que todo numero que al dividirlo entre dos, no tenga resto o remainder, es par

# Respuestas

#### Ejercicio 1

B) False
#### Ejercicio 2

B) 18 es menor a 20
#### Ejercicio 3

B) 7 no es divisible por 2, 3 ni 5
#### Ejercicio 4

C) 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
#### Ejercicio 5

B) 45
#### Ejercicio 6

este ejercicio se puede resolver con dos tipos de bucles,

con el while loop

```python
a = 100
b =  0
while a > 0:
  b += 1
  a -= 1
  print b
```

con el for loop

```python   
a = 0
for i in range(100):
  a += 1
  print a
```


#### Ejercicio 7

```python
num = raw_input("introduce un numero: ")
if num % 2 == 0:
  print str(num) + " es par"
else:
  print str(num) + " es inpar"
```
