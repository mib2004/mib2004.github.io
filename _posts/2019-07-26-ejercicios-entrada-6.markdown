---
layout: post
title: "Ejercicios entrada 6"
date: "2019-07-26 19:58:47 -0500"
---

# Ejercicio 1

```python
class Persona
p1 = Persona()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) nada
* C) p1 = Persona

# Ejercicio 2

```python
class Persona:
  def __init__(self, nombre):
    self.nombre = nombre
  def hola(self):
    print "hola, me llamo " + self.nombre
p1 = Persona(Juan)
p1.hola()

```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) nada
* C) hola, me llamo Juan

# Ejercicio 3

```python
class Profesor:
  def __init__(self, nombre, curso):
    self.nombre = nombre
    self.curso = curso
  def presentarse(self):
    print "hola, mi nombre es " + self.nombre + " y enseño el curso de " + self.curso
p1 = Profesor(Juan, Mate)
p1.presentarse()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A)
* B) hola, mi nombre es Juan y enseño el curso de Mate
* C)

# Ejercicio 4

```python
class Carro:
  def __init__(self, velocidad):
    self.velocidad = velocidad
  def cienKm(self):
    print "El carro ha hecho 100 kilometros en " + str(60 * 100 / self.velocidad) + " minutos"
c1 = Carro(50)
c1.cienKm()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) El carro ha hecho 100 kilometros en 240 minutos
* B) El carro ha hecho 100 kilometros en 0 minutos
* C) El carro ha hecho 100 kilimetros en 120 minutos

# Ejercicio 5

```python
class Carro:
  def __init__(self, velocidad):
    self.velocidad = velocidad
  def xKm(self, kilometros):
    print "El carro ha hecho " + str(kilometros) + " kilometros en " + str(60 * kilometros / self.velocidad) + " minutos"
c1 = Carro(75)
c1.xKm(150)
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) El carro ha hecho 150 kilometros en 120 minutos
* B) El carro ha hecho 150 kilometros en 150 minutos
* C) El carro ha hecho 100 kilometros en 75 minutos

# Ejercicio 6
Piensa en un codigo que cree una clase llamada Persona la cual al llamarla tienes que introducir un nombre y un apellido y luego los imprima mientras saluda
# Ejercicio 7
Piensa en un codigo que cree una clase llamada Profesor que le des un nombre y tenga una profesionalidad al azar del 1 al 10


# Respuestas

#### Ejercicio 1

A) error

#### Ejercicio 2

C) hola, me llamo Juan

#### Ejercicio 3

B) hola, mi nombre es Juan y enseño el curso de Mate

#### Ejercicio 4

C) El carro ha hecho 100 kilimetros en 120 minutos

#### Ejercicio 5

A) El carro ha hecho 150 kilometros en 120 minutos

#### Ejercicio 6

```python
class Persona:
  def __init__(self, nombre, appellido):
    self.nombre = nombre
    self.apellido = apellido
  def saludar(self):
    "hola me llamo " + self.nombre + " " + self.apellido
```
#### Ejercicio 7

```python
import random
class Profesor:
  def __init__(self, nombre):
    self.nombre = nombre
    self.profesionalidad = random.randint(1, 10)
```
