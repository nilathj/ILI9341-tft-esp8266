## ESP8266 TFT analogue clock demo
This is an an example analogue clock using an ILI9341 TFT LCD screen to show the time use of some of the drawing commands with the TFT_eSPI library.

I am using a 320x240 ILI9341 driver based TFT display connected to an ESP8266 NodeMCU using the TFT_eSPI library on a PlatformIO development environment.

The configuration of the TFT_eSPI library for the TFT display is done inside the platformio.ini file build flags section.

### Here's an image of the display in action:
![ESP8266 TFT Display](/docs/ESP8266TftClock.jpeg)

## TFT Display Pinout for ESP8266 Boards

| TFT Pin     | ESP8266 NodeMCU |GPIO Pin No| Wemos D1 Mini |
|-------------|-----------------|-----------|---------------|
| VCC         | 3V3             |           | 5V            |
| GND         | GND             |           | GND           |
| CS          | D2              | GPIO4     | D2            |
| RST         | D3              | GPIO0     | D3            |
| D/C         | D4              | GPIO2     | D4            |
| SDI (MOSI)  | D7              | GPIO13    | D7            |
| SCK (CLK)   | D5              | GPIO14    | D5            |
| BL (LCD)    | 3V3             |           | 5V            |
| SD0 (MISO)  | D6              | GPIO12    |               |  * Only used for SD card, not for the TFT screen.

## References
* https://github.com/Bodmer/TFT_eSPI/wiki/Installing-on-PlatformIO
* https://thesolaruniverse.wordpress.com/2021/05/02/wiring-an-ili9341-spi-tft-display-with-esp8266-based-microcontroller-boards-nodemcu-and-wemos-d1-mini/