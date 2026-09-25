# Hi, I'm Mustafa Ekici

**Senior Automation Engineer & IoT Platform Developer**

I build industrial IoT systems from the ground up — from PLC cabinets on the factory floor to cloud-scale backend architectures. Currently developing a multi-site energy monitoring and control platform serving real production facilities.

---

## What I Do

- **Automation Engineering** — Commissioning large-scale industrial facilities: PLCs, SCADA, field instruments, safety systems. Siemens, Schneider Electric, Delta.
- **Industrial IoT Platform** — Designed and built a multi-tenant SaaS platform for solar and industrial energy management. Gateway firmware → backend microservices → real-time dashboards.
- **On-Premise Deployment** — Enterprise on-prem solution: containerized stack, automated installer, schema migration system, license management.
- **Embedded Gateway** — Custom Python gateway running on Raspberry Pi (DietPi): Modbus TCP/RTU, Siemens S7, OPC-UA, BACnet. SQLite offline buffer, MQTT publish, zero-export PID control.

---

## Tech Stack

**Industrial Protocols & Tools**
- Siemens S7 (snap7 / S7comm), TIA Portal, STEP 7, WinCC, PCS7
- Schneider Electric — EcoStruxure, Unity Pro, Modicon
- Delta PLC & Drives
- Kepware OPC Server (OPC-DA / OPC-UA data aggregation)
- Modbus TCP/RTU, OPC-UA (asyncua), BACnet, SNMP
- IEC 62061 / ISO 13849 (functional safety)

**Backend**
- Python (advanced) — asyncio, FastAPI, SQLAlchemy async
- Apache Kafka (event streaming), MQTT (EMQX broker)
- PostgreSQL / TimescaleDB (continuous aggregates, time-series)
- Redis (caching, pub/sub)

**Infrastructure & DevOps**
- Docker, Docker Compose, GitHub Actions CI/CD
- Cloudflare (Tunnel, DNS, CDN, WAF), Caddy, Nginx
- Tailscale (mesh VPN for remote gateway access)
- Linux server management (Ubuntu, DietPi, Raspberry Pi OS)

**Architecture**
- Multi-tenant SaaS, event-driven microservices
- On-premise containerized deployment
- Zero-export control (PID + ramp + deadband)
- Alarm management system (rules, cooldown, notifications)
- AI inference microservice integration

---

## Projects

### Industrial IoT Platform
Multi-tenant energy monitoring and control platform for solar and industrial facilities.
Built entirely from scratch: custom gateway firmware, FastAPI microservices, real-time MQTT telemetry pipeline, Kafka event streaming, TimescaleDB, dashboard engine with 20+ widget types, alarm system, zero-export controller, on-premise deployment package.

`Python` `FastAPI` `Kafka` `MQTT` `TimescaleDB` `Docker` `Cloudflare`

> Production system — source is private; architecture and components represented in public repos.

---

### [modbus-mqtt-bridge](https://github.com/ekicimustafa/modbus-mqtt-bridge)
Async Python bridge: reads Modbus TCP/RTU registers and publishes to MQTT — single YAML config, Docker-ready. Designed for connecting inverters, energy meters, and PLCs to any MQTT broker.

`Python` `pymodbus` `aiomqtt` `asyncio` `pydantic`

---

### [modbus-s7-mqtt-bridge](https://github.com/ekicimustafa/modbus-s7-mqtt-bridge)
Lightweight Python bridge: polls Modbus TCP/RTU and Siemens S7 PLCs, publishes to MQTT with SQLite offline buffering. Configurable via YAML, runs on Raspberry Pi with < 100 MB RAM.

`Python` `pymodbus` `snap7` `paho-mqtt` `aiosqlite`

---

### [industrial-commissioning-checklist](https://github.com/ekicimustafa/industrial-commissioning-checklist)
8-phase field commissioning checklist based on real large-scale facility commissioning experience. Covers electrical, PLC I/O, SCADA, network, safety (IEC 62061 / ISO 13849), and handover.

`PLC` `SCADA` `Siemens` `Safety` `IEC-62061`

---

## Currently Focused On

- Industrial reliability patterns for IoT gateways (queued commands, redundancy, offline resilience)
- On-premise enterprise deployment at scale
- Dutch language (A0 → A2) — planning to work in the Netherlands

---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-mstfaekici-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/mstfaekici)
[![GitHub](https://img.shields.io/badge/GitHub-ekicimustafa-181717?style=flat&logo=github)](https://github.com/ekicimustafa)

---

*Based in Turkey · Open to opportunities in the Netherlands · Industrial IoT · SCADA · Backend Engineering*
