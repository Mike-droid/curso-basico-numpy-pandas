# Curso Básico de Manipulación y Transformación de Datos con Pandas y NumPy

## Librerías de manipulación de datos con Python

### ¿Por qué NumPy y Pandas?

Requisitos previos:

- Matemáticas
- Python
- Jupyter Notebooks

¿Para qué sirven *Numpy* y *Pandas*?

[Numpy](https://numpy.org/) sirve para el *calculo numérico_ y _manejo de arrays*. Es muy veloz, optimiza el almacenamiento en memoria. Es muy poderosa.
[Pandas](https://pandas.pydata.org/docs/getting_started/index.html) sirve para la *manipulación y análisis de datos*. Es veloz, requiere poco código, soporta múltiples formatos de archivos y ordena los datos de forma inteligente. Es muy poderosa.

```python
import numpy as np
import pandas as pd
```

## NumPy

### NumPy Array

El array es el **principal objeto** de numpy. Con este ocurre toda la magia. Es una estructura ordenada, indexada, con cabecera.

```python
import numpy as np

a = np.array([1,2,3])
```

[Archivo de clase 2 en jupyter notebook](https://colab.research.google.com/drive/1Pw4mJovDm_atbbcXaGogP1H-LZPXNh3R?usp=sharing)

### Tipos de datos

Numpy soporta muchos tipos de datos en sus arrays para tus necesidades. Sin embargo, el array de numpy **solo debe tener un tipo de dato en su array**. Si mezclamos, por ejemplo, entero64 con string, se perdería la eficiencia en memoria.

[Archivo de la clase 3 - tipos de datos](https://colab.research.google.com/drive/17FoT28JrNpHhqo4xwBw5EM0exBIdkXnG?usp=sharing)

### Dimensiones

scalar: dim = 0 Un solo dato o valor

vector: dim = 1 Listas de Python

matriz: dim = 2 Hoja de cálculo

tensor: dim > 3 Series de tiempo o Imágenes

[Archivo de clase 4- dimensiones](https://colab.research.google.com/drive/13d8QL5crJH13RSEQDH8401CRIG6fgyLy?usp=sharing)

### Creando arrays

[Archivo de la clase 5 - creando arrays](https://colab.research.google.com/drive/1hDJQxPY9-p8czNGtAHf72Hc1Ip3DZkM3?usp=sharing)

### Shape y Reshape

[Archivo de la clase 6 - shape y reshape](https://colab.research.google.com/drive/1o_HHHrBp5ozzg5sYECHMaWLdy-Te1iKT?usp=sharing)

### Funciones principales de Numpy

[Archivo de la clase 7 - funciones principales](https://colab.research.google.com/drive/1wAMM3mHMQS_aAL8WwZAVPW8QV9aoEnax?usp=sharing)

### Copy

Es común tener errores en la programación con los arreglos, ya que puede que, sin querer, modifiquemos el array original en vez de la copia. Pero la función copy de numpy nos ayuda a prevenir estos errores.

[Archivo de la clase 8 - copy](https://colab.research.google.com/drive/10GWNUutdrZRjonVZtAquTzRVL7VU3-8s?usp=sharing)

### Condiciones

[Archivo de la clase 9 - Condiciones](https://colab.research.google.com/drive/1BQBCgdxn3Au7ZmYOAupF3nzNn86qr4OD?usp=sharing)

### Operaciones

[Archivo de la clase 10 - Operaciones](https://colab.research.google.com/drive/1tdbvSU9wHr8c3d9iGEqG-J5SCoUeIGIF?usp=sharing)

## Quiz

- ¿Qué línea de código genera este array de NumPy?: `array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])` -> `np.arange(0, 10)`
- ¿Cómo se asigna de forma correcta al array_copy una copia de el array arr? -> `arra_copy = arr.copy()`
- ¿Qué número retorna esta sentencia?: `np.array([[1,2,3],[4,5,6],[7,8,9]]).ndim` -> 2
- ¿Con cuál de las siguientes opciones se obtiene el siguiente array de NumPy?: `array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])` -> `np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9] ])`

## Pandas

### Series y DataFrames en Pandas

Pandas maneja 2 objetos principales:

1. Pandas series(muy similar a un array 1D o vector)
2. Pandas dataframe (básicamente una matriz con índices)

[Archivo de la clase 11- series y dataframes](https://colab.research.google.com/drive/1C5CbZ9L6vLI0WGeM_HkjFlfMYOglEcOQ?usp=sharing)

### Leer archivos CSV y JSON con Pandas

[Archivo de la clase 12 - leer archivos csv y json con pandas](https://colab.research.google.com/drive/1WcQORM-mkHfoDwhFrF0ESNW8yv-wOUav?usp=sharing)

### Filtrado con loc y iloc

[Archivo de la clase 13 - loc e iloc](https://colab.research.google.com/drive/1WcQORM-mkHfoDwhFrF0ESNW8yv-wOUav?usp=sharing)

### Agregar o eliminar datos con Pandas

[Archivo de la clase 14 -agregar y eliminar datos](https://colab.research.google.com/drive/1o8lFuS7uGA9c1HOxKHcEAZWMJLw0D8zX?usp=sharing)

### Manejo de datos nulos

[Archivo de clase 15 - manejo de datos nulos](https://colab.research.google.com/drive/1J9KiXpdvT7BfsUyi4WesF_fzugcgRySL?usp=sharing)

### Filtrado por condiciones

[Archivo de la clase 16 - filtrado por condiciones](https://colab.research.google.com/drive/1-_NsUjqS_VeO3jAzv9x66hGuzd2G_EEz?usp=sharing)

### Funciones principales de Pandas

[Archivo de la clase 17 - funciones principales de pandas](https://colab.research.google.com/drive/1UJMTTL0ijdMHQsgNhy5A0MNeCezTtowA?usp=sharing)

### groupby

[Archivo 18 - groupby](https://colab.research.google.com/drive/16c_qxqeo69wXoPVE5yBlUXGPT3CCUXwC?usp=sharing)

### Combinando DataFrames

- [Documentación de Pandas para join](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.join.html?highlight=join#pandas.DataFrame.join)
- [Documentación de Pandas para concat](https://pandas.pydata.org/docs/reference/api/pandas.concat.html?highlight=concat#pandas-concat)
- [Documentación de Pandas para merge](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.merge.html?highlight=merge#pandas.DataFrame.merge)

### Merge y Concat

[Archivo 20 - merge y concat](https://colab.research.google.com/drive/1HuozMHjxu85s44lUdt_GKKW2IFHmAgZt?usp=sharing)

### Join

Lo mismo que en el archivo 20.

### Pivot y Melt

[Artículo en Platzi](https://platzi.com/clases/2912-pandas-numpy/47995-pivot-y-melt/)

[Archivo de la clase 22 - pivot y melt](https://colab.research.google.com/drive/1ukPX1nxRA3_bkLC8YaSy_C2veTzm_qDY?usp=sharing)

### Apply

[Archivo 23 - apply](https://colab.research.google.com/drive/1-VA2UU13ltbP16xi4jxsmcEcovUc5AfD?usp=sharing)

## Quiz

- ¿Cuál es el parámetro para especificar el delimitador del archivo en pd.read_csv()?: `sep`
- De esta manera se pueden eliminar filas con valores nulos de un DataFrame en Pandas: `df.dropna()`
- ¿Con cuál de las opciones se ordenan los datos del DataFrame df_books de manera descendente por la columna year?: `df_books.sort_values('Year', ascending=False)`
- ¿Cuál comando imprime las n primeras filas de un DataFrame de Pandas?: `head`

