---
layout: post
title: "Ejercicios entrada 4"
date: "2019-07-24 19:58:47 -0500"
---

# Ejercicio 1

```python
a = (1, 2, 3, 4, "hola")
print str(a) + " es un tuple"
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) 1, 2, 3, 4, "hola" es un tuple
* B) (1, 2, 3, 4, "hola" es un tuple)
* C) (1, 2, 3, 4, "hola") es un tuple

# Ejercicio 2

```python
a = {nombre: Marcelo, edad: 14}
a[edad] = 15
print a[edad]
```


Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) 14
* B) 15
* C) error

# Ejercicio 3

```python
a = [3, "hola", 4]
b = [0, 6, "bueno"]
print a + b
```
> una vaiable avanzada solo se puede sumar con su mismo tipo

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) [3, "hola", 4] [0, 6, "bueno"]
* B) [3, "hola", 4, 0, 6, "bueno"]
* C) error

# Ejercicio 4

```python
a = [3, "hola ", 4]
b = (0, 6, "bueno ")
print a[1] + b[2]
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) hola bueno
* B) 9
* C) error

# Ejercicio 5

```python
a = [1, 2]
a.append("hola")
print a
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) [1, 2, "hola"]
* B) [1, 2]"hola"
* C) error

# Ejercicio 6

Usando el metodo .append y un bucle, piensa en un codigo que cree una lista con los 100 primeros numeros y luego los imprime

# Ejercicio 7

Usando raw_input() piensa en un codigo que cree un diccionario con el nombre y edad de un usuario

# Respuestas

#### Ejercicio 1

C) (1, 2, 3, 4, "hola") es un tuple

#### Ejercicio 2

B) 15

#### Ejercicio 3

B) [3, "hola", 4, 0, 6, "bueno"]

#### Ejercicio 4

A) hola bueno

#### Ejercicio 5

A) [1, 2, "hola"]

#### Ejercicio 6

```python
a =  []
for i in range(1, 101):
  a.append(i)
print a
```

#### Ejercicio 7

```python
persona1= {}
nombre = raw_input("¿Cual es tu nombre?")
persona1["nombre"] = nombre
edad = raw_input("¿Cual es tu edad?")
persona1["edad"] = edad
```
