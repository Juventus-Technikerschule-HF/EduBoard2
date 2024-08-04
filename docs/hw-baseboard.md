---
title: "Baseboard"
permalink: /docs/hw-baseboard
parent: "Hardware"
nav_order: 2
---

# Baseboard

The Eduboard2 Baseboard provides a rich set of Peripherals to use. 
Based on the Idea to have one Baseboard and multiple different Microcontroller Boards the Baseboard provides a m.2 Connector where a Microcontroller Board can be connected. The Pinout is propriatary and does not follow any m.2 standard. 
The Connector has USB routed, which provides the Option to the Microcontroller to be directly connected via USB or to add a Programming Chip via USB.
In Case of the first Microcontroller-Board provided the USB Connection is directly attached to the ESP32-S3. 
This provides Programming and JTAG-Debugging. 

Specifications:
- Supply Voltage
    - USBC
    - External Connector up to 40V
    - 40V to 5V Regulator (1A+)
    - 5V to 3.3V Regulator (1A+)
- External Connections:
    - USBC (Debugging, Programming, Serial Communication)
    - 2x20 Hardware Extension Connector
    - RS485 Connector (3.3V)
    - I2C Connector (3.3V / 5V Selectable)
    - WS2812 Connection Pads (5V)

Hardware Interfaces:

| Description | Pin-Name | ESP32-S3 GPIO | Info |
| -------- | ------- | ------- | --------- |
| 4 x Button  | SW0 - SW3 | IO21 IO47 IO48 IO45 |  |
| 8 x LED | LED0 - LED8 | IO4 IO5 IO6 IO7 IO38 IO35 IO37 IO36 |  |
| 1 x RGB PWM LED | R G B | IO39 IO40 IO41 |  |
| 1 x WS2812 RGB LED | Data | IO15 |  |
| 1 x Potentiometer | AN0 | IO9 |  |
| 1 x Rotary Encoder | A B SW | IO41 IO40 IO39 |  |
| 1 x Piezo Buzzer | Buzzer | IO46 |  |
| 1 x RTC PCF8563T | SDA SCL | IO2 IO1 |  |
| 1 x Accelerometer STK8321 | SDA SCL | IO2 IO1 |  |
| 1 x Thermometer TMP112 | SDA SCL | IO2 IO1 |  |
| 1 x Capacitive Touch FT6236 | SDA SCL | IO2 IO1 |  |
| 1 x 320 * 480 RGB Display ER-TFTM035-6 | MOSI SCK TFT_CS TFT_DC Reset | IO13 IO14 IO11 IO16 IO8 |  |
| 1 x Data Flash W25Q128JV | MOSI MISO SCK Flash_CS | IO13 IO12 IO14 IO3 | CS normally not connected, Shared with DAC |
| 1 x Micro SD Slot | MOSI MISO SCK SD_CS | IO13 IO12 IO14 IO10 | SD_CS Shared with DAC_LD |
| 1 x Dual SPI DAC MCP4802 | MOSI SCK DAC_CS DAC_LD | IO13 IO12 IO3 IO12 | DAC_LD shared with SD_CS |
| 1 x USB-Serial CH340G | UP-TX0 UP-RX0 | TXD0 RXD0 |  |
| 1 x RS485 Transceiver SP3485EN | UP-TX1 UP-RX1 RS485_DE | IO17 IO18 IO42 |  |
| 1 x USB-HUB USB2514BI | D+ D- | IO20 IO19 | Two USB Lanes are used. One for USB-Serial Converter and one for UP |
| 1 x Hardware Extension Connector | See Schematic |  |  |
| 1 x Protoboard Solderpads | See Schematic |  |  |
