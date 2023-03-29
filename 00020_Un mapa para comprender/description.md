En el ejercicio anterior hicimos un mapeo utilizando `for...in`. En Python contamos con otras formas de hacer eso, ¡las listas por comprensión! :star_struck:

Veamos cómo funcionan, si a partir de una lista de strings quisieramos obtener una lista con los largos de cada uno, podríamos definir:

``` python
def largos(palabras):
  largos = []
  for palabra in palabras:
    list.append(largos, len(palabra))
  return largos
```

Sin embargo, también podríamos hacerlo de esta manera utilizando listas por comprensión:

``` python
def largos(palabras):
  return [len(palabra) for palabra in palabras]
```

Como ves, las listas por comprensión son una forma compacta de hacer iteraciones simples. Están escritas entre paréntesis y, en su forma más simple, deben contener al menos tres partes:

- una transformación de elementos;
- un nombre para cada elemento de la secuencia;
- y una referencia a una secuencia.

```python
[alguna_transformación(elemento) for elemento in secuencia]
```

:fast_forward: Podés pensarlas como un atajo a un recorrido de mapeo. Pero lo mejor es que las comprensiones, a diferencia de la estructura de control `for..in`, son expresiones, lo que permite usarlas cada vez que se espera un valor :open_mouth: en un `retorno`, en una asignación de variable, como un argumento de invocación de función o incluso en la consola:

```python
ム[ 1930 + 10 * decada for decada in range(0, 10) ]
[1930, 1940, 1950, 1960, 1970, 1980, 1990, 2000, 2010, 2020]
```

> Redefiní la función `meses` para que haga lo mismo que antes pero utilizando listas por comprensión.