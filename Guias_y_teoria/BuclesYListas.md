# Bucles y Listas

* lo que empieza por $ son variables

## Bucles y demás

* Bucle while desde "start" hasta "end"
  
```python
$varName = $start
while $varName < $end:
    #El codigo que sea (podemos usar el valor de la variable $varName)
    $varName = $varName +1
```

* Bucle for desde "start" hasta "end"

```python
for $varName in range($start, $end):
    #El codigo que sea (podemos usar el valor de la variable $varName)
```

## LISTAS

* Son conjuntos de elementos (todos del mismo tipo ej: int) y los valores van entre []
  
Ejemplo de lista:

```python
$lista = [$elemento0, $elemento1]
```

Uso basico:

* conseguir elemento en una posicion "Pos" especificada

```python
$lista[pos] -> elementoPos
```

* escribir un valor "Val" en una posicion "Pos" especificada

```python
$lista[pos] = Val
```

### Funciones interesantes

append() añade el elemento especificado al final de la lista

```python
$lista.append($elemento2)
```

remove() elimina el primer elemento con valor especificado

```python
$lista.remove($elemento1)
```

sort() ordena la lista de la manera mas "obvia" (por valor o por orden alfabetico)

```python
$lista.sort()
```

Bucle for para recorrer una lista "list"

```python
for $varName in $list:
    #El codigo que sea (podemos usar el valor de la variable $varName)
```

* Podemos hacer cosas interesantes con la lista que queremos recorrer como por ejemplo ordenarla antes de recorrerla
  
  * una opcion seria:
  
    ```python
    $list.sort()
    for $varName in $list:
        #El codigo que sea (podemos usar el valor de la variable $varName)
    ```

  * Pero podemos aprovechar espacio y hacerlo dentro del for:
  
    ```python
    for $varName in sorted $list:
        #El codigo que sea (podemos usar el valor de la variable $varName)
    ```

## Diccionarios: Lista de parejas (clave, valor)

* Tienen un nombre y los valores van entre {}

Ejemplo de diccionario:

```python
$diccionario = {$clave0 : $valor0, $clave1 : $valor1}
```

### Funciones interesantes

get(): Especificamos una clave y nos devuelve el valor asociado

```python
$diccionario.get($clave0) -> $valor0
```

keys(): Devuelve una lista con todas las claves del diccionario

```python
$diccionario.keys() -> [$clave0, $clave1]
```

values(): Devuelve una lista con todos los valores del diccionario

```python
$diccionario.values() -> [$valor0, $valor1]
```

items(): Devuelve una lista con todas las parejas clave valor del diccionario.

* las parejas son realmente listas y se comportan como tal, es decir la funcion devuelve una lista de listas

```python
$diccionario.items() -> [[$clave0, $valor0], [$clave1, $valor1]]
```

Recorrer diccionarios tiene mas "miga" ya que al ser parejas podemos recorrer solo las claves, solo los valores o ambos

* Recordamos que podemos de la misma manera usar el sorted para obtenerlas en orden

* Recorrer solo claves:

```python
for $clave in $diccionario.keys()
    #El codigo que sea (podemos usar el valor de la variable $clave)
```

* Rrecorrer solo valores

```python
for $valor in $diccionario.values()
    #El codigo que sea (podemos usar el valor de la variable $valor)
```

* Rrecorrer las parejas

```python
for $clave, $valor in $diccionario.items()
    #El codigo que sea (podemos usar el valor de la variable $clave y $valor)
```

## Funciones y librerias extras

* La lista que usaremos para los ejemplos

```python
$lista = [$elemento0, $elemento1, $elemento2]
```

sum(): Suma todos los elementos de la lista que le pasemos como parametro y nos devuelve el resultado

```python
sum($lista) -> $elemento0 + $elemento1 + $elemento2
```

choice() (de la libreria random) recibe una lista y nos devuelve un elemento aleatorio de la lista

```python
choice($lista) -> $elementoK (siendo K un numero random de 0 a 2 en este caso)
```

sample() (de la libreria random) recibe una lista y nos devuelve una lista de n elementos (n especificado por nosotros) aleatorios de la lista
    * Recordar que pueden repetirse los elementos

```python
sample($lista, $N) -> [$elementoK_0 ... $elementoK_(n-1)]
```

Imprimir con formato

* El texto ha de tener {} donde queramos insertar alguna variable (numeros, caracteres, strings...)

* Pondremos un punto y format()

* Dentro del parentesis de format() los valores en orden de aparicion en el texto original

```python
print("Aqui ira el primer valor (string) {}, aqui ira el segundo (numero) {}".format("Hola", 5))
```

Intercalar strings

* Usaremos join() con el formato:

```python
$listaDeStrings = [$string0, $string1, $string2]
"T1".join($listaDeStrings) -> ($string0 "T1" $string1 "T1" $string2)
```
