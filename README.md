# PMOD I3C Sensor Board

Copyright (c) 2026 [Antmicro](https://www.antmicro.com)

![](img/pmod-i3c-sensor-board-visualization.png)

## Overview

This project contains open hardware PCB design files for a simple expansion board with three environmental sensors connected to a common I3C bus. 
This expansion board has a pinout that is electrically compatible with Digilend PMOD (Peripheral Module) which allows to use it with various development platforms.
Additionally the board is equipped with two push-pull digital output drivers composed of discrete MOSFETs.
This allows to use the board with FPGA-driven systems to implement I3C output stage driver which can act as open drain or push-pull.
The driver topology is switchable via digital control signals from FPGA-side.
A separate set of control signals allows to activate pull-up or pull-down resistors connected to the output signals.

The PCB design files were prepared in KiCad 9.x.

## Key features

* [P3T1755DP/Q900Z](https://www.nxp.com/part/P3T1755DP~~Q900) - Temperature Sensor 

* [MMC5603NJ](https://www.memsic.com/Public/Uploads/uploadfile/files/20220119/MMC5603NJDatasheetRev.B.pdf) - 3-axis Magnetic Sensor 

* [BMA580](https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bma580-ds000.pdf) - 3-axis Accelerometer 

* All sensors support I2C/I3C interfaces

* Two independent digital output stages configurable as push-pull or open drain

* Switchable pull-up and pull-down resistors

## Licensing

This project is published under the [Apache-2.0](LICENSE) license.
