# PPV2-Samples-GeigerMueller

A Geiger-Müller counter based on an inexpensive counter tube with electronics and an ESP32.
The counter tube transmits the impulses of the radioactive particles to an ESP32. This sums up the impulses and writes them to a REDIS database via WiFi.
This happens hourly as a rin buffer for one month, as well as continuously on a daily basis.
A LuaRTOS runs on the ESP32. The application was developed using the p + simulation system.

1. Download the lates version of [p+](https://github.com/Mynogs/PPV2-ESP32)
2. Visit the [Lua RTOS](ttps://github.com/whitecatboard/Lua-RTOS-ESP32) page and follow the intruction to install the Lua RTOS on the ESP32 device.

:exclamation: Set the p+ user level to **Basic** to enable remote target injection.

:exclamation: Don't forget to set the correct COM port under <i>Simulation->Settings->Remote Target</i>!
