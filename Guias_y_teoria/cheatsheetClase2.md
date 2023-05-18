# Clase 2: Control de flujo en Python

## Condicionales (if-else)

Permiten ejecutar diferentes bloques de código según una condición.

```python

if condicion:
    # bloque de código a ejecutar si la condición es verdadera
elif condicion2:
    #condicion 2
else:
    # bloque de código a ejecutar si la condición es falsa
```

Por ejemplo, si queremos determinar si un número es positivo o negativo, podemos usar un condicional:

```python

numero = 5

if numero > 0:
    print("El número es positivo")
else:
    print("El número es negativo")
```

En este caso, si la variable numero es mayor que cero, se imprimirá "El número es positivo", de lo contrario se imprimirá "El número es negativo".

## Bucles (for y while)

Los bucles en Python permiten repetir un bloque de código varias veces. Hay dos tipos de bucles en Python: for y while.

El bucle for nos permite iterar sobre una secuencia de elementos, como una lista o una cadena de caracteres. La sintaxis básica es la siguiente:

```python

for elemento in secuencia:
    # bloque de código a ejecutar en cada iteración
```

```python

while condicion:
    # bloque de código a ejecutar mientras la condición sea verdadera
```

Por ejemplo, si queremos imprimir los números del 1 al 10, podemos usar un bucle while:

```python

i = 1

while i <= 10:
    print(i)
    i = i + 1
```