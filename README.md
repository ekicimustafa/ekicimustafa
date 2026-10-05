<div align="center">

# Mustafa Ekici

**OT/IT Integration Engineer** · Industrial Automation & IoT Platforms

🇹🇷 Turkey → Netherlands 🇳🇱

![Open to work](https://img.shields.io/badge/⚡_Open_to_work_in_NL-F7A823?style=flat&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/TimescaleDB-black?style=flat&logo=postgresql)

</div>

---

## 🔌 What I Build

I engineer production IoT platforms — from industrial protocol connectors and
high-throughput telemetry pipelines to real-time SCADA dashboards.

On the OT side: I've commissioned Siemens S7 and Modbus RTU/TCP systems in the field
and built the gateway layer that bridges them to cloud pipelines.

Currently shipping **[SolarTools](https://www.solartools.io)**, deployed at solar farms and cold-storage
facilities across Turkey.

```text
Industrial Devices → Gateway (Modbus/S7/OPC-UA) → MQTT/EMQX → Kafka → TimescaleDB → Dashboard
```

## 🧰 Tech Stack

| Layer | Stack |
|---|---|
| **Languages** | Python · Go · SQL · Ladder · FBD |
| **PLC / SCADA** | Siemens TIA Portal (S7-1500/1200) · WinCC · PCS7 · Schneider Unity Pro (Modicon M340/M580) · Delta |
| **Industrial** | Modbus RTU/TCP · Siemens S7 · OPC-UA · IEC 60870-5-104 · PROFINET |
| **Backend** | FastAPI · SQLAlchemy · asyncpg · Kafka |
| **Messaging** | MQTT (EMQX) · Redis · WebSocket |
| **Database** | TimescaleDB · PostgreSQL |
| **Infra** | Docker · GitHub Actions · Tailscale · Cloudflare Tunnel |
| **Gateway HW** | Raspberry Pi · DietPi · ARM Linux |
| **Product** | System architecture and SCADA/HMI UX direction, driven by field experience |

## ⚡ Featured — SolarTools

A ThingsBoard-class industrial IoT platform that I architected and built end to end:
edge gateway, message pipeline, multi-tenant backend, infrastructure and on-premise delivery.
It monitors and controls **10+ industrial sites** in real time.

📐 **Full architecture write-up with diagrams:** [solartools-architecture](https://github.com/ekicimustafa/solartools-architecture)

```text
Field devices → Edge gateway → EMQX (MQTT) → Kafka → Telemetry workers → TimescaleDB → API → Dashboards · Alarms · Reports
                     ▲                                                                       │
                     └──────────────── Commands (RPC) with status tracking ◄─────────────────┘
```

**🛰️ Edge**
- Python edge gateway on Raspberry Pi / DietPi with Modbus TCP/RTU, Siemens S7, OPC-UA, BACnet, SNMP and REST connectors
- Offline SQLite buffer, remote config deploy, over-the-air updates and watchdogs, so no data is lost when the link drops

**🔀 Data pipeline**
- EMQX → Kafka → horizontally scaled telemetry workers → TimescaleDB, with **850× compression** on telemetry
- Two-way commands from the dashboard down to the PLC, with delivery and result tracking

**🏗️ Platform**
- Multi-tenant FastAPI backend: 100+ endpoints, role-based access, OpenAPI docs
- Device and gateway management, a dashboard/widget engine and virtual (computed) signals
- 🔔 Alarm system with SMS and e-mail notifications, cooldowns and quiet hours; PDF reporting (in progress)
- Integrations with Huawei FusionSolar, NetEco and Enerjisa; subscription billing (TRY/USD)
- AI model integration for forecasting and anomaly detection (TÜBİTAK-funded R&D)

**🎮 Control**
- ☀️ **Zero-export control** for grid-connected solar inverters
- **SCADA-grade command path:** guaranteed delivery, no duplicate execution and no lost commands across restarts; write readback and device-offline checks in progress

**🚀 Infrastructure & delivery**
- Dockerised services, GitHub Actions CI/CD to staging and production, container registry
- Cloudflare Tunnel for zero-trust access, Redis caching
- **On-premise edition** for air-gapped industrial sites: installer, license server, schema-migration tracking, backup/restore

## 🌱 Currently

- 🔧 Shipping SolarTools on-premise edition
- 📊 Building SCADA command reliability (GAP series) & PDF reporting
- 🌍 Actively looking for opportunities in the **Netherlands**
- 🇳🇱 Learning Dutch · English B2+
- ⚡ Exploring distributed systems & cloud-native IoT patterns

## 📈 GitHub Stats

![Mustafa's GitHub stats](https://github-readme-stats.vercel.app/api?username=ekicimustafa&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=F7A823&icon_color=F7A823)

---

<div align="center">
  <sub>Building reliable industrial software, one commit at a time.</sub>
</div>
