# Embedded IoT Journey

A public, 32-week learning log: moving from Arduino and ESP32 hobby projects to professional embedded systems, industrial IoT and automation engineering.

**Started:** 9 November 2026 · **Target finish:** 20 June 2027

**Goal:** become an engineer who can design, program, test, secure and deploy connected microcontroller products, and prove it with three finished projects.

---

## Why I'm doing this

I have been building projects with Arduino and ESP32 for a while. They work, but most of them are hobby-grade: quick prototypes, little testing, almost no documentation. I want to build the way professional engineers do, so that companies in telecom, energy and industry can trust my work.

This repo is my public record of that change. It is not a polished showcase. It is an honest log of what I learn, what I build, and what goes wrong along the way.

## Where I'm starting

- I can wire up and program Arduino and ESP32 boards and get a project working.
- I have not yet worked with professional toolchains, RTOS-based firmware, proper testing, custom PCBs or industrial protocols.
- I'm a student, so I study alongside lectures, labs and exams.

## What I'm committing to

- **Show up every day.** Even on busy days I do one lesson, one small build step and one commit.
- **Build something every Saturday** that runs and is documented.
- **Write in my own words.** My notes explain how I understand things, not copied text.
- **Write down what breaks.** Every week's README has a section on bugs and how I fixed them.
- **Finish three flagship projects** that I can demonstrate and explain in an interview.
- **Prefer depth over breadth.** I would rather understand 20 concepts properly than skim 100.

## How I'll know it worked

By June 2027 I want to be able to walk into an Embedded Systems or Industrial IoT interview and show real, working systems that I designed, built, tested, secured and documented myself.

## A note to anyone reading this

If you are an engineer or recruiter, I would value feedback, especially on my architecture choices and code quality. If you are learning too, feel free to copy the structure and start your own journey log.

---

## How this repo works

- One folder per week (`week-01-c-basics/`, `week-02-pointers/`, ...).
- Every week folder has its own `README.md` with what I learned, what I built, what broke and how I fixed it.
- Every Saturday ends with a small build that runs and is documented.
- Topics I want to keep long-term go in [`notes/`](notes/).
- The three flagship projects live in their own repos (linked below).

```
embedded-iot-journey/
  README.md          <- this file: index and progress tracker
  notes/             <- reusable notes (pointers, I2C, MQTT QoS, ...)
  week-01-c-basics/
    README.md
    bitlib/
  week-02-pointers/
    README.md
    ring_buffer/
  ...
```

---

## Flagship projects

| # | Project | Weeks | Repo | Status |
|---|---------|-------|------|--------|
| 1 | Cellular remote-monitoring node (NB-IoT/LTE-M, mutual-TLS MQTT, battery budget) | 16-17 | *coming* | ⬜ |
| 2 | Industrial Modbus-to-MQTT gateway | 18-24 | *coming* | ⬜ |
| 3 | Capstone: industrial IoT monitoring system (custom PCB, RTOS, cloud, OTA, security) | 27-30 | *coming* | ⬜ |

Each flagship repo includes: system architecture, schematics, bill of materials, firmware documentation, test report, README and a demo video.

---

## Progress

Status key: ⬜ not started · 🔄 in progress · ✅ done

### Phase 1: Foundations

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 1 | C fundamentals | Bit-manipulation library with tests | ⬜ |
| 2 | Pointers and memory | Ring buffer + traffic-light state machine | ⬜ |
| 3 | Electronics foundations | MOSFET relay driver + battery monitor | ⬜ |
| 4 | Linux, Git, networking, serial | UART packet protocol (C + Python) | ⬜ |

### Phase 2: Microcontroller architecture and bare-metal

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 5 | ARM Cortex-M and STM32 basics | Interrupt-driven LED patterns | ⬜ |
| 6 | Timers, PWM, ADC, DMA | ADC + DMA data logger with fan control | ⬜ |
| 7 | UART, I2C, SPI | Sensor node with UART console | ⬜ |
| 8 | Debugging, memory, low power, bootloaders | Low-power logger with flash storage | ⬜ |
| 9 | ESP32 with ESP-IDF | ESP-IDF sensor node (Wi-Fi, SNTP, deep sleep) | ⬜ |

### Phase 3: RTOS and professional firmware

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 10 | FreeRTOS I | Multi-task sensor pipeline | ⬜ |
| 11 | FreeRTOS II and architecture | Layered firmware with state machine and fault log | ⬜ |
| 12 | C++, testing, CI | Unit tests + CI + static analysis | ⬜ |
| 13 | LTE/5G architecture, SIM provisioning, sensors, motors | Calibrated multi-sensor module | ⬜ |

### Phase 4: Protocols and connectivity

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 14 | MQTT and TLS | Mutual-TLS telemetry with offline buffer | ⬜ |
| 15 | HTTP, CoAP, LwM2M, BLE | BLE Wi-Fi provisioning | ⬜ |
| 16 | Cellular IoT I | MCU + modem telemetry over TLS | ⬜ |
| 17 | Cellular IoT II, power budgets | **Flagship 1** complete | ⬜ |
| 18 | Modbus, CAN, LoRaWAN theory, network troubleshooting | Modbus-to-MQTT gateway (start of Flagship 2) | ⬜ |

### Phase 5: Cloud, OTA and security

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 19 | Cloud and data | Device to cloud to dashboard with alerts | ⬜ |
| 20 | OTA firmware updates | Signed OTA pipeline with rollback | ⬜ |
| 21 | IoT security | Threat model and security review | ⬜ |

### Phase 6: Hardware design

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 22 | KiCad and PCB design | Capstone board designed and ordered | ⬜ |
| 23 | Assembly, bring-up, manufacturing | Production-test firmware + enclosure design | ⬜ |
| 24 | Standards, gateways, networking, reliability | **Flagship 2** complete | ⬜ |

### Phase 7: Industrial automation and control

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 25 | Control, industrial signals, PLC | Closed-loop PID controller | ⬜ |
| 26 | SCADA, IIoT, safety | IIoT demo with dashboard and alarms | ⬜ |

### Phase 8: Capstone (Flagship 3)

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 27 | Specify and architect | Core sensing + state machine on hardware | ⬜ |
| 28 | Connectivity, cloud, OTA | Integration test + 72-hour soak test | ⬜ |
| 29 | Hardening and testing | Release v1.0.0 | ⬜ |
| 30 | Documentation and showcase | Documentation pack + demo video | ⬜ |

### Phase 9: Job launch

| Week | Topic | Saturday build | Status |
|------|-------|----------------|--------|
| 31 | Interview preparation | Final CV, LinkedIn, portfolio | ⬜ |
| 32 | Apply and close | Applications sent | ⬜ |

---

## Skills I am building

| Area | What |
|------|------|
| Languages | C, C++, Python |
| Microcontrollers | STM32 (ARM Cortex-M), ESP32 (ESP-IDF) |
| Firmware | FreeRTOS, state machines, drivers, bootloaders, OTA, unit testing, CI |
| Protocols | MQTT/TLS, HTTP, CoAP, BLE, NB-IoT/LTE-M, LoRaWAN, Modbus, CAN, I2C, SPI, UART |
| Telecom and networking | LTE/5G architecture, SIM provisioning, VLANs, routing, IPv6, VPNs, Wireshark |
| Cloud | AWS IoT Core, Mosquitto, InfluxDB, Grafana, Docker, REST APIs |
| Hardware | KiCad PCB design, power design, bring-up, enclosures |
| Automation | PID control, PLC (ladder), SCADA, OPC UA, Node-RED, IEC 62443 |
| Security | Threat modelling, secure boot, flash encryption, signed OTA |

---

## About me

**Brian Kipruto Chepchieng**, Electrical Technology and Computing student at Moi University, Eldoret, Kenya.

- GitHub: [github.com/Brian44ki](https://github.com/Brian44ki)
- LinkedIn: [linkedin.com/in/brian-kipruto-061799287](https://www.linkedin.com/in/brian-kipruto-061799287)
- Email: chepchiengkipruto@gmail.com

---

## License

Code in this repo is released under the MIT License unless a folder states otherwise. Notes are written in my own words from the resources listed in each week's README.
