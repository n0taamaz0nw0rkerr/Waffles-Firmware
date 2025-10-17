# Waffles Firmware

Ethical hacking & defensive cybersecurity firmware for embedded devices
Lightweight, audit-friendly firmware and tooling designed for responsible security research, lab-based pentesting, and device hardening practice. Built with transparency, testability, and strong ethical safeguards at the core.

### Key features

Minimal, auditable firmware stack for common microcontrollers (template-based, hardware-agnostic).

Secure boot & basic runtime integrity checks (reference implementations).

Safe, sandboxed diagnostic tools for network/USB/serial observation in lab environments.

Logging & forensics hooks to capture reproducible test artifacts.

CI-friendly build matrix and firmware signing examples.

Developer-focused: comprehensive docs, unit tests, and example lab topologies.

Strong emphasis on legality, consent and responsible disclosure — for research/use in controlled environments only.

### Who it's for

Security researchers building reproducible embedded-device tests.

Red-team/blue-team labs that need a safe, auditable firmware baseline.

Educators teaching secure embedded development and ethical hacking.

Device teams who want a reference for hardening their own firmware.

### Supported Devices

| Platform / MCU       | Board Example              | Template                | Build Status    | Wi-Fi |    BLE    |  RF |  FM |   nRF24   | Mic | NFC |  IR | Est. Price (USD) | Notes                                                                       |
| -------------------- | -------------------------- | ----------------------- | --------------- | :---: | :-------: | :-: | :-: | :-------: | :-: | :-: | :-: | ---------------: | --------------------------------------------------------------------------- |
| **ESP32**            | ESP32-DevKitC, ESP32-WROOM | `templates/esp32/`      | ⚙️ In Progress       |   ✅   |     ✅     |  ✅  |  —  |     —     |  ✅  |  ⚙️ |  ✅  |     **$8 – $12** | Full support for Wi-Fi/BLE + optional mic and IR; great for network labs    |
| **STM32**            | Nucleo-F446RE, Blue Pill   | `templates/stm32/`      | ⚙️ In Progress  |   —   |     —     |  ✅  |  —  |     ✅     |  ⚙️ |  —  |  ✅  |    **$10 – $20** | Good RF/nRF24 lab target; mic integration WIP                               |
| **RP2040**           | Raspberry Pi Pico          | `templates/rp2040/`     | ⚙️ In Progress |   —   | ✅ (addon) |  ✅  |  —  |     ✅     |  ✅  |  —  |  ✅  |      **$4 – $8** | Versatile teaching board; supports modular sensors                          |
| **ATmega328P**       | Arduino Uno R3             | `templates/atmega328p/` | ⚙️ In Progress      |   —   |     —     |  ✅  |  —  |     ✅     |  ⚙️ |  —  |  ✅  |    **$12 – $18** | Excellent low-level RF and IR example                                       |
| **ESP8266**          | NodeMCU                    | `templates/esp8266/`    | ⚙️ In Progress  |   ✅   |     —     |  ✅  |  —  |     —     |  —  |  —  |  —  |      **$5 – $8** | Legacy Wi-Fi stack, telemetry only                                          |
| **BBC micro:bit v2** | nRF52833 SoC               | `templates/microbitv2/` | ⚙️ In Progress        |   —   |     ✅     |  ✅  |  —  | ✅ (addon) |  ✅  |  —  |  ✅  |    **$18 – $25** | Built-in BLE, mic, buttons & sensors — ideal for educational security demos |
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
⚠️ Important: Waffles Firmware is for ethical research, education, and defensive testing in controlled environments only.
Do not deploy to devices connected to production networks or devices you do not own/explicitly have permission to test.
If you do not follow these instructions you could face serious trouble.
