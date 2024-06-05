# Analyzing Code Performance

1. Lo primero es lo primero que tu código funcione. Cualquier optimización o tuneo que hagamos tiene que ser que tu código ya funcione.
2. Preguntate si es importante que la rapidez del performance ayude en algo. Ejemplo si es para un cliente interno o externo. Si esto no cumple ningun principio entonces probablemente hacer un boost en el performance no ayude mucho.

Teniendo en cuenta estos principios es importante y empezando a dar los primeros pasos es saber dónde está el cuello de botella, es decir, saber cual es la parte más lenta de tu código. Una vez que puedas recolectar esta data puedes tomar decisiones. Es importante darle un timing o "timear" tu código. 
SUPER IMPORTANTE: Optimización prematura es la raíz de todos los problemas así que es importante no optimizar nada sin saber donde están los errores o sin saber qué problemas de optimización tiene el código.

## Methods to Improve Performance

Se definirá como código performante como aquel que reduce los recursos computacionales al mínimo para hacerlo o ejecutar la tarea lo más rápido posible. Existen distintas formas de hacer o aumentar el performance de tú codigo:

1. Elegir bien el algoritmo: La forma de buscar, iterar y las funciones elegidas afecta mucho el performance.
2. Elegir bien las estructuras: Listas, tuplas o dictionaries, buscar un elemento en un dictionary es mucho más rapido que en una lista.
3. Using built-in functions: Python tienen funciones por defecto que usualmente resuelven todos los problemas que uno conoce, la idea es conocerlas e ir ocupándolas.
4. Compiling functions: Hay librerías como Cython, Numba y Pypy que son capaces de ejectuar código en C y ocupar a python como un lenguaje de bajo nivel.
5. Asynchronus code: Esto no lo entendí.
6. Programación distribuida: Hay una formas de distribuir los cálculos, esto es como Dask. 


### Resources

Si se quiere profundizar en performance se tiene este libro: High Performance Python - Mucha Gorelick (2020)

## Timing Your Code