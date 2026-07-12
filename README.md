# SBM

Repositorio con información de la asignatura Sistemas Basados en Microprocesador de la ETSIS Telecomunicación de la UPM. 

## Estructura del repositorio

- `B2/` - Ejemplos de uso de CMSIS-RTOS v2 (proyectos Keil µVision y Visual Code) y material de presentación de la asignatura.
  - `ejemplothreads/`, `ejemplothreads-flags/`, `ejemplothreads-queues/`, `ejemplothreads-timers/` - Código fuente (`src/`), proyecto Keil (`keil/`) y proyecto Visual Code/CMSIS (`vc/`) de cada ejemplo.
  - `presentation/` - Diapositivas y material gráfico (en español e inglés) usados en las sesiones teóricas.
- `docs/` - Fuentes en reStructuredText (Sphinx) de la documentación de ayuda publicada en GitHub Pages.
- `vc-install/` - Scripts de instalación/desinstalación de Visual Studio Code y el soporte CMSIS para Windows y Linux.

## Instalación de las herramientas para Visual Code

La carpeta `vc-install` contiene los scripts para instalar Visual Code en Windows y Linux y el soporte para usar CMSIS.
La asignatura continúa usando de manera oficial Keil µVision, pero debido a que ARM va a dejar de actualizar esas herramientas y migrar a VC, se proporciona la opción de comenzar a utilizarlo.

- `vc-install/windows/installer2.ps1` y `vc-install/windows/uninstaller.ps1` - Instalación y desinstalación completas del entorno en Windows.
- `vc-install/linux/install.sh` y `vc-install/linux/uninstall.sh` - Instalación y desinstalación completas del entorno en Linux (Ubuntu 24.04).

## Documentación

La documentación de ayuda (generada a partir de las fuentes en `docs/`) está disponible en:

- Sphinx Doc: https://mruizglz.github.io/SBM
- PDF: https://mruizglz.github.io/SBM/simplepdf/SBM-CMSIS-RTOS-V2.pdf

## Ejemplos de uso de CMSIS-RTOS incluidos en el repositorio

Todos los ejemplos están implementados para el STM32F429 y pueden compilarse/depurarse tanto con Keil µVision (carpeta `keil/`) como con Visual Studio Code y CMSIS-Toolbox (carpeta `vc/`).

- `B2/ejemplothreads`
  - Uso básico de un **thread** en CMSIS-RTOS v2.
  - Crea dos hilos que controlan los LEDs en `PB0` y `PB7` con distintos retardos (`osThreadNew`, `osDelay`).

- `B2/ejemplothreads-flags`
  - Comunicación/sincronización entre hilos mediante **thread flags**.
  - Un hilo `Producer` señaliza flags y un hilo `Consumer` actúa sobre los LEDs según `osThreadFlagsWait`.

- `B2/ejemplothreads-queues`
  - Comunicación entre hilos mediante **colas de mensajes**.
  - Un `Producer` inserta datos con `osMessageQueuePut` y un `Consumer` los procesa con `osMessageQueueGet` para controlar LEDs.

- `B2/ejemplothreads-timers`
  - Uso de **software timers** en CMSIS-RTOS v2.
  - Crea un hilo `Timers` con un timer one-shot y otro periódico (`osTimerNew`, `osTimerStart`) para secuenciar el comportamiento de los LEDs.

Más detalles de cada ejemplo en la documentación de Sphinx (`docs/*.rst`).
