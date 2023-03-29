Así como podíamos hacer mapeos utilizando listas por comprensión, también podemos hacer filtrados. :open_hands:

Imaginemos que tenemos la función `mayores_a_5` que dada una lista de números nos retorna una nueva con aquellos que son mayores a 5:

``` python
def mayores_a_5(numeros):
  mayores = []
  for numero in numeros:
    if numero > 5:
      list.append(mayores, numero)
  return mayores
```

Otra manera de definirla sería haciendo:

``` python
def mayores_a_5(numeros):
  return [numero for numero in numeros if numero > 5]
```

Esta comprensión es muy parecida a las que vimos anteriormente: es una **expresión** escrita entre corchetes que incluye un mapeo, un elemento y una secuencia. Sin embargo, también tiene una cuarta sección `if` que introduce una condición: solo los elementos que la satisfagan se incluirán en la lista resultante. En otras palabras, las listas de comprensión en realidad pueden tener cuatro partes:

- una transformación de elementos;
- un nombre para cada elemento de la secuencia;
- una referencia a la secuencia;
- una condición opcional.

```python
[ alguna_transformación(elemento) for elemento in secuencia if cumple_condicion(elemento)]
```

¡Ahora es tu turno!

> Redefiní la función `afortunados` para que haga lo mismo pero utilizando listas por comprensión.