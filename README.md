# HERENCIA
## EJERCICIO 1
class Persona:
    def _init_(self, nombre, edad):
        self.nombre  = nombre 
        self.edad = edad
class Estudiante(Persona):
    def _init_(self, nombre, edad, grado):
        super()._init_(nombre, edad)
        self.grado = grado
Cristian = Estudiante("Cristian", 17, "11°")

print("El nombre del estudiante es: " + Cristian.nombre)

print("La edad del estudiante es: " + str(Cristian.edad))

print("El grado del estudiante es:" + Cristian.grado)

## EJERCICIO 2

class Animal:
    def _init_(self, nombre, especie):
        self.nombre = nombre
        self.especie = especie

class Perro(Animal):
    def _init_(self, nombre, especie, raza):
        super()._init_(nombre, especie)
        self.raza = raza

Max = Perro("Max", "Canino", "Labrador")

print("El nombre del perro es: " + Max.nombre)
print("La especie del perro es: " + Max.especie)
print("La raza del perro es: " + Max.raza
## EJERCICIO  2

class Vehiculo:
    def _init_(self, marca, año):
        self.marca = marca
        self.año = año

class Coche(Vehiculo):
    def _init_(self, marca, año, modelo):
        super()._init_(marca, año)
        self.modelo = modelo

mi_coche = Coche("Toyota", "2022", "Corolla")

print("La marca del coche es: " + mi_coche.marca)
print("El año del coche es: " + mi_coche.año)
print("El modelo del coche es: " + mi_coche.modelo)




### Ejercicio 1: Persona y Estudiante
Crea una clase Persona con los atributos nombre y edad. Luego, crea una clase Estudiante que hereda de Persona y agrega el atributo grado. Se crea un estudiante llamado "Cristian", y se imprimen su nombre, edad y grado.

### Ejercicio 2: Animal y Perro
Define una clase Animal con nombre y especie. Luego, crea una clase Perro que hereda de Animal y añade el atributo raza. Se crea un perro llamado "Max" y se imprime su nombre, especie y raza.

### Ejercicio 3: Vehículo y Coche
Crea una clase Vehiculo con marca y año. Luego, crea una clase Coche que hereda de Vehiculo y agrega el atributo modelo. Se crea un coche llamado "Toyota Corolla" y se imprimen su marca, año y modelo.
