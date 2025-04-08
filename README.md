# HERENCIA
### EJERCICIO 1
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

### EJERCICIO 2

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
### EJERCICIO  2

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
