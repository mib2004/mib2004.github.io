---
layout: post
title: "Ejercicios entrada 7"
date: "2019-07-26 19:58:47 -0500"
---
# Ejercicio 1

```python
class Persona:
  def __init__(nombre):
    self.nombre = nombre
  def saludar(self):
    print "hola, me llamo " + self.nombre
class Estudiante(Persona):
  pass
p1 = Estudiante(Marcelo)
p1.saludar()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) hola, me llamo Marcelo
* C) Marcelo

# Ejercicio 2

```python
class Persona:
  def __init__(nombre):
    self.nombre = nombre
  def saludar(self):
    print "hola, me llamo " + self.nombre
class Estudiante(Persona):
  def saludar(self):
    print "hola, soy un estudiante y me llamo " + self.nombre
p1 = Estudiante(Marcelo)
p1.saludar()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) hola, soy un estudiante y me llamo Marcelo
* B) hola, me llamo Marcelo
* C) error

# Ejercicio 3

```python
class Persona:
  def __init__(nombre):
    self.nombre = nombre
  def saludar(self):
    print "hola, me llamo " + self.nombre
class Estudiante:
  pass
p1 = Estudiante(Marcelo)
p1.saludar()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) Marcelo
* B) hola, me llamo Marcelo
* C) error

# Ejercicio 4

```python
class Persona:
  def __init__(nombre):
    self.nombre = nombre
  def saludar(self):
    print "hola, me llamo " + self.nombre
class Estudiante(Persona):
  def __init__(nombre, inteligencia):
    self.inteligencia = inteligencia
  def saludar(self):
    print "hola, me llamo " + self.nombre " y tengo " + self.inteligencia + " de inteligencia"
p1 = Estudiante(Marcelo, 5)
p1.saludar()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) hola, me llamo Marcelo y tengo 5 de inteligencia
* B) hola, me llamo Marcelo
* C) error

# Ejercicio 5

```python
class Carro:
  def __init__(modelo):
    self.modelo = modelo
  def presentarse(self):
    print "soy, un carro marca " + self.modelo
class CarroDeCarrera(Carro):
  def __init__(modelo, velocidad):
    Carro.__init__(self, modelo)
    self.velocidad = velocidad
  def presentarse(self):
    print "soy, un carro marca " + self.modelo " y tengo una velocidd de " + self.velocidad + " Km/h"
p1 = CarroDeCarrera(Ford, 220)
p1.presentarse()
```

Pregunta: ¿Que se imprime tras ejecutar este codigo?
* A) error
* B) soy un carro marca ford y tengo una velocidad de 120
* C) soy, un carro marca Ford y tengo una velocidd de 220 Km/h


# Ejercicio 6

Piensa en un codigo que cree una clase llamada persona a la cual se le atribuye un nombre, y la habilidad de presentarse, y otra clase llamada trabajador que herede el atributo de nombre, y tenga un nuevo atributo llamado trabajo, sobreescribiendo la funcion de presentarse ahora mencionando su trabajo

# Ejercicio 7

Piensa en un codigo que cree una clase llamada instrumento que tenga un atributo de calidadDeSonido que sea un numero al azar del 1 al 10 y un atributo marca, y la habilidad de presentarse diciendo su marca, y otra clase llamada guitarra, que herede el atributo de calidadDeSonido y marca, y tenga un nuevo atributo llamado calidadDeGuitarra que sea otro numero al azar del 1 al 10, conservando su funcion de presentarse, y que tenga una nueva funcion que se llame PruebaDeCalidad que multiplique calidadDeSonido por calidadDeGuitarra y presente el nuevo numero en un porcentaje de la maxima calidad posible.


# Respuestas

#### Ejercicio 1

B) hola, me llamo Marcelo

#### Ejercicio 2

A) hola, soy un estudiante y me llamo Marcelo

#### Ejercicio 3

C) error

#### Ejercicio 4

C) error

#### Ejercicio 5

C) soy, un carro marca Ford y tengo una velocidd de 220 Km/h

#### Ejercicio 6

```python
class Persona:
  def __init__(self, nombre):
    self.nombre = nombre
  def presentarse(self):
    print "hola me llamo " + self.nombre
class Trabajador(Persona):
  def __init__(self, nombre, trabajo):
    Persona.__init__(self, nombre)
    self.trabajo = trabajo
  def presentarse(self):
    print "hola me llamo " + self.nombre " y mi trabajo es " + self.trabajo

```
#### Ejercicio 7

```python
import random
class Instrumento:
  def __init__(self, marca):
    self.marca = marca
    self.calidadDeSonido = random.randint(1, 10)
  def calidad(self):
    print "soy un instrumento de marca " + self.marca
class Guitarra(Instrumento):
  def __init__(self):
    Instrumento.__init__(self, marca)
    self.calidadDeSonido = random.randint(1, 10)
    self.calidadDeGuitarra = random.randint(1, 10)
  def pruebaDeCalidad(self):
    print "tengo un " + str(self.calidadDeSonido * self.calidadDeGuitarra) + "% de la maxima calidad"
```
