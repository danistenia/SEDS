# Resumen

libro: Software engineering for Data Scientists

## Prefacio

Todo lo que hacemos en ciencia de datos nace en código ya sea un modelo, análisis de datos, procesamiento, etc. Por lo tanto, la importancia de programar bien ayuda en todos los ámbitos de lo que hacemos. 
Buenas prácticas de software engineering son (o por lo menos las más comunes):

- Testing.
- Error Handling.
- Logging.

### Why Python?

Para que tenga el dato anotado de una encuesta de 3.000 Data Scientist 63% ha usado o usa python para resolver problemas de su día a día y el 83% de los entrantes al mundo de ML aprendieron python para meterse dentro del mundo de python.

Por otro lado, para que tampoco se me olvide Tensorflow es de Google y Pytorch es de Meta.

### Recomendaciones de Libros

Para programación más avanzada en Python la autora recomienda: Robust Python by Patrick Viafore.

### Using code examples

Para material complementario, ejercicios, códigos tenemos el github del libro:

https://github.com/catherinenelson1/SEforDS

## Chapter 1: What is Good Code?

Para la autora existen muchas posibles formas de definir qué es un buen código, para ello explicará a través de 5 categorías:

1. Simpicity.
2. Modularity.
3. Readibilty.
4. Performance.
5. Robustness.

Nota: Clean code de Robert C. Martin es una buuena referencia de los principios SOLID.

### Simplicity

Complejidad: Se define como todo aquello a la estructura de un sistema que lo hace dificil de entender y modificar.
Un ejemplo sería que se le hace un cambio a un código y algo pasa y no funciona. Complejo quiere decir cuando no sabes que función arreglar o modificar para mejorar o cambiar una acción.
Se puede hacer el código más conciso y separarlo en pequeñas partes.

#### DRY: Don´t repeat yourself

Ojalá evitar problemas en tus codigos donde tengas que cambiar muchas veces un pequeño pedazo de codigo como las rutas o las credenciales por ejemplo. Por otro lado, si tienes una tarea que se repite muchas veces es mejor hacer una funció y no repetir infinitamente cosas. 

#### Avoid Verbose Code (Código detallado)

Un código demasiado detallado lleva a demasiado detalle innecesario , pero por otro lado también lleva que un código muy corto lleva al problema de poco legible. Por lo tanto, hay que tener un trade off entre algo muy detallado y algo muy corto. La autora recomienda que es un poco mejor agregar un poco de líneas adicionales a tu código en vez de privilegiar algo muy corto.

### Modularity

El arte de modular es de dividir un sistema en pequeñas partes.