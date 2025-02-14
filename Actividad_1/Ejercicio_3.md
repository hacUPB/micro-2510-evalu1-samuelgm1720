1. ¿Qué es un programa y dónde se almacena?
Un programa es un conjunto de instrucciones que una computadora ejecuta. Se guarda en el disco duro o SSD y, al ejecutarse, se carga en la RAM.

Si pongo un comentario en un programa como: //variable tipo contador. ¿Dónde se almacena dicho comentario?
Un comentario en el código solo existe en el archivo fuente (memoria secundaria). No se almacena en la RAM ni en el ejecutable

¿Dónde se almacena una variable?

**Variables locales**: En la pila (stack) dentro de la RAM, mientras la función está activa.
**Variables globales y estáticas**: Se almacenan en la sección de datos del programa, en la memoria RAM, y permanecen mientras el programa esté en ejecución.
**Variables dinámicas**: Se almacenan en el montículo (heap), que también está en la RAM, y permanecen hasta que se liberan.