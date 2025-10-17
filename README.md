🧠 Supported Devices & Interfaces

Waffles Firmware supports a range of embedded boards and virtual platforms. Below is a detailed compatibility matrix including connectivity options, peripheral support, and estimated retail prices (USD, 2025).

Legend:
✅ = Supported ⚙️ = In Progress 🚧 = Experimental — = Not applicable Sim = Simulated support (no real hardware access)

Platform / MCU	Board Example	Template	Build Status	Wi-Fi	BLE	RF	FM	nRF24	Mic	NFC	IR	Est. Price (USD)	Notes
ESP32	ESP32-DevKitC, ESP32-WROOM	templates/esp32/	✅ Stable	✅	✅	✅	—	—	✅	⚙️	✅	$8 – $12	Full support for Wi-Fi, BLE, RF, optional Mic and IR. Ideal for network labs and pentest simulations.
STM32	Nucleo-F446RE, Blue Pill	templates/stm32/	⚙️ In Progress	—	—	✅	—	✅	⚙️	—	✅	$10 – $20	Supports RF & nRF24. Mic support in progress. Great for hardware hacking exercises.
RP2040	Raspberry Pi Pico	templates/rp2040/	🚧 Experimental	—	✅ (addon)	✅	—	✅	✅	—	✅	$4 – $8	Lightweight and modular. Supports BLE, RF, Mic, and IR. Perfect for educational labs.
ATmega328P	Arduino Uno R3	templates/atmega328p/	✅ Stable	—	—	✅	—	✅	⚙️	—	✅	$12 – $18	Classic Arduino platform for low-level RF, IR, and educational security experiments.
ESP8266	NodeMCU	templates/esp8266/	⚙️ In Progress	✅	—	✅	—	—	—	—	—	$5 – $8	Legacy Wi-Fi support. Good for telemetry and IoT experiments.
BBC micro:bit v2	nRF52833 SoC	templates/microbitv2/	✅ Stable	—	✅	✅	—	✅ (addon)	✅	—	✅	$18 – $25	Built-in BLE, Mic, buttons, accelerometer. Excellent for educational demos and security teaching.
x86 VM Simulator	QEMU / VirtualBox	templates/sim/	✅ Stable	Sim	Sim	Sim	Sim	Sim	Sim	Sim	Sim	Free	Simulated platform for safe lab exercises, CI builds, and testing firmware logic.
💡 Notes on Interface Support

Wi-Fi / BLE — Network experimentation, pentesting exercises, and IoT security simulations.

RF / nRF24 — Low-power wireless communication experiments and lab simulations.

FM — Experimental radio signal reception (lab-only).

Mic — Audio input for signal analysis or detection labs.

NFC — Secure tag reading/writing for safe hacking simulations.

IR — Remote-control signal testing, IR communication labs.

Tip: All hardware features should be tested in controlled lab environments with consented devices only. Avoid using Waffles Firmware on live production hardware.

🔧 Upcoming Devices & Modules

We plan to expand support for:

ESP32-S3 / ESP32-C3 — Enhanced BLE and Wi-Fi modules.

Teensy 4.1 — High-speed microcontroller for advanced RF experiments.

Raspberry Pi Compute Module 4 — Full lab-grade experimentation platform.

Contributions for device templates and module integrations are highly encouraged. See CONTRIBUTING.md
 for guidelines.
