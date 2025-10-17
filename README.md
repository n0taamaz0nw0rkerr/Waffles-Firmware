Waffles Firmware

Ethical hacking & defensive cybersecurity firmware for embedded devices
Lightweight, audit-friendly firmware and tooling designed for responsible security research, lab-based pentesting, and device hardening practice. Built with transparency, testability, and strong ethical safeguards at the core.

Key features

Minimal, auditable firmware stack for common microcontrollers (template-based, hardware-agnostic).

Secure boot & basic runtime integrity checks (reference implementations).

Safe, sandboxed diagnostic tools for network/USB/serial observation in lab environments.

Logging & forensics hooks to capture reproducible test artifacts.

CI-friendly build matrix and firmware signing examples.

Developer-focused: comprehensive docs, unit tests, and example lab topologies.

Strong emphasis on legality, consent and responsible disclosure — for research/use in controlled environments only.

🧠 Supported Devices & Interfaces
Platform / MCU	Board Example	Template	Build Status	Wi-Fi	BLE	RF	FM	nRF24	Mic	NFC	IR	Notes
ESP32	ESP32-DevKitC, ESP32-WROOM	templates/esp32/	✅ Stable	✅	✅	✅	—	—	✅	⚙️	✅	Full support for Wi-Fi/BLE + optional mic input and IR; great for network labs
STM32	Nucleo-F446RE, Blue Pill	templates/stm32/	⚙️ In Progress	—	—	✅	—	✅	⚙️	—	✅	Good RF/nRF24 lab target; mic integration WIP
RP2040	Raspberry Pi Pico	templates/rp2040/	🚧 Experimental	—	✅ (addon)	✅	—	✅	✅	—	✅	Versatile teaching board; supports modular sensors
ATmega328P	Arduino Uno	templates/atmega328p/	✅ Stable	—	—	✅	—	✅	⚙️	—	✅	Excellent low-level RF and IR example
ESP8266	NodeMCU	templates/esp8266/	⚙️ In Progress	✅	—	✅	—	—	—	—	—	Legacy Wi-Fi stack, telemetry only
x86 VM Simulator	QEMU / VirtualBox	templates/sim/	✅ Stable	Sim	Sim	Sim	Sim	Sim	Sim	Sim	Sim	Perfect for safe virtual labs, CI, and firmware logic testing

✅ = Supported ⚙️ = In Progress 🚧 = Experimental — = Not applicable Sim = Simulated support (no real hardware access)

🧩 More devices and modules (ESP32-S3, Teensy 4.1, Raspberry Pi CM4) are planned. Contributions for new interfaces welcome — see CONTRIBUTING.md.

Who it's for

Security researchers building reproducible embedded-device tests.

Red-team/blue-team labs that need a safe, auditable firmware baseline.

Educators teaching secure embedded development and ethical hacking.

Device teams who want a reference for hardening their own firmware.

Quick start (safe, high-level)

Clone the repo.

Pick the device template matching your lab hardware (e.g., templates/esp32).

Build with the provided Makefile/CMake scripts.

Flash only to lab-owned, consented devices or contained hardware-in-the-loop rigs.

Use the included test suite and VM-based sims before running on physical devices.

⚠️ Important: Waffles Firmware is for ethical research, education, and defensive testing in controlled environments only.
Do not deploy to devices connected to production networks or devices you do not own/explicitly have permission to test.

Example repo README badges
[![Build Status](https://img.shields.io/github/actions/workflow/status/your-org/waffles-firmware/ci.yml?branch=main)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)]()
[![Issues Welcome](https://img.shields.io/badge/Issues-welcome-brightgreen)]()

Project layout
/docs               # Design docs, threat model, lab setup guides
/src                # Firmware source (device templates)
/tools              # Helper scripts (builders, signers, log parsers)
/tests              # Unit & integration tests + simulation harness
/examples           # Example lab topologies and workflows
/CONTRIBUTING.md
/SECURITY.md
/LICENSE

Responsible use & legal / ethical policy

Waffles Firmware is explicitly intended for lawful, consensual security research and defensive testing. By using this project you agree to:

Only run firmware on devices you own or have explicit written permission to test.

Use a segregated lab network or isolated hardware-in-the-loop environment for all tests.

Follow all applicable laws and institutional policies.

Respect privacy; never capture or exfiltrate production data without permission.

Report vulnerabilities responsibly following the SECURITY.md responsible disclosure process.

Contributing

Contributions are welcome — especially improvements that increase safety, auditability, and testability.
Please read CONTRIBUTING.md and SECURITY.md before submitting PRs. Suggested contribution areas:

New device templates and CI build profiles.

Additional defensive features (secure update workflows, attestation examples).

Test suites and simulators for safe validation.

Docs: lab setup, legal checklist, classroom exercises.

License

MIT License — see LICENSE for details.

GitHub Topics

embedded · firmware · cybersecurity · ethical-hacking · pentest-lab · iot-security · secure-boot · forensics · education
