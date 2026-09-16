<div align="center">

# 김신우 · bu-xl

**Full-stack Developer · React · TypeScript · Backend · IoT**

제품을 실제로 동작하게 만드는 것을 좋아합니다.
웹 프론트엔드부터 모바일, 백엔드, 실시간 데이터, 하드웨어까지 직접 연결합니다.

<br />

<a href="https://github.com/bu-xl?tab=repositories">
  <img src="https://img.shields.io/badge/GitHub-Projects-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Projects" />
</a>
<a href="https://github.com/bu-xl/talktail_gait_web">
  <img src="https://img.shields.io/badge/TalkTail-Gait%20Viewer-FF8A00?style=for-the-badge" alt="TalkTail Gait Viewer" />
</a>

</div>

---

## About

저는 **아이디어 → 제품 → 데이터 → 운영**까지 이어지는 개발을 지향합니다.

- 🖥️ **Frontend** — React, Vite, TypeScript
- 📱 **Mobile** — React Native
- ⚙️ **Backend** — Node.js, Express, REST API
- 📡 **Realtime** — MQTT, WebSocket / Socket.IO
- 🔌 **IoT / Embedded** — ESP32, BLE, FreeRTOS
- 📊 **Data** — Sensor data processing, visualization, CSV/PDF reporting
- 🧰 **DevOps** — Linux, Nginx, PM2, SSL, GitHub
- 🤖 **AI-assisted Development** — AI tools를 활용한 설계, 구현, 리뷰, 자동화

> **Build it. Connect it. Measure it. Improve it.**

---

## Featured Work

### 🐾 TalkTail Gait

실시간 압력 매트 데이터를 수집하고 시각화하며, 기록된 보행 데이터를 기반으로 canine gait analysis를 수행하는 프로젝트입니다.

**핵심 기술**

`TypeScript` `Web Serial` `Electron` `Canvas` `Signal Processing` `Gait Analysis`

**주요 기능**

- 실시간 40×40 압력 매트 데이터 처리
- Serial frame parsing / resync
- Baseline calibration & pressure normalization
- 실시간 heatmap rendering
- CoP / pressure statistics
- Canine paw tracking & gait analysis
- CSV / PDF / GIF / PNG export
- Browser + Electron 동일 processing pipeline

[View repository →](https://github.com/bu-xl/talktail_gait_web)

---

### 🐶 TalkTail Platform

반려동물의 생체·활동 데이터를 디바이스에서 수집하고 서버와 애플리케이션으로 연결하는 실시간 IoT 플랫폼을 개발하고 있습니다.

```text
Wearable / Sensor
       ↓ BLE
     Hub
       ↓ MQTT
   Backend
       ↓ WebSocket / REST
 Web / Mobile App
```

관련 프로젝트:

- `talktail_B2C_APP`
- `talktail-B2C-backend`
- `talktail_gait_web`
- `hub_project`
- `talktail_hub_app`

---

## Tech Stack

<div align="center">

### Frontend

<img src="https://skillicons.dev/icons?i=react,vite,ts,html,css" alt="Frontend stack" />

### Backend

<img src="https://skillicons.dev/icons?i=nodejs,express,mysql,nginx" alt="Backend stack" />

### Mobile / Embedded

<img src="https://skillicons.dev/icons?i=react,androidstudio,arduino" alt="Mobile and embedded stack" />

### Tools

<img src="https://skillicons.dev/icons?i=git,github,linux,docker,vscode" alt="Tools" />

</div>

---

## Engineering Focus

```text
Frontend
├── React + TypeScript
├── Component architecture
├── State management
├── Data visualization
└── Performance optimization

Backend
├── Node.js + Express
├── REST API
├── Authentication / Authorization
├── Database design
├── Realtime communication
└── Production deployment

IoT
├── BLE
├── MQTT
├── ESP32
├── Sensor data pipelines
├── OTA
└── Realtime device management
```

---

## Current Direction

### From UI development → product engineering

단순히 화면을 만드는 것보다 **전체 시스템의 흐름을 이해하고 직접 연결하는 것**에 집중하고 있습니다.

```text
Product
   │
   ├── UX / UI
   │
   ├── Frontend
   │
   ├── Mobile
   │
   ├── Backend / API
   │
   ├── Realtime Data
   │
   ├── IoT / Embedded
   │
   └── Deployment / Operations
```

앞으로는 대규모 서비스의 **architecture, reliability, observability, automated testing**까지 더 깊게 다루는 것을 목표로 합니다.

---

## GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=bu-xl&show_icons=true&hide_border=true&rank_icon=github&include_all_commits=true" height="170" alt="GitHub statistics" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bu-xl&layout=compact&hide_border=true&langs_count=8" height="170" alt="Top languages" />

<br />

<img src="https://streak-stats.demolab.com?user=bu-xl&hide_border=true" alt="GitHub streak" />

</div>

---

## Selected Repositories

| Project | Description | Stack |
|---|---|---|
| [TalkTail Gait Web](https://github.com/bu-xl/talktail_gait_web) | Pressure mat & canine gait analysis | TypeScript · Electron · Web Serial |
| [TalkTail B2C App](https://github.com/bu-xl/talktail_B2C_APP) | TalkTail mobile application | React Native |
| [TalkTail B2C Backend](https://github.com/bu-xl/talktail-B2C-backend) | Application backend | Node.js · Express |
| [Server Monitor](https://github.com/bu-xl/server-monitor) | Server monitoring project | Web · Backend |
| [Inventory Management](https://github.com/bu-xl/inventory-management) | Inventory management system | Web · Backend |

---

## Development Philosophy

> **Make the architecture simple enough to understand, and robust enough to survive production.**

- Prefer explicit types over `any`
- Keep data flow observable
- Separate domain logic from rendering
- Design APIs before coupling clients to them
- Optimize after measuring actual bottlenecks
- Automate repetitive development work
- Treat hardware, backend and frontend as one system when the product requires it

---

<div align="center">

### Thanks for visiting 👋

[![GitHub](https://img.shields.io/badge/GitHub-bu--xl-181717?style=flat-square&logo=github)](https://github.com/bu-xl)

</div>
