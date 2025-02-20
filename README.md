# AntTracker
ESP32 based Antenna Tracker for tracking a moving model aircraft or drone with a small high-gain UHF or SHF antenna. 
Supports Mavlink 1 & 2, CRSF, and GPS


Forked from [zs6buj Ant Tracker](https://github.com/zs6buj/AntTracker) to do a major clean up.
## Tested HW
 * ESP32 dev board - [Aliexpress](https://es.aliexpress.com/item/1005008232257795.html)
 * Mateksys Servo PDB - [Aliexpress](https://www.aliexpress.com/item/1005005020804815.html)
 * OLED SSD1306 I2C 0,96inch - [Aliexpress](https://www.aliexpress.com/item/1005007389730469.html)
 * CYCLONE M10 GPS Module + compass M1018C - [Aliexpress](https://www.aliexpress.com/item/1005007507570270.html)
 * MGR MG996 180 All metal servo - [Aliexpress](https://www.aliexpress.com/item/1005007596671764.html)
   
## How to build the SW
 0. Install [Platformio](https://platformio.org/install) 
 1. Check config.h and edit the options.
    Double check the pin definitions!
 2. Connect the esp32 dev kit module
 3. run pio run -t upload to build and upload
    It should download the correct libraries, build and upload the code.

## Developed for 
 * ESP32 Dev Kit
 * ELRS ESP_NOW Telemetry
 * [Sentinel ATT lite HD Case and Hardware](https://github.com/aat-sentinel/AAT-lite-HD-case)


## TODO
 * CleanUp: Add proper header files to the code files under include/
 * CleanUp: Remove STM code, this will be an esp32 only project
 * Document HW wiring and working components
 * Add Tracker batery voltage sensors.
   Voltage Divider: R1: 10k R2: 2.2k for a 4s setup
 * Test BoxGPS Support
 * Test QMC5883L Compass support
 * Fix: HMC588L compass support

## Ideas
 * move to a runtime configuration
 * Add a web interface for configuration
 

