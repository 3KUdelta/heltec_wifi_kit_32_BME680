# HELTEC WIFI Kit 32 BME680 IAQ example

Calculates IAQ with a BME680 sensor on a Heltec WIFI Kit 32 display

Example, how to use a BME680 (here: GY-BME680 5V/3.3V) and display calculated values on a HELTEC WIFI Kit 32 display
- Reading of raw temperature, humidity and gas resistance
- Allow offset for temperature calibration
- Automatically calculate respective humidity using the August-Roche-Magnus approximation
- Calculate IAQ from temperature, humidity and gas resistance following Dr. Julie Riggs, The IAQ Rating Index, www.iaquk.org.uk

[![BME680](https://github.com/3KUdelta/heltec_wifi_kit_32_BME680/blob/master/images/IMG_20191217_194643.jpg)](https://github.com/3KUdelta/heltec_wifi_kit_32_BME680/)

Code for those who are interested in using a BME680 sensor via I2C and Adafruit libraries to calculate IAQ without the proprietary libraries from Bosch. 

Adafruit´s library: 
  This is a library for the BME280 humidity, temperature & pressure sensor
  Designed specifically to work with the Adafruit BME280 Breakout
  ----> http://www.adafruit.com/products/2650
  These sensors use I2C or SPI to communicate, 2 or 4 pins are required
  to interface. The device's I2C address is either 0x76 or 0x77.
  Adafruit invests time and resources providing this open source code,
  please support Adafruit andopen-source hardware by purchasing products
  from Adafruit!
  Written by Limor Fried & Kevin Townsend for Adafruit Industries.
  BSD license, all text above must be included in any redistribution

Libraries needed:
- ThingPulse SSD1306 (https://github.com/ThingPulse/esp8266-oled-ssd1306)
- General Adafruit Sensor (Arduino Library Manager)
- Adafruit BME680 (Arduino Library Manager)
- SoftwWire Steve Marple (Arduino Library Manager)
- AsyncDelay Steve Marple (Arduino Library Manager)

Hardware settings Mac:
Heltec_WFIF_Kit_32,80MHz,921600 on /dev/cu.SLAB_USBtoUART
