# VTOL R2 Flight Controller

A single-string flight controller board for a 1.6 m tilt-rotor tricopter VTOL, designed in KiCad 9 and intended to run ArduPilot.

> **Status: design stage, not yet fabricated or bench-tested.** Items marked "simulated" or "assumed" have not been verified on hardware. Do not treat this design as flight-proven.

## Overview

- **Vehicle:** Heewing T1-style tilt-rotor tricopter, 1.6 m span, ~30 min flight time target
- **Firmware target:** ArduPilot
- **Architecture:** single-string (no redundancy)
- **Battery:** 6S Li-ion (6S2P 21700)

## Board

| Item | Value |
|---|---|
| MCU | STM32H743 |
| IMU | BMI270 |
| Barometer | BMP581 |
| Power stage | LT8641 buck, 2 MHz, 5 V rail |
| Size / layers | 70 x 55 mm, 4-layer |
| Servo outputs | 12 x 3-pin headers |
| Other | microSD, USB, SWD, buzzer |
| Fabrication | JLCPCB |

## Current state

- Layout: 0 unrouted nets, 0 DRC errors
- BOM checked against LCSC/JLC part pages
- Power stage simulated in LTspice and ngspice (efficiency figures indicative only, some derating values assumed)
- Not yet fabricated

## Safety

Unvalidated prototype. Do not fly until the board has passed bring-up and bench testing, and always power up first from a current-limited supply.

## License

To be decided.
