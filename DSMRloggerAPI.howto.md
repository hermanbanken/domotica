# DSMR
Docs: https://mrwheel-docs.gitbook.io/dsmrloggerapi

MAC: 84:F3:EB:78:8D:8D
Deze kan je vinden in de router settings als verbonden. ESP maakt hotspot als router niet gevonden is.
Te updaten via OTP en via FTDI.

ESP8266 Core v3.1.2 gebruikt. v2.7.2 eerst geprobeerd; bugje in 2.7.2, workaround:
1. Download https://github.com/espressif/esptool/archive/v3.0.zip
2. Download https://github.com/pyserial/pyserial/archive/v3.4.zip
3. Extract the contents to esptool/ and pyserial/ in the ~/Library/Arduino15/packages/esp8266/hardware/esp8266/2.7.4/tools/ folder (an equivalent must exist on Windows)

Reference van alle pinouts:  https://mrwheel.github.io/DSMRloggerWS/hardware_V4/

Van: https://mrwheel-docs.gitbook.io/dsmrloggerapi/firmware/benodigde-bibliotheken:

- https://github.com/PaulStoffregen/Time/archive/refs/heads/master.zip
- https://github.com/mrWheel/dsmr2Lib/archive/refs/heads/master.zip
- https://github.com/PaulStoffregen/Time/archive/refs/heads/master.zip
- https://github.com/tzapu/WiFiManager/archive/refs/heads/master.zip
- https://github.com/mrWheel/dsmr2Lib/archive/refs/heads/master.zip
- https://github.com/greiman/SSD1306Ascii/archive/refs/heads/master.zip
- https://github.com/knolleary/pubsubclient/archive/refs/heads/master.zip
- https://github.com/mrWheel/ModUpdateServer/archive/refs/heads/master.zip

Preferences > Board Manager URL > https://arduino.esp8266.com/stable/package_esp8266com_index.json > ESP8266

Connect it to FTDI: https://mrwheel.github.io/DSMRloggerWS/hardware_V4_Programmer/

Ingesteld op Flash Size 4MB, want anders past de data niet.
Manueel eerst firmware flashen en dan data kopieren met Arduino ESP8266 LittleFS Filesystem Uploader.
https://github.com/earlephilhower/arduino-esp8266littlefs-plugin
