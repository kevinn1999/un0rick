---
layout: default
title: un0rick hardware 
parent: un0rick
nav_order: 2
---

## Open ultrasound pulse-echo features 

![](https://github.com/kelu124/un0rick/raw/master/images/un0rick_black.png)

## Design and specs of the un0rick


1. __FPGA__: Lattice iCE40HX4K - TQFP 144 Package
2. __Memory__:
  * 8 Mbit SRAM, 10ns, 512 k x 16, equivalent:
      * 65 full lines of 120us at 64Msps
      * 840 lines of 120us at 10Msps, 8 bits
  * 8 Mb SPI Flash for FPGA configuration 
3. __Ultrasound processing__:
  * __VGA__: AD8331 controled by DAC
  * __Pulser__: MD1210 + TC6320
  * __ADC__: 65Msps ADC10065
    * 10 bits of data / sample
    * 2 bits of line counters
    * 4 bits of IOs (counters, ...) 
4. __Parameters__: Settings programable via USB or Raspberry Pi 
  * Type of acquisition (one line / set of lines)
  * Number of lines
  * Length of lines acquisitions
  * Delay between acquisitions
  * Pulse width 
  * Delay between pulse and beginning of acquisitions
  * 200us time-gain-compensation programmable (8 bits, from 0 to Max), every 5us
5. __Extensibility__:
  * 2 x Pmod connectors
  * SMA plug for transducers
  * RPi GPIO
6. __User Interfaces__:
  * 2 x PMOD for IOs
  * 3 x push button (with software noise debouncing)
  * Jumpers for high voltage selection
7. __Input Voltage__: 
  * 5 V from RPi or USB
  * Uses 350mA-450mA at 5V
8. __Fully Open Source__:
  * Hardware: [github](https://github.com/kelu124/un0rick/tree/master/hardware) - done through [upverter](https://upverter.com/design/kelu124/c59550d3e0dcf944/un0rick-v11/).
  * Gateware: [github](https://github.com/kelu124/un0rick/tree/master/software)
  * Toolchain: [Project YoSys](http://www.clifford.at/yosys/)
  * Documentation: [this website](http://un0rick.cc/un0rick)
9. __Operating Voltage__: 
  * FPGA and logics at at 3.3 V
  * High voltage at 25V, 50V, 75V
10. __Dimensions__: @todo!
11. __Weight__: @todo! 


## Overview of the board itself

![](https://raw.githubusercontent.com/kelu124/echomods/master/matty/images/black/P_20191214_151518_good.jpg)
