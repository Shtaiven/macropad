# PCB Design

## MCU preferences

* Support both QMK (ChibiOS) and custom ducky firmware.
* MCU must be hand solderable.
* Must have USB stack  on SoC.
* ARM Cortex 32-bit based (M0 or M4).
* Ideally below $15.
* Support mounting as mass storage.
* Support DFU.
* UF2 support?

## Board preferences

* Shouldn't be too big, reduce from 25 keys. 4x4? 3x5?
* Differentiate from the ducky pad.
* Addressable LEDs.
* Optional rotary encoders.
* Hotswap.
* Numpad compatibility?

## MCUs considered

| MCU | Arch | Bit | Clock | Flash | RAM | I/O | QMK | USB | Note |
| --- | ---- | --- | ----- | ----- | --- | --- | --- | --- | ---- |
| [ATmega32u4](https://www.microchip.com/wwwproducts/en/ATmega32U4) | AVR | 8 | 16MHz | 32KB | 2.5KB | 26 | x | x | Arduino UNO and baseline for QMK |
| [STM32F042G6](https://www.st.com/content/st_com/en/products/microcontrollers-microprocessors/stm32-32-bit-arm-cortex-mcus/stm32-mainstream-mcus/stm32f0-series/stm32f0x2/stm32f042g6.html) | ARM Cortex-M0 | 32 | 48MHz | 32KB | 6KB | 38 | x | x | Used by duckyPad |
| [AT32UC3B1256](https://www.microchip.com/wwwproducts/en/AT32UC3B1256) | AVR | 32 | 60MHz | 64KB | 32KB | 28 |  | x | Used by USB Rubber Ducky |
| [STM32F303CCT6](https://www.st.com/en/microcontrollers-microprocessors/stm32f303cc.html) | ARM Cortex-M4 | 32 | 72MHz | 256KB | 40KB | 27 | x | x | Used by Proton C |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |


## Specifications

| Parameter | Value |
| --------- | ----- |
| Board thickness | X mm |
