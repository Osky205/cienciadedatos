# Estructuras de Control

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
