# esp-flasher

Web-hosted firmware flasher for the ESP32-S3 WROOM Board.

Firmware flashed includes:
- Micropython 
- ulab
- camera


From this link: https://micropython.org/download/ESP32_GENERIC_S3/, we want the latest .bin under **Firmware (Support for Octal-SPIRAM)**. This flasher uses v1.28.

copied this
https://github.com/cnadler86/micropython-camera-API#build-your-custom-firmware

the camera is a freenove esp32s3

from firmware directory:
`micropython-camera-API/build.sh micropython -b ESP32_GENERIC_S3 -v SPIRAM_OCT`

