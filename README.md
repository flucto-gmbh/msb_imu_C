# smb_imu

this repository contains the code of the ICM-20948 driver + standalone exec to run measurements on the motion sensor box

## Overview

Core sensor for the motion sensor box is [TDK's ICM-20948](https://invensense.tdk.com/products/motion-tracking/9-axis/icm-20948/). The sensor is part of the waveshare senseHat used in the motion sensor boxes. More details can be found under [doc/ICM-20948.md](./doc/ICM-20948.md).

## Hookup

The ICM-20948 is hooked up to the rasberry pi zero by I2C. A few additional connections are available:

| NAME      | PI ZERO PIN              | FUNCTION                                      |
|-----------|--------------------------|-----------------------------------------------|
| ICM_INT   | Pin 22 (WPi) / Pin 6 BCM | Interrupt if new data is available            |
| ICM_FSYNC | Pin 21 (Wpi) / Pin 5 BCM | Synchronize measurement with the raspberry pi |


