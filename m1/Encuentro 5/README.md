# Pandas, filtrar y visualizar



![Open In Colab](https://drive.google.com/file/d/1PP3mCBeLQeHFsg3Xi36N5VHeqyalThyl/view?usp=sharing)

[Descarga archivo csv](https://drive.google.com/file/d/1vH2ym59HCkPSgt40f5cdy5sTSaz0CFUF/view?usp=sharing)

# Indexado

Como con las listas nos va interesar visualizar solo algunos elementos de nuestra tabla. Empecemos aprendiendo como visualizar alguna columna en particular:


```python
dataframe['nombre_columna']
```

Tambien podemos usar el punto:

```python
dataframe.nombre_columna
```

Esto solo funciona con columnas que no tengan espacios en su nombre.

Si queremos visualizar por ejemplo las 3 primeras filas podemos usar:

```python
dataframe[0:3]
```
O la 3 ultimas:

```python
dataframe[-3:]
```

# Filtrar

Tambien podemos filtrar filas que cumplan cierta condicion. Imagenemos que necesitamos solos las filas que correspondan a encuentros que se realizaron el '2016'.

Esta condicion se escribiria:

```python
data["encuentro_anio"] == 2016
```

Esto devuelve una columna de booleanos, donde se listan si la fila cumple o no la condicion.

A esta columna que no pertenece a nuestra tabla, pero hace referencia a sus filas, la llamaremos *mascara booleana*. 

Vamos a guardar esta informacion en una variable:

```python
mascara=data["encuentro_anio"] == 2016
```

Y para que sirve? Bueno, nos sirve para poder seleccionar de nuestra tabla solo las filas que cumplan la condicion.

Ahora podemos usar la mascara para indexar que filas quiero:

```python
data[mascara]
``` 
Esto que hicimos nos permitio filtrar datos de una tabla, la tabla original sigue intacta, si necesitamos trabajar con la nueva tabla filtrada tenemos que asignarle un nuevo nombre.

```python
data_2016=data[mascara]
``` 

# Funciones de Agregacion:

- .sum() Calcula la suma de todos los elementos de la columna.
- .mean() Calcula el promedio de una columna.
- .min()  Busca el minimo de una columna.
- .max()  Busca el maximo de una columna.

Ahora estamos interesadxs en calcular el promedio de participantes por encuentro en el 2016.

Necesitamos entonces trabajar la tabla filtrada:

```python
data_2016
```

De esta tabla la columna que nos interesa es: `encuentro_participantes` es sobre esta columna que debemos aplicar el promedio:

```python
data_2016['encuentro_participantes'].mean()
```
Piensen como harian usando un 'for' para tener una lista del promedio de participantes para cada año.

# Visualizar



Veamos ahora como realizar graficos en python. Imaginen que tenemos esta lista de valores para los encuentros realizados entres 2010 y 2015:

```python
promedio_participantes= [103, 400, 800, 333, 120,70]
```

Queremos ver un grafico de estos datos para ver como fue cambiando en el tiempo la participacion.

Una de las librerias de python que nos permite realizar graficos muy sencillos es `matplotlib`.

Recordemos que no es necesario generar ningun codigo desde 0, solo utilizamos funciones que debemos importar desde alguna libreria.

```python
import matplotlib.pyplot as plt
```

Esto siempre sera igual! Importamos la libreria usando un alias 'plt' para que sea mas facil llamar a sus funciones.

Veamos la funcion `plot`:

```python
plt.plot(promedio_participantes)
```

Si bien podemos ver los valores, este grafico esta incompleto, no se saben a que año corresponde cada valor. Tampoco se sabe valores de que es lo vemos. Necesitamos agregarle la informacion del eje x (los años):

Sabemos que son los encuentros entre 2010 y 2015 entonces definimos:

```python
años=[2010,2011,2012,2013,2014,2015]
```
```python
plt.plot(años,promedio_participantes)
```

Por ultimos debemos agregar la informacion de cada eje:

```python
plt.plot(años,promedio_participantes)
plt.xlabel('Años del encuentro')
plt.ylabel('Promedio de participantes')
```

Ya nos quedo mucho mejor, tambien podriamos haber usado un grafico de barras. 


```python
plt.bar(años,promedio_participantes)
plt.xlabel('Años del encuentro')
plt.ylabel('Promedio de participantes')
```

Para estos datos, este grafico es mas apropiado, ya que se tiene un valor anual. Una barra por cada año, el grafico anterior sugeria valores intermedios que en realidad desconocemos.
