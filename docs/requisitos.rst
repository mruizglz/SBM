.. _requisitos:

===================
Recursos a utilizar
===================

Para el desarrollo de las prácticas del curso, se debe utilizar el software Keil µVision (disponible únicamente en Windows). Adicionalmente, también se da la opción de poder utilizar Visual Code (disponible en Windows y en Linux), aunque el uso de esta opción todavía está en pruebas. Se recomienda instalar Visual Code con los instaladores incluidos en este repositorio. Están disponibles en la carpeta ``vc-install`` para Linux (Ubuntu 24.04) y Windows 11/10


Keil µVision
============

El instalador de Keil µVision permite instalar el IDE y seleccionar los paquetes de software correspondientes. Utilice las versiones indicadas en la tabla :numref:`KeilµVision`

.. list-table:: Versiones para Keil µVision a utilizar en SBM 
   :header-rows: 1
   :widths: 30 20 50
   :name: KeilµVision

   * - Software
     - Versión
     - Propósito
   * - Keil Microvision
     - Version 5.43a
     - Editor e IDE principal
   * - Paquete Keil::STM32F4xx\_DFP
     - 2.17.1
     - Soporte de dispositivo para STM32F4
   * - Paquete Keil::MDK\_Middelware
     - 8.1.0
     - Soporte Middleware para procesadores ARM
   * - Paquete ARM::CMSIS
     - 6.3.0
     - Núcleo CMSIS, headers Cortex-M
   * - Paquete ARM::CMSIS-Driver
     - 2.10.0
     - Drivers para I2C, SPI, USART, etc Cortex-M
   * - Paquete ARM::CMSIS-RTX
     - 5.9.1
     - Sistema operativo RTX5 para Cortex M

  

Visual Code
===========

Los instaladores proporcionados para Windows y Linux instalan las versiones indicadas en las siguiente tabla :numref:`vc`

.. list-table:: Versiones para VC a utilzar en SBM 
   :header-rows: 1
   :widths: 30 20 50
   :name: VC

   * - Software
     - Versión
     - Propósito
   * - Visual Studio Code
     - Última estable
     - Editor e IDE principal
   * - ARM Keil Studio Pack
     - MDK v6 (última)
     - Extensión de VS Code para desarrollo embebido ARM
   * - CMSIS-Toolbox
     - Última (vía vcpkg)
     - Herramientas de línea de comandos: ``cbuild``, ``cpackget``, ``csolution``
   * - Arm Compiler
     - 6.24.0 
     - Compilador ``AC6``
   * - CMake
     - 3.25 
     - Sistema de build
   * - Ninja
     - 1.10 
     - Generador de build rápido
   * - Paquete Keil::STM32F4xx\_DFP
     - 2.17.1 
     - Soporte de dispositivo para STM32F4
   * - Paquete ARM::CMSIS
     - 6.3.0
     - Núcleo CMSIS, headers Cortex-M
   * - Paquete Keil::MDK\_Middelware
     - 8.1.0
     - Soporte Middleware para procesadores ARM
   * - Paquete ARM::CMSIS-Driver
     - 2.10.0
     - Drivers para I2C, SPI, USART, etc Cortex-M
   * - Paquete ARM::CMSIS-RTX
     - 5.9.1
     - Sistema operativo RTX5 para Cortex M

Hardware necesario
==================

* Ordenador con sistema operativo Windows 10/11 (64 bits) o Ubuntu 24.04. En Windows tambien se puede utilizar una máquina virtual con VMWare Player para ejecutur Ubuntu 24.04-
* Placa STM32F429I-Discovery con cable USB para depuración en hardware real.
* Driver de software para comunicarse con el ST-LINK V2/V3.


