# M0 Introduccion a Python

## Indice:

## Tipos de Datos



### Enteros

```python
31
```

```python
n = 35
```

Usemos nuestra primer funcion basica de python, la funcion `type` nos devuelve el tipo de variable.

```python
type(n)
```

### Decimales 


```python
31.7
```

```python
d = 3.5
```

```python
type(d)
```

### Cadenas de caracteres

```python
hola
```

```python
'hola'
```

```python
s = 'hola'
```

```python
type(s)
```

### Booleanos

```python
true
```

```python
b = true
```

```python
type(b)
```


Que pasa si uso comillas?

```python
b = 'true'
```

```python
type(b)
```
### Operaciones
 
Muchas veces los datos por si solos carecen de sentido, y tenemos que aplicarle operaciones para poder obtener información de ellos. 
 
En _python_ podemos hacer varias operaciones entre dos datos, dependiendo de sus tipos.
 
Operación | Operador | Tipo de datos | Ejemplo | Resultado
----------|----------|---------------|---------|---------
Suma | + | int, float, bool, str | 3 + 4 | 7
Resta | - | int, float, bool | 5 - 10 | -5
Multiplicación | \* | int, float, bool, str | 9 \* 8 | 72
División | / | int, float, bool |  10 / 5 | 2.0
Módulo | % | int, float, bool | 10 % 3 | 1
Cociente | // | int, float, bool | 105 // 10 | 10
Potencia | \*\* | int, float, bool | 2 \*\* 5 | 32
 
¿Pueden adivinar el resultado de las siguientes operaciones y de qué tipo son los mismos?

### Funciones

```python
def cuadrado(x):
    return x*x
``` 

```python
cuadrado(6)
```


```python
def cuadrado(x):
    return x**2
```
 
```python
cuadrado(6)
```

```python
def raiz(x):
    return x**(1/2)
``` 

```python
def promedio(x1,x2):
    return (x1+x2)/2
``` 


## Estructuras de Datos



[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1PfpljcOVYRQDEZBxM-Hgyj98BU-65MXB/view?usp=sharing)

### Listas

```python
milista = ['uva','mandarina', 'kiwi']
```
### Diccionarios

```python
midiccionario = { 'frutas' : ['uva','mandarina', 'kiwi'], 'comidas' : ['milanesa','pizza','asado'] } 
```

## Estructuras de Control


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1r2eZMzhAyC6TQvStuiJu0cXDJ4EceXny/view?usp=sharing)

### Estructuras de control condicionales

Las estructuras de control condicionales son muy útiles para decidir qué sección de código se ejecuta dado el valor de las variables (llamado estado del programa) en un determinado momento.

#### IF

Con el comando if (sí en inglés) ejecutamos cierta sección de código, si y sólo si, cierta condición se cumple. Se usa de la siguiente manera:

```python
if condicion:
  algunCodigo
```

### Estructuras de control iterativas
Las estructuras de control iterativas nos ayudan a ejecutar una misma sección de código varias veces, mientras se cumpla una condición o por cada valor de una lista de valores. Esto nos permite ejecutar el mismo bloque de código cambiando los valores en cada ejecución.

#### FOR

Usaremos for (para) para los casos en los que queremos ejecutar varias veces el mismo bloque de código para una lista de valores.

El comando for necesita de dos elementos: un objeto que pueda ser iterable, como una lista, y una variable auxiliar que será la que lleve el valor actual de la lista de valores, para esa ejecución en particular.

```python
for item in lista:
  algunCodigo
```

## Funciones

<img src="https://camo.githubusercontent.com/d4ab80aae7ca83650bae0c68e5e585e7df43a07747813b78f63d5e4a4322cf1f/68747470733a2f2f736361757365792e6769746875622e696f2f6173736574732f696d616765732f746f617374657246756e6374696f6e4469616772616d2e6a7067" width="600px">

Las funciones son lineas de código, enfocadas en resolver un problema específico. En python podemos crear nuestras propias funciones usando la siguiente sintaxis:

```python
def nombrefuncion(panblanco):
  *codigo*
  *codigo*
  ...
  *mas codigo*
  return tostada
```

Notar nuevamente los dos puntos `:` y la identacion (espacio desde el margen).

---


## Clases


## Librerias

