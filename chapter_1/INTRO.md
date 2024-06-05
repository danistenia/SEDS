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

## Modularity

El arte de modular es de dividir un sistema grande en pequeñas partes. Un ejemplo simple es pensar en un proyecto de ML, cada etapa puede ser una etapa o modulo distinto, ejemplo: Collect data, explore data, clean data and Visualize Data.

## Readability

Cuando escribes un código es importante que la persona que sigue a ti pueda ser capaz de leerlo y entenderlo. Cosas que ayudan a que el código sea más legible es escoger buenos nombres, remover código que no se utiliza y escribir documentación del código. 

### Standards and conventions

Para los standards es bueno adherirse y para eso la fuente maestra o referencia que se puede tomar es el PEP8. Si queremos cumplir con el standard podemos ocupar helpers como linters. Otro formateador automático es Black que es una librería que te formatea todo automáticamente.

### Names

Es necesario escoger nombres de funciones, variables, clases que ayuden a entender o sean auto-explicativas.

### Clean it up

Otra forma de hacer que tu código sea más entendible es que luego de hacer una función la limpies completamente de las cosas que no sirven y no aportan. Eliminar también los prints de la función que no ayudan, como standard es mejor ocupar un debugg que eso. 
Si se tienen buenos standards eso hace que todo el resto tenga buenos standards. (La teoría de los vidrios rotos)
Refactoring puede ser una opción para tu código y qué significa? Es modificar tu código sin que cambie su comportamiento. Los Tests son vitales para el funcionamiento del código. 

### Documentation

La documentación puede tener muchos aspectos puede ir de documentar una línea, generar un docstring y tener un README en github como todo el proyecto explicando el funcionamiento del paquete.

## Performance

El performance del código también es importante y se mide en términos de rapidez y memoria. Siempre hay estructuras de datos que peuden hacer tus algoritmos más eficientes. 

## Robustness

La idea es que tu código sea robusto, es decir, que sea capaz de correr de principio a fin. Además, debiese ser capaz de leer y sabes cuando los inputs son incorrectos. Tu código puede ser más robusto para manejar errores, loggings y escribir buenos Tests.

### Errors and Logging

Tu código, si es que es robusto, no debiese manejarse de forma innesperada si es que recibe inputs que no son. Tu debes decidir si tu código debiese morir o no. La idea es si decides seguir con errores de manera silenciosas, también debiese existir un warning, pero seguir con el código y esto depende como tú lo decidas.

### Testing

Software engineers tiene dos formas de testear.

1. User testing: Que el usuario pruebe la funcionalidad. 
2. Automated testing: Es mandar un input de prueba y esperar que el resultado sea igual a lo que uno espera. (Esto es automatizado, al parecer)
3. Unit tests: Se prueba solamente una función.
4. End to end tests: Prueban un proyecto entero.
5. Integration tests: Prueba un chunk de código que tiene muchas funciones, pero que aún así es pequeño en función del proyecto completo.

Si tu código funciona en tu máquina no quiere decir que vaya a funcionar en la máquina de alguien, por lo tanto, una buena práctica es que alguien pueda correr tus pruebas y sepa si tu código le funciona en su máquina o entorno.
Un consejo para partir es con un código que uno tenga y que siempre se cae en algun punto es poner un test en ese error para que no vuelva a suceder.

## Resources

1. The Pragmatic Programmer, 20th anniversary edition. (David Thomas and Andrew Hunt)
2. A Philosophy of Software Arquitecture by John Ousterhout.