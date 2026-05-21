# rc-webusb-tx

Phone → USB-OTG → ESP32-C3 → PPM. WebUSB-based RC transmitter front-end.

Open the live page on Android Chrome (HTTPS required by WebUSB):

  https://madiwelakombuwa.github.io/rc-webusb-tx/

Pair with an ESP32-C3 SuperMini running the matching `servo_control.ino`
firmware (VID 0x303a / PID 0x1001 — Espressif USB-Serial/JTAG). The page
sends `"<throttle> <steering>\n"` lines and `h`/`l`/`t`/`b` LED commands
over USB-CDC at ~50 Hz.
