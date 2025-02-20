# AntTracker
ESP32 based Antenna Tracker for tracking a moving model aircraft or drone with a small high-gain UHF or SHF antenna. 
Supports Mavlink 1 & 2, CRSF, and GPS


Forked from [zs6buj Ant Tracker](https://github.com/zs6buj/AntTracker) to do a major clean up.
## How to build
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


# TODO
 * CleanUp: Add proper header files to the code files under include/
 * CleanUp: Remove STM code, this will be an esp32 only project
 * Test BoxGPS Support
 * Test QMC5883L Compass support
 * Fix: HMC588L compass support
 * Add/Fix: Baterry voltage sensors


