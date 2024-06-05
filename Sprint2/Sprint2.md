
# Sprint 2

Se actualizan las clases para los nuevos requisitos

## Clase Objeto

![alt text](image-16.png)

Atributos:
- Nombre

## Clase Acertijo

![alt text](image-17.png)
Atributos:
- Pregunta
- RespuestaCorrecta
Métodos:
- Resolver: validar la respuesta
- getPregunta: obtener la pregunta

## Clase Habitación
 Se actualizan los atributos agregando objetos y acertijos con sus respectivos getters y setters.
 ![alt text](image-19.png)

## Clase Jugador

Se actualiza la clase.
![alt text](image-18.png)

Metodo addObject: ahora se requiere por parámetro un Objeto
useObject: busca en el inventario de objetos y quita el objeto del arreglo
resolverAcertijo: intenta resolver el acertijo

## Clase Juego

Se actualiza la lógica del juego para poder llenar las habitaciones con sus respectivos objetos y acertijos según sean par o impar
![alt text](image-20.png)

Mostramos las opciones según la habitación 
![alt text](image-21.png)

Según la primera palabra del comando ingresado, luego busca en la habitación actual, si es recoger objeto, usar objeto y usando split obtiene que objeto vamos a utilizar; sino resolver que intenta resolver el acertijo devolviendo el resultado de procesar la elección

![alt text](image-22.png)

## Tests

### Clase Objeto
Crea un objeto de nombre llave y valida que retorne su nombre
![alt text](image-23.png)

### Clase Acertijo
Se crea un acertijo, se valida la pregunta y la respuesta correcta e incorrecta
![alt text](image-24.png)

## Cambios en tests

Debido a que se agregaron objetos y acertijos se necesita cambiar los tests, además de agregar otros nuevos

## Test Jugador
Para validar agregar un objeto, quitarlo y resolver un acertijo
![alt text](image-26.png)

Todo lo demás sigue funcionando 
![alt text](image-27.png)

## Test Habitación
![alt text](image-28.png)

## Test Juego
![alt text](image-29.png)