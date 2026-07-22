# esp-flasher

Web-hosted firmware flasher for the ESP32-S3 WROOM Board.

Firmware flashed includes:
- Micropython (v1.29.0)
- ulab (v6.12.1)
- camera (v0.6.2)

copied this
https://github.com/cnadler86/micropython-camera-API#build-your-custom-firmware

to build, run:
`firmware/micropython-camera-API/build.sh firmware/micropython -b ESP32_GENERIC_S3 -v SPIRAM_OCT`

to flash:
use the web tool or do `idf.py -B build-mp_camera-ESP32_GENERIC_S3_SPIRAM_OCT erase-flash flash` with an existing esp-idf environment (do `. ~/esp/esp-idf/export.sh`). 

to update the web tool, make ur changes then make sure to duplicate the new firmware into 
/docs by `cp firmware/micropython/ports/esp32/build-mp_camera-ESP32_GENERIC_S3_SPIRAM_OCT/firmware.bin docs`
