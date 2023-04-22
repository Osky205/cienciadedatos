
# Encuentro 3

Notebook: https://drive.google.com/file/d/1iN6sE5KYaShL_D-lD7_RLqjOCH8sQx7Z/view?usp=sharing

## Dummies

Necesitamos pasar la variables (columnas) categoricas, es decir con valores texto, a valores numericos. 

Vamos a usar la siguiente tecnica: 

```
0 = No
1 = Si
```
## Apply

Es un metodo que tienen las columnas que nos permiten aplicar una funcion cualquiera, a todos los elementos de la columna:

Imaginemos que necesitamos crear una nueva columna en una tabla a partir de la columna `precio`. La nueva columna es el precio en dolares.

```python

def mifuncion(x):
    return x/300
    
nueva_columna=tabla.precio.apply(mifuncion)
````
