## Explica la diferencia entre desplazamiento lógico y desplazamiento aritmético con tus propias palabras.

El **desplazamiento lógico** (LSR, Logical Shift Right) mueve los bits de un número hacia la derecha o izquierda, rellenando con ceros en los espacios vacíos. Es útil para operaciones de multiplicación o división por potencias de 2. En cambio, el **desplazamiento aritmético** (ASR, Arithmetic Shift Right) también mueve los bits, pero al desplazar a la derecha, mantiene el bit de signo (el bit más significativo) para preservar el valor negativo o positivo del número. Esto es crucial en operaciones con números con signo.

---

## ¿En qué tipo de aplicaciones sería más útil usar ASR en lugar de LSR?

El **ASR** es más útil en aplicaciones que trabajan con números con signo, como en procesamiento de señales o cálculos matemáticos donde se necesita preservar el signo del número. Por ejemplo, al dividir un número negativo por 2, el ASR asegura que el resultado siga siendo negativo, mientras que el LSR lo trataría como un número positivo, lo que podría llevar a errores en el cálculo.

---

## Explica la diferencia entre `MOV R0, #42` y `MOV R0, R1`.

La instrucción `MOV R0, #42` mueve el valor inmediato **42** al registro **R0**, es decir, asigna directamente el número 42 a R0. En cambio, `MOV R0, R1` copia el valor almacenado en el registro **R1** al registro **R0**. La primera instrucción trabaja con un valor fijo, mientras que la segunda trabaja con el contenido de otro registro.

---

## ¿Qué función tiene la instrucción `MOVS` y cómo difiere de `MOV`?

La instrucción `MOVS` realiza la misma función que `MOV` (mover un valor a un registro), pero además actualiza las **banderas de estado** en el registro CPSR (Current Program Status Register), como la bandera de cero (Z) o negativo (N). Esto es útil cuando se necesita verificar el resultado de la operación inmediatamente después de mover el valor, como en comparaciones o condiciones.

---

## ¿Por qué se utiliza la instrucción `MOVT` en combinación con `MOVW`?

La instrucción `MOVW` (Move Wide) mueve un valor de 16 bits a un registro, pero solo afecta a los 16 bits menos significativos, dejando los 16 bits superiores en cero. Para mover un valor de 32 bits, se usa `MOVT` (Move Top), que mueve otros 16 bits a la parte superior del registro. Juntas, `MOVW` y `MOVT` permiten cargar un valor de 32 bits completo en un registro.

---

## ¿Por qué algunos valores se pueden mover de manera inmediata y otros no?

En ARM, los valores inmediatos deben cumplir con ciertas restricciones debido a cómo se codifican en las instrucciones. Un valor inmediato debe poder representarse con un patrón específico de 12 bits (8 bits de valor y 4 bits de rotación). Si un valor no puede expresarse de esta forma, no se puede mover directamente y requiere una alternativa, como cargarlo desde memoria o usar varias instrucciones.

---

## ¿Cuál es el máximo valor que puede utilizarse como valor inmediato (#valor)?

El máximo valor que puede usarse como valor inmediato en una instrucción ARM es **4095** (0xFFF), ya que los valores inmediatos están limitados a 12 bits. Sin embargo, no todos los valores dentro de este rango son válidos, ya que deben cumplir con las reglas de codificación de ARM (8 bits de valor y 4 bits de rotación).

---

## ¿Cuál es la alternativa para mover números grandes de forma inmediata?

Para mover números grandes que no pueden representarse como valores inmediatos, se puede usar una combinación de instrucciones como `MOVW` y `MOVT`, que permiten cargar un valor de 32 bits en dos pasos (16 bits inferiores y 16 bits superiores). Otra alternativa es almacenar el valor en memoria y cargarlo usando una instrucción como `LDR`.