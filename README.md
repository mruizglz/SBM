# SBM

Repositorio con información de la asignatura Sistemas Basados en Microprocesador de la ETSIS Telecomunicación de la UPM. 

## Instalación de las herramientas para Visual Code

La carpeta `vc-install` contiene los scripts para instalar en Windows y Linux Visual Code y el soporte para usasr CMSIS.
La asignatura continua usando de manera oficial Keil Microvision pero debido a que ARM va a dejar de actualizar esa herramientas y migrar a VC se proporciona la opción de comenzar a utilizarlo.

## Documentación

La documentación de ayuda está disponible en:

- Sphinx Doc: https://mruizglz.github.io/SBM
- PDF: https://mruizglz.github.io/SBM/simplepdf/SBM-CMSIS-RTOS-V2.pdf

## Ejemplos de uso de CMSIS-RTOS incluidos en el repositorio


- `/SBM/B2/ejemplothreads`
  - Uso básico de **threads** concurrentes.
  - Crea dos hilos que controlan los LEDs en `PB0` y `PB7` con distintos retardos (`osThreadNew`, `osDelay`).

- `/SBM/B2/ejemplothreads-flags`
  - Comunicación/sincronización entre hilos mediante **thread flags**.
  - Un hilo `Producer` señaliza flags y un hilo `Consumer` actúa sobre LEDs según `osThreadFlagsWait`.

- `/SBM/B2/ejemplothreads-queues`
  - Comunicación entre hilos con **colas de mensajes**.
  - Un `Producer` inserta datos con `osMessageQueuePut` y un `Consumer` los procesa con `osMessageQueueGet` para controlar LEDs.

- `/SBM/B2/ejemplothreads-timers`
  - Uso de **software timers** en CMSIS-RTOS v2.
  - Crea un timer one-shot y otro periódico (`osTimerNew`, `osTimerStart`) para secuenciar el comportamiento de los LEDs.

Más detalle de cada ejemplo en la documentación Sphinx (`docs/*.rst`).
