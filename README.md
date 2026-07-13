# Sistemas Basados en Microprocesador (ETSI Sistemas de Telecomunicación-Campus Sur UPM)

Repositorio con información sobre la asignatura Sistemas Basados en Microprocesador de la ETSIS Telecomunicación de la UPM. 

## Estructura del repositorio

- `B2/` - Ejemplos de uso de CMSIS-RTOS v2 (proyectos en Keil µVision y Visual Studio Code) y material de la presentación de CMSIS-RTOS2.
  - `ejemplothreads/`, `ejemplothreads-flags/`, `ejemplothreads-queues/`, `ejemplothreads-timers/` - Código fuente (`src/`), proyecto Keil (`keil/`) y proyecto de Visual Code/CMSIS (`vc/`) de cada ejemplo.
  - `presentation/` - Diapositivas y material gráfico (en español e inglés) utilizados en las sesiones teóricas.
- `docs/` - Fuentes en reStructuredText (Sphinx) de la documentación de ayuda publicada en GitHub Pages.
- `vc-install/` - Scripts de instalación/desinstalación de Visual Studio Code y del soporte CMSIS para Windows y Linux.

## Instalación de las herramientas para Visual Code

La carpeta `vc-install` contiene los scripts para instalar Visual Code en Windows y Linux y el soporte para usar CMSIS.
La asignatura continúa usando de manera oficial Keil µVision, pero debido a que ARM va a dejar de actualizar esas herramientas y migrar a VC, se proporciona la opción de comenzar a utilizarlo.

- `vc-install/windows/installer2.ps1` y `vc-install/windows/uninstaller.ps1` - Instalación y desinstalación completas del entorno en Windows.
- `vc-install/linux/install.sh` y `vc-install/linux/uninstall.sh` - Instalación y desinstalación completas del entorno en Linux (Ubuntu 24.04).

## Documentación

La documentación de ayuda (generada a partir de las fuentes en `docs/`) está disponible en:

- Sphinx Doc: https://univ-politecnica-madrid.github.io/SBM/
- PDF: https://univ-politecnica-madrid.github.io/SBM/simplepdf/SBM-CMSIS-RTOS-V2.pdf

