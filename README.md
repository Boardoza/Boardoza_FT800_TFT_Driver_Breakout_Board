# Boardoza FT800 TFT Driver Breakout Board

The **Boardoza FT800 TFT Driver Breakout Board** is a powerful graphics controller solution designed to simplify the creation of high-quality Human-Machine Interfaces (HMIs) for makers and embedded developers. Powered by the **Bridgetek (FTDI) FT800 Embedded Video Engine (EVE)**, this module unburdens your main microcontroller by handling complex graphics rendering, audio processing, and touch control on a dedicated chip. It is the perfect bridge for connecting low-cost MCUs to sophisticated color displays.

Operating with a **5V supply**, the board communicates via a standard **SPI interface** at speeds up to 30 MHz, making it compatible with popular platforms including Arduino, ESP32, STM32, and Raspberry Pi. It supports **WQVGA (480x272)** and **QVGA (320x240)** resolution TFT displays through a standard 40-pin FPC connector. Beyond graphics, it includes a built-in audio engine with PWM output for direct speaker connection. The FT800 offers flexible touch input options with **integrated resistive touch support** and **native capacitive touch connectivity via I²C**, providing a complete multimedia solution for industrial control panels, medical devices, IoT projects, and smart home interfaces.

## [Click here to purchase!](https://www.ozdisan.com/p/arduino-sensorleri-ve-modulleri-613/boardoza-boardoza-ft800-1473939)

|Front Side|Back Side|
|:---:|:---:|
| ![FT800 Front](./assets/FT800%20Front.png)| ![FT800 Back](./assets/FT800%20Back.png)|

---

## Key Features

- **Dual Resolution Support:** Compatible with WQVGA (480x272) and QVGA (320x240) TFT panels with both DE mode and VSYNC/HSYNC synchronization.  
- **Works with any MCU:** Uses standard SPI, compatible with Arduino, ESP32, STM32, Raspberry Pi Pico, and more.  
- **Resistive & Capacitive Touch Support:** Integrated resistive and capacitive touch controller support via I²C.  
- **Audio Output:** Mono audio channel with PWM output and dedicated speaker connections.  
- **Object-Oriented Architecture:** Advanced command-based system enables low-cost host MCUs to create sophisticated HMI applications.  
- **Perfect for custom HMIs:** Great for dashboards, robotics screens, measurement devices, smart panels, and DIY UI projects.  
- **Display Control Signals:** Built-in display enable, pixel clock, and sync signal outputs for direct TFT panel control.  
- **Interrupt Capability:** Hardware interrupt output for efficient event-driven programming.  

---

## FT800 vs [FT810](https://github.com/Boardoza/Boardoza_FT810_TFT_Driver_Breakout_Board) Comparison

| Feature | FT800 | [FT810](https://github.com/Boardoza/Boardoza_FT810_TFT_Driver_Breakout_Board) |
|:---|:---:|:---:|
| **Supported Resolutions** | WQVGA (480x272), QVGA (320x240) | up to SVGA (800x600) |
| **Maximum Resolution** | WQVGA (480x272) | SVGA (800x600) |
| **Resistive Touch Support** | ✓ Integrated | ✓ Integrated |
| **Capacitive Touch Support** | ✓ Direct connection via I²C (J9) | ✗ Requires expansion board |
| **Audio Output** | ✓ Mono with PWM output, integrated speaker & line out | ✓ Mono with PWM output, integrated speaker & line out |
| **SPI Interface** | ✓ Up to 30 MHz | ✓ Up to 30 MHz |
| **Board Dimensions** | 40mm x 100mm | 40mm x 100mm |

> **Note:** The FT800 provides native capacitive touch support through the dedicated I²C connector (J9), allowing direct connection to capacitive touch panels. The FT810 focuses on resistive touch integration but can support capacitive touch through an external interface board if needed.

---

## Technical Specifications

**Model:** FT800  
**Manufacturer:** Bridgetek (FTDI)  
**Input Voltage:** 5V  
**Voltage Input Type:** Multiple pin connector (standard 2.50mm pitch)  
**Working Current:** 150mA  
**Functions:** Embedded Video Engine (Graphics Controller, Audio Processor, Touch Controller)  
**Interface:** SPI (up to 30 MHz), I²C (capacitive touch)  
**Supported Resolutions:** WQVGA (480x272), QVGA (320x240)  
**Display Modes:** Data Enable (DE), VSYNC/HSYNC  
**Touch Input:** Resistive (integrated), Capacitive (external via I²C)  
**Color Depth:** RGB666 (18-bit, 6-bit per color channel)  
**Audio Output:** Mono PWM audio channel  
**Connector Type:** 40-Pin FPC  
**Operating Temperature:** -40°C ~ +85°C  
**Board Dimensions:** 40mm x 100mm

---

## Board Pinout

### **( J1 ) Power and Control**

| Pin Number | Pin Name | Description |
|:---:|:---:|---|
| 1 | 3V3 | 3.3V Voltage Output |
| 2 | 5V | Board Supply Input |
| 3 | GND | Ground |
| 4 | PD | Power Down / Board Enable (Active High, 3.3V-5V compatible) |
| 5 | INT | Interrupt Output (3.3V logic level) |

### **( J2 ) TFT Display & Touch Interface**

| Pin Number | Pin Name | Description |
|:---:|:---:|---|
| 1 | LED- | LED Backlight Driver Negative |
| 2 | LED+ | LED Backlight Driver Positive |
| 3 | GND | Ground |
| 4 | VDD | 3.3V Power Output |
| 5 | GND | Ground |
| 6 | GND | Ground |
| 7 | R2 | Red RGB Signal Bit 2 |
| 8 | R3 | Red RGB Signal Bit 3 |
| 9 | R4 | Red RGB Signal Bit 4 |
| 10 | R5 | Red RGB Signal Bit 5 |
| 11 | R6 | Red RGB Signal Bit 6 |
| 12 | R7 | Red RGB Signal Bit 7 |
| 13 | GND | Ground |
| 14 | GND | Ground |
| 15 | G2 | Green RGB Signal Bit 2 |
| 16 | G3 | Green RGB Signal Bit 3 |
| 17 | G4 | Green RGB Signal Bit 4 |
| 18 | G5 | Green RGB Signal Bit 5 |
| 19 | G6 | Green RGB Signal Bit 6 |
| 20 | G7 | Green RGB Signal Bit 7 |
| 21 | GND | Ground |
| 22 | GND | Ground |
| 23 | B2 | Blue RGB Signal Bit 2 |
| 24 | B3 | Blue RGB Signal Bit 3 |
| 25 | B4 | Blue RGB Signal Bit 4 |
| 26 | B5 | Blue RGB Signal Bit 5 |
| 27 | B6 | Blue RGB Signal Bit 6 |
| 28 | B7 | Blue RGB Signal Bit 7 |
| 29 | GND | Ground |
| 30 | DATA_CLOCK | TFT Pixel Clock Output (Push-Pull) |
| 31 | DISP | Display Enable Output (Push-Pull) |
| 32 | HSYNC | Horizontal Sync Output (Push-Pull) |
| 33 | VSYNC | Vertical Sync Output (Push-Pull) |
| 34 | DE | Data Enable Output (Push-Pull) |
| 35 | NC | Not Connected |
| 36 | GND | Ground |
| 37 | X+ | Touch Screen Right Electrode |
| 38 | Y- | Touch Screen Bottom Electrode |
| 39 | X- | Touch Screen Left Electrode |
| 40 | Y+ | Touch Screen Top Electrode |

### **( J3 ) Speaker Output**

| Pin Number | Pin Name | Description |
|:---:|:---:|---|
| 1 | Speaker+ | Speaker Output Positive |
| 2 | Speaker- | Speaker Output Negative |

### **( J5 ) Audio Line Output**

| Pin Number | Pin Name | Description |
|:---:|:---:|---|
| 1 | Audio Out+ | Audio Line Output Positive |
| 2 | Audio Out- | Audio Line Output Negative |

### **( J6 ) SPI Communication**

| Pin Number | Pin Name | Description |
|:---:|:---:|---|
| 1 | CS | SPI Chip Select (Active Low) |
| 2 | MISO | SPI Master In, Slave Out |
| 3 | MOSI | SPI Master Out, Slave In |
| 4 | SCK | SPI Clock Input |

### **( J7 ) Auxiliary Power**

| Pin Number | Pin Name | Description |
|:---:|:---:|---|
| 1 | 5V+ | Board Supply Input |
| 2 | 5V- | Ground |

### **( J9 ) Capacitive Touch I²C Interface**

| Pin Number | Pin Name | Description |
|:---:|:---:|---|
| 1 | INT | Capacitive Touch Interrupt (Active Low) |
| 2 | SDA | I²C Serial Data Pin |
| 3 | SCL | I²C Serial Clock Pin |
| 4 | RST | Capacitive Touch Reset (Active Low) |

> **Note:** The FT800 includes an integrated resistive touch controller. The J9 connector provides optional support for external capacitive touch controllers via I²C interface.

---

## Board Dimensions

<img src="./assets/FT800%20Dimension.png" alt="FT800 Board Dimensions" width="450"/>

---

## Step Files

[Boardoza FT800.step](./assets/FT800%20Step.step)

---

## Datasheet

[FTDI FT800 Datasheet.pdf](./assets/FT800%20Datasheet.pdf)

---

## Version History

- V1.0.0 – Initial Release  

---

## Support

For technical questions or assistance, please contact **<support@boardoza.com>**

---

## License

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
