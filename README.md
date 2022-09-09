# esphome-itho
 ESPHome version of the ESPEASY-ITHO plugin. This is code @jodur reworked form https://github.com/CoMPaTech/esphome_c1101 
 The code missed some things i had available in the ESPEASY ITHO plugin
 
## Wiring schema used:

```
Connections between the CC1101 and the ESP8266 or Arduino:
CC11xx pins    ESP pins Arduino pins  Description
*  1 - VCC        VCC      VCC           3v3
*  2 - GND        GND      GND           Ground
*  3 - MOSI       13=D7    Pin 11        Data input to CC11xx
*  4 - SCK        14=D5    Pin 13        Clock pin
*  5 - MISO/GDO1  12=D6    Pin 12        Data output from CC11xx / serial clock from CC11xx
*  6 - GDO2       04=D1    Pin  2        Programmable output 1
*  7 - GDO0       NC       NC            Programmable output 2 (not used)
*  8 - CSN        15=D8    Pin 10        Chip select / (SPI_SS)
```

## Dependencies

 - ESPHome
 - https://github.com/CoMPaTech/esphome_itho
 
 Added:
 - Timer value is counting down when a timer function is activated
 - Extra textsensor to identify the device that had issued the state change of the fan.
 
 Forked from https://github.com/jodur/ITHO-Lib
