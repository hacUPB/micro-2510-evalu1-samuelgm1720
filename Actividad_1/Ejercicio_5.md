# Instrucciones tipo A

Las instrucciones tipo A se caracterizan porque el bit de mayor peso siempre es 0. Su propósito es almacenar los 15 bits menos significativos de la instrucción en un registro A interno de la CPU.
Al ejecutarse, el valor 0x4000 se almacena en el Registro A.

# Instrucciones Tipo C

Las instrucciones tipo C se identifican porque los tres bits de mayor peso siempre son 111. Estas instrucciones permiten realizar operaciones aritméticas y lógicas, así como almacenar resultados en distintos registros y modificar el flujo del programa mediante saltos condicionales.  

## Formato de las instrucciones tipo C:

`destino = operación; salto`  
`1 1 1  a  c1 c2 c3 c4 c5 c6  d1 d2 d3  j1 j2 j3`

- a c1 c2 c3 c4 c5 c6: Determinan la operación que ejecutará la CPU.

- d1 d2 d3: Indican el destino del resultado.

- j1 j2 j3: Definen el tipo de salto que se ejecutará.

La instrucción 0xEC10 esta en lenguaje ensamblador es D=A, lo que significa que el valor almacenado en el Registro A se copia al Registro D.

# Clasificación de las Instrucciones del Procesador
- **Cálculo y Operaciones Lógicas**: Realizan funciones matemáticas y lógicas. Ejemplo: `ADD R1, R2`.  

- **Transferencia de Datos**: Permiten mover información entre registros o entre la memoria y los registros. Ejemplo: `MOV R1, R2`.

- **Control del Programa**: Alteran el orden de ejecución de las instrucciones. Ejemplo: `JMP 200`.

- **Interacción con Periféricos**: Gestionan la comunicación con dispositivos externos. Ejemplo: ``IN R1``.

- **Evaluación y Comparación**: Analizan valores y afectan registros según el resultado. Ejemplo: ``CMP R1, R2``.