# Reto-09

## 1. Desarrollar un algoritmo que calcula el promedio de un arreglo de reales.

```python  
  # Aqui ingresamos la cantidad de datos que vamos a promediar
cantidad_valores = int(input("Cantidad de valores a promediar: "))

# Creamos una lista para guardar los valores que ingresamos
lista_valores = []

# Pedimos que ingresen los valores uno por uno
for indice in range(cantidad_valores):
    valor_real = float(input("Ingrese el valor " + str(indice + 1) + ": "))
    lista_valores.append(valor_real)

# Iniciamos la variable para la suma total en 0
suma_total = 0

# Aqui se suman todos los valores de la lista
for valor in lista_valores:
    suma_total += valor

# Verificamos que la cantidad sea mayor a cero para evitar división por cero
if cantidad_valores > 0:
    promedio = suma_total / cantidad_valores
    print("El promedio es:", promedio)
else:
    print("No hay valores para calcular el promedio.")
```
## 2. Desarrollar un algoritmo que calcule el [producto punto](https://www.cuemath.com/algebra/dot-product/) de dos arreglos de números enteros (reales) de igual tamaño# Paso 1: Ingresar la cantidad de elementos en los arreglos
```python
# Paso 1: Aqui ingresamos la cantidad de elementos en los arreglos
cantidad_elementos = int(input("Ingrese la cantidad de elementos en los arreglos: "))

# Paso 2: Crear las listas para almacenar los dos arreglos
arreglo_1 = []
arreglo_2 = []

# Paso 3: Ingresamos los elementos del primer arreglo
print("Ingrese los elementos del primer arreglo:")
for i in range(cantidad_elementos):
    numero = float(input("Ingrese el valor " + str(i + 1) + " del arreglo 1: "))
    arreglo_1.append(numero)

# Paso 4: Ingresa los elementos del segundo arreglo
print("Ingrese los elementos del segundo arreglo:")
for i in range(cantidad_elementos):
    numero = float(input("Ingrese el valor " + str(i + 1) + " del arreglo 2: "))
    arreglo_2.append(numero)

# Paso 5: Aqui se calcula el producto punto
producto_punto = 0
for i in range(cantidad_elementos):
    producto_punto += arreglo_1[i] * arreglo_2[i]

# Paso 6: Se muestra el resultado
print("El producto punto de los dos arreglos es: " + str(producto_punto))
```
## 3. Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.

```python
# Ingresamos el tamaño del arreglo
cantidad = int(input("Ingrese la cantidad de elementos de los arreglos "))
# Se crea el arreglo
arreglo = []
# Se llena el arreglo
for n in range(cantidad):
    numero = int(input("Ingresar el número " + str(n + 1) + ": "))
    arreglo.append(numero)
# Creamos un nuevo arreglo para los números distintos de cero
no_ceros = []
# Se cuenta cuántos ceros hay
contador_ceros = 0
for n in range(cantidad):
    if arreglo[n] != 0:
        no_ceros.append(arreglo[n])
    else:
        contador_ceros = contador_ceros + 1
# Agregaos los ceros al final
for n in range(contador_ceros):
    no_ceros.append(0)
# Se muestra el resultado
print("El arreglo con los ceros al final es: " + str(no_ceros))
```
## 4. Revisar que son los algoritmos de *sorting*, entender *bubble-sort* ([enlace](https://www.geeksforgeeks.org/bubble-sort/) a implementación).
- ¿Qué son los algoritmos de sorting?
Los algoritmos de sorting (ordenamiento) son procedimientos diseñados para organizar elementos de una lista o arreglo según un criterio específico, usualmente de menor a mayor o de mayor a menor. Son fundamentales en programación porque facilitan tareas como la búsqueda de datos, visualización ordenada y procesamiento eficiente.
- ¿Qué es Bubble Sort?
El Bubble Sort es uno de los algoritmos de ordenamiento más simples. Su funcionamiento se basa en comparar pares de elementos adyacentes y intercambiarlos si están en el orden incorrecto. Este proceso se repite hasta que toda la lista esté ordenada.
