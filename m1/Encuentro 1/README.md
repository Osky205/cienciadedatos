# Tipo de datos en python

## Enteros

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

## Decimales 


```python
31.7
```

```python
d = 3.5
```

```python
type(d)
```

## Cadenas de caracteres

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

## Booleanos

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
# Operaciones
 
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

## Funciones

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

