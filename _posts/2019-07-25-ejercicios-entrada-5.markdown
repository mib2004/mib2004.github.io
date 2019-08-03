---
layout: post
title: "Ejercicios entrada 5"
date: "2019-07-25 19:58:47 -0500"
---

# Ejercicio 1

```python
import random

a = randint(1, 10)
print a
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) numero al azar del 1 al 10
* B) error
* C) numero al azar del 1 al 9

# Ejercicio 2

```python
import random

a = random.randint(1, 10)
a *= 2
print a
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) numero al azar del 1 al 10
* C) numero par al azar del 2 al 20

# Ejercicio 3

```python
import random
a = []
print random.choice(a)
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) nada
* B) error
* C) un elemento al azar de a

# Ejercicio 4

```python
import random

a = ("hola", "como", "estas")
print random.choice(a)
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) hola como estas
* C) un elemento al azar de a

# Ejercicio 5
Piensa en un codigo que imprima un numero al azar del 5 al 20
# Ejercicio 6
Piensa en un codigo que imprima una vocal al azar
# Respuestas

#### Ejercicio 1

A) error

#### Ejercicio 2

C) numero par al azar del 2 al 20

#### Ejercicio 3

B) error

#### Ejercicio 4

C) un elemento al azar de a

#### Ejercicio 5

```python
import random

print random.randint(5, 20)
```

#### Ejercicio 6

```python
import random

a = (a, e, i, o, u)
print random.choice(a)
```
