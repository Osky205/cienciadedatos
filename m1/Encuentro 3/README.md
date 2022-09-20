# Estructuras de Control

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1r2eZMzhAyC6TQvStuiJu0cXDJ4EceXny/view?usp=sharing)

## Estructuras de control condicionales

Las estructuras de control condicionales son muy útiles para decidir qué sección de código se ejecuta dado el valor de las variables (llamado estado del programa) en un determinado momento.

### IF

Con el comando if (sí en inglés) ejecutamos cierta sección de código, si y sólo si, cierta condición se cumple. Se usa de la siguiente manera:

```python
if condicion:
  algunCodigo
```

## Estructuras de control iterativas
Las estructuras de control iterativas nos ayudan a ejecutar una misma sección de código varias veces, mientras se cumpla una condición o por cada valor de una lista de valores. Esto nos permite ejecutar el mismo bloque de código cambiando los valores en cada ejecución.

### FOR

Usaremos for (para) para los casos en los que queremos ejecutar varias veces el mismo bloque de código para una lista de valores.

El comando for necesita de dos elementos: un objeto que pueda ser iterable, como una lista, y una variable auxiliar que será la que lleve el valor actual de la lista de valores, para esa ejecución en particular.

```python
for item in lista:
  algunCodigo
```

## Funciones



<img src="https://camo.githubusercontent.com/d4ab80aae7ca83650bae0c68e5e585e7df43a07747813b78f63d5e4a4322cf1f/68747470733a2f2f736361757365792e6769746875622e696f2f6173736574732f696d616765732f746f617374657246756e6374696f6e4469616772616d2e6a7067" width="600px">
---

## Ejercicios


- Calculen la suma de los primeros 200 números pares.

- Crea un condicional que si dos números son distintos, imprima "son distintos". (distinto es !=)

- Crea una lista de amigos/as/es y crea una iteración que permita contar la cantidad de personas en la lista.

- Crea una lista de números y una iteración que imprima en cada caso el número multiplicado por -1
