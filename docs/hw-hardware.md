---
title: Hardware
permalink: /docs/hw-hardware
has_children: true
nav_order: 2
---

# Eduboard2 Hardware

The Eduboard2 was designed with 3 maingoals in mind:
- Support different Microcontroller-Platforms
    - The Microcontroller is separated out onto a second Board, connected via m.2. This allows easy adaptability to other microcontrollers. The first supported Microcontroller was descided to be the ESP32-S3. The ESP32-S3 can be programmed and debugged via USB.
- Have a wide and modern variety of Peripheral options
    - From the classics like buttons leds and potentiometers up to a modern Color screen with capacitive touch. Also some external Interfaces like RS485 are present. 
        - 4x Buttons
        - 8x LEDs
        - 1x ADC Potentiometer
        - 1x Rotary Encoder
        - 1x 320*480 16Bit LCD
            - Touch Controller FT6236 Dual Capacitive Touch
        - 1x PWM RGB LED
        - 1x WS2812 RGB LED
            - signal output routed to expansion connection
        - 1x Piezo Buzzer
        - 1x RTC PCF8563T with Battery
        - 1x SPI DAC MCP4802 with 2 Outputs
        - 1x SPI-Flash W25Q128 (16MByte)
        - 1x MicroSD Card Slot
        - 1x STK8321 3 Axis Accelerometer
        - 1x USB-Serial Interface CH340G routed to Microcontroller
        - 1x RS485 Transceiver SP3485
        - 1x 2x20 Expansion Connector
        - Supply Voltage
            - USBC
            - External Connector up to 40V
        - Protoboard Area with all important Signals routed to it
- be cheaper in production then the first iteration
    - Production of the Eduboard2 is done at JLCPCB. This cuts the costs even with the two seperate boards more then in half.

