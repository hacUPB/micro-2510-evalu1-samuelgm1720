## ¿Qué significa que ARM sea una arquitectura RISC?

Que ARM sea una arquitectura **RISC** (Reduced Instruction Set Computer) significa que su diseño se basa en un conjunto de instrucciones reducido y altamente optimizado. Las características principales incluyen instrucciones simples que se ejecutan en un solo ciclo de reloj, eficiencia energética ideal para dispositivos móviles, un pipeline eficiente que permite la ejecución simultánea de múltiples instrucciones, y un uso intensivo de registros que reduce la necesidad de acceder a la memoria, lo que acelera las operaciones.


## ¿Por qué la arquitectura ARM es popular en dispositivos móviles?

La arquitectura ARM es popular en dispositivos móviles debido a su bajo consumo de energía, que maximiza la duración de la batería, su alto rendimiento que equilibra potencia y eficiencia, y su escalabilidad, ya que existen variantes para diferentes necesidades. Además, su coste reducido y su ecosistema robusto, con amplia compatibilidad de software y herramientas de desarrollo, la hacen ideal para smartphones y tablets.


## ¿En qué consiste la “Arquitectura Harvard modificada” en ARM?

La **Arquitectura Harvard modificada** en ARM combina características de las arquitecturas Harvard y von Neumann. Usa buses separados para instrucciones y datos a nivel interno, lo que permite acceder a ambos simultáneamente, pero a nivel externo utiliza un espacio de memoria unificado para simplificar el diseño del sistema. Esto mejora el rendimiento sin sacrificar la flexibilidad.


## ¿Cuáles son las principales familias de procesadores ARM?

Las principales familias de procesadores ARM son **Cortex-A** (para aplicaciones de alto rendimiento como smartphones), **Cortex-R** (optimizados para aplicaciones en tiempo real como automóviles), **Cortex-M** (para microcontroladores de bajo consumo), **ARM Classic** (procesadores antiguos como ARM7 y ARM9), y **ARM Neoverse** (diseñados para infraestructura en la nube y servidores).


## ¿Qué ventajas ofrece el set de instrucciones Thumb-2?

El set de instrucciones **Thumb-2** combina lo mejor de Thumb (instrucciones de 16 bits) y ARM (instrucciones de 32 bits), ofreciendo densidad de código que reduce el tamaño del programa, rendimiento mejorado al permitir instrucciones más complejas, flexibilidad para mezclar instrucciones de 16 y 32 bits, y compatibilidad con software diseñado para Thumb.


## ¿Por qué es relevante la comunidad ARM?

La comunidad ARM es relevante porque fomenta la innovación colaborativa, proporciona soporte y documentación para desarrolladores, facilita un ecosistema abierto que permite la creación de productos compatibles y personalizados, y su adopción masiva garantiza una amplia base de usuarios y expertos que contribuyen al crecimiento de la tecnología.



## ¿Qué características distinguen al ARM Cortex-M4?

El **ARM Cortex-M4** se destaca por incluir una unidad de punto flotante (FPU) para operaciones en coma flotante, instrucciones optimizadas para procesamiento digital de señales (DSP), bajo consumo energético típico de la familia Cortex-M, y un rendimiento equilibrado que lo hace ideal para sistemas embebidos avanzados.


## ¿Qué tipos de registros básicos se encuentran en la arquitectura ARM Cortex-M?

En la arquitectura ARM Cortex-M, los registros básicos incluyen registros de propósito general (R0-R12) para almacenar datos temporales, el registro de stack pointer (SP) que apunta a la pila actual, el registro de enlace (LR) que almacena la dirección de retorno en llamadas a funciones, el registro de contador de programa (PC) que indica la siguiente instrucción a ejecutar, y el registro de estado del programa (PSR) que contiene banderas de estado como cero o negativo.


## ¿Para qué se utilizan los modos Thread y Interrupt en ARM Cortex-M?

En ARM Cortex-M, el **modo Thread** es el modo normal de ejecución del programa, utilizado para ejecutar código de aplicación, mientras que el **modo Interrupt** se activa cuando ocurre una interrupción o excepción, permitiendo ejecutar rutinas de servicio de interrupciones (ISR) con prioridad sobre el código normal.


## ¿En qué consiste el mapa de memoria de 4 GB en Cortex-M?

El mapa de memoria de 4 GB en Cortex-M divide el espacio de direcciones en regiones específicas: código (0x00000000 - 0x1FFFFFFF) para instrucciones, SRAM (0x20000000 - 0x3FFFFFFF) para datos, periféricos (0x40000000 - 0x5FFFFFFF) para acceder a registros de periféricos, RAM externa (0x60000000 - 0x9FFFFFFF), dispositivos externos (0xA0000000 - 0xDFFFFFFF), y sistema (0xE0000000 - 0xFFFFFFFF) para el núcleo y funciones del sistema. Este mapa permite una organización eficiente de los recursos.