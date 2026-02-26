# Ejercicios - Semana 03 - Infraestructuras Paralelas

- Nombre : kevin steven trujillo riascos
- Codigo: 1830771-3743
- correo: kevin.steven.trujillo@correounivalle.edu.co

---


## Ejercicio 01

En este primer ejercicio vamos a usar la herramienta valgrind para valorar
que tantos accesos hacen a la memoria cache cuando se ejecuta un programa

## ejercicio 02 

En el segundo ejercicio, analizamos el impacto del orden de los ciclos (Lazos Anidados) en la multiplicación de matrices o el recorrido de arreglos bidimensionales.

## ejercicio 03

Este ejercicio mide el impacto en el rendimiento al pasar datos de gran tamaño (200 KB) a una función de dos formas distintas:

Por Valor: Se crea una copia física de toda la estructura en el stack.

Por Referencia (Puntero): Solo se envía la dirección de memoria (8 bytes).

Al ejecutar 100.000 iteraciones, el programa nos muestra que la copia constante de datos ralentiza drásticamente la ejecución comparada con el acceso directo vía punteros.

## responder

### por que de acuerdo al codigo es mas costoso pasar argumentos a las funciones por valor que por referencia?

Según el código, el costo superior del paso por valor se debe a:

Sobrecarga de CPU: Copiar 200,000 bytes requiere miles de ciclos de reloj por cada llamada, mientras que copiar un puntero de 8 bytes es casi instantáneo.

Uso de Memoria (Stack): El paso por valor satura la pila de ejecución con duplicados innecesarios,