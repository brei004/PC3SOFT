

## Ejercicios

1. Refactoriza el código del juego para adherirse a los principios SOLID 

## Single Responsibility Principle (SRP)

En jugador se está usando métodos que serían más adecuados para una clase inventario y no dentro de la misma clase Jugador, como son los de agregar objeto o usar objeto

- Nueva clase Jugador
![alt text](image-37.png)

- Nueva clase Inventario
![alt text](image-38.png)


## Open/Closed Principle (OCP)

Luego, creamos una interfaz Comando para los comandos del jugador y la extendemos para implementar nuevos comandos sin modificar las clases existentes.
![alt text](image-40.png)

Y las correspondientes clases que reemplazarán luego a los métodos en la clase *Juego* 
![alt text](image-39.png)


## Liskov Substitution Principle (LSP)
Debido a que no se han utilizado subclases, no hay cambios notables que haces. Sin embargo, como ya se utilizan interfaces podemos sustituir implementaciones fácilmente

## Interface Segregation Principle (ISP)

Dividimos las interfaces grandes en interfaces más específicas y pequeñas.

Como ya existe IHabitación y IJugador, creamos IInventario 

![alt text](image-41.png)


## Dependency Inversion Principle (DIP)
Usamos interfaces o clases abstractas para definir dependencias y luego implementamos estas abstracciones.

Implementamos las abstracciones creadas con OCP para agregar los comandos
![alt text](image-42.png)

Y ejecutar los comandos 
![alt text](image-43.png)

## Test 

Siguen funcionando los test
- JugadorTest
![alt text](image-44.png)
- HabitacionTest
![alt text](image-45.png)


2.  Implementar Jacoco para medir la cobertura de código del proyecto del juego y asegurarse de que las pruebas cubran un alto porcentaje del código

![alt text](image-46.png)

Se puede ver que Juego tiene poca cobertura y esto debido a que no se implementaron pruebas de ingreso de datos, sin embargo se pueden agregar pruebas para mejorar la cobertura

![alt text](image-47.png)

Se observa como mejoró la cobertura
![alt text](image-48.png)