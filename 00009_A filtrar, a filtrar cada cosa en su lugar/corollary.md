¡Muy bien! :raised_hands: Ahora ya sabemos cómo filtrar una lista. En criollo, aprendimos a recorrer una lista y obtener los elementos que cumplen una condición determinada. En este caso obtuvimos una nueva lista con los balances que presentaban una ganancia positiva. :moneybag:

¡El filtrado también es un recorrido muy común! Por lo general, se ve así:

```python
def filtrar_algo(lista):
  nueva_lista = []
  for elemento in lista:
    if cumple_condicion(elemento):
      list.append(nueva_lista, elemento)
  return nueva_lista
```
