<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF8A00,100:FF3D00&height=180&section=header&text=%EA%B9%80%EC%8B%A0%EC%9A%B0%20%C2%B7%20bu-xl&fontSize=44&fontColor=ffffff&fontAlignY=38&desc=Web%20%C2%B7%20Mobile%20%C2%B7%20Backend%20%C2%B7%20IoT%20%2F%20Embedded&descSize=18&descAlignY=60" width="100%" alt="header" />

<div align="center">

**Product Engineer** — 웹 · 모바일 · 백엔드 · 펌웨어를 하나의 제품으로 연결합니다.<br/>
현재 크림오프(cream-off)에서 반려동물 생체신호 모니터링 제품 **TalkTail**을 만들고 있습니다.

<a href="https://github.com/bu-xl?tab=repositories"><img src="https://img.shields.io/badge/Repositories-181717?style=flat-square&logo=github&logoColor=white" alt="Repositories"/></a>
<a href="https://github.com/bu-xl/talktail_gait_web"><img src="https://img.shields.io/badge/TalkTail%20Gait%20Viewer-FF8A00?style=flat-square&logo=electron&logoColor=white" alt="TalkTail Gait"/></a>
<a href="https://www.instagram.com/elsels_dn/"><img src="https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white" alt="Instagram"/></a>
<img src="https://komarev.com/ghpvc/?username=bu-xl&style=flat-square&color=FF8A00&label=views" alt="views"/>

</div>

<br/>

## 🧩 Tech Stack

<table>
<tr>
<td align="right"><b>Frontend</b></td>
<td>
<img src="https://skillicons.dev/icons?i=react,ts,vite,electron" height="36" alt="React TypeScript Vite Electron"/>&nbsp;
<img src="https://img.shields.io/badge/Zustand-443E38?style=flat-square" alt="Zustand"/>
<img src="https://img.shields.io/badge/Recharts-22B5BF?style=flat-square" alt="Recharts"/>
<img src="https://img.shields.io/badge/Web%20Serial-4285F4?style=flat-square&logo=googlechrome&logoColor=white" alt="Web Serial"/>
</td>
</tr>
<tr>
<td align="right"><b>Mobile</b></td>
<td>
<img src="https://skillicons.dev/icons?i=react" height="36" alt="React Native"/>&nbsp;
<img src="https://img.shields.io/badge/React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React Native"/>
<img src="https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white" alt="Expo"/>
<img src="https://img.shields.io/badge/BLE-0082FC?style=flat-square&logo=bluetooth&logoColor=white" alt="BLE"/>
<img src="https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white" alt="Socket.IO"/>
</td>
</tr>
<tr>
<td align="right"><b>Backend</b></td>
<td>
<img src="https://skillicons.dev/icons?i=nodejs,express,mysql,prisma,sequelize" height="36" alt="Node.js Express MySQL Prisma Sequelize"/>&nbsp;
<img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
<img src="https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white" alt="MQTT"/>
<img src="https://img.shields.io/badge/S3-569A31?style=flat-square" alt="S3"/>
</td>
</tr>
<tr>
<td align="right"><b>Firmware</b></td>
<td>
<img src="https://skillicons.dev/icons?i=c,cpp" height="36" alt="C C++"/>&nbsp;
<img src="https://img.shields.io/badge/ESP32--S3-E7352C?style=flat-square&logo=espressif&logoColor=white" alt="ESP32-S3"/>
<img src="https://img.shields.io/badge/ESP--IDF%20%2F%20FreeRTOS-E7352C?style=flat-square" alt="ESP-IDF FreeRTOS"/>
<img src="https://img.shields.io/badge/nRF5340-00A9CE?style=flat-square&logo=nordicsemiconductor&logoColor=white" alt="nRF5340"/>
<img src="https://img.shields.io/badge/Zephyr%20%2F%20NCS-2E3440?style=flat-square" alt="Zephyr NCS"/>
<img src="https://img.shields.io/badge/MCUboot%20DFU-2E3440?style=flat-square" alt="MCUboot"/>
</td>
</tr>
<tr>
<td align="right"><b>Ops</b></td>
<td>
<img src="https://skillicons.dev/icons?i=linux,nginx,docker,git,github" height="36" alt="Linux Nginx Docker Git GitHub"/>&nbsp;
<img src="https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white" alt="PM2"/>
</td>
</tr>
</table>

<br/>

## 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🐾 TalkTail Gait Viewer
<a href="https://github.com/bu-xl/talktail_gait_web"><img src="https://img.shields.io/badge/bu--xl%2Ftalktail__gait__web-181717?style=flat-square&logo=github&logoColor=white" alt="repo"/></a>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TS"/>
<img src="https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white" alt="Electron"/>
<img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/>

40×40 USB-Serial 압력 매트를 실시간 히트맵으로 그리고, 기록한 보행 데이터로 반려견 보행 분석을 수행하는 뷰어. Qt6/C++ 수집 프로그램을 TypeScript로 재구현해 **브라우저(Web Serial)와 Electron이 같은 파이프라인**을 씁니다.

- 3 Mbps 시리얼 프레임 파싱 · header resync · 부분 프레임 처리
- per-cell median 베이스라인 캘리브레이션 · EMA 스무딩
- Canvas 히트맵 (upsample → Gaussian blur → colormap)
- 보행 엔진: Hungarian tracking · contact hysteresis · CoP 기반 방향 · LF/RF/LH/RH 라벨링
- CSV · PDF · GIF · PNG export (PDF writer · GIF 인코더 직접 구현)
- `node --test` 41개 · electron-builder Win/mac 배포

</td>
<td width="50%" valign="top">

### 🐶 TalkTail Platform
<img src="https://img.shields.io/badge/cream--off-FF8A00?style=flat-square" alt="cream-off"/>
<img src="https://img.shields.io/badge/source-private-lightgrey?style=flat-square" alt="private"/>
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React"/>
<img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" alt="Express"/>
<img src="https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white" alt="MQTT"/>

웨어러블(PPG · 온도 · IMU) → BLE → 허브 → MQTT → 서버 → 웹/앱으로 이어지는 실시간 IoT 플랫폼. 프론트엔드 · 백엔드 · 모바일 앱을 주로 담당하고 허브·디바이스 펌웨어 작업에 참여합니다.

- **Web** — 실시간 생체 차트, 디바이스/허브 관리, i18n, 브라우저 펌웨어 플래싱(esptool-js)
- **Backend** — 허브 제어 API, MQTT 연동, Socket.IO 브로드캐스트, JWT, S3, OTA 배포 API
- **App** — BLE 페어링 · Wi-Fi 프로비저닝 · 실시간 스트리밍 · 푸시 알림
- **Contract** — BLE / MQTT / REST / Socket / OTA 계약 문서화, 무유실 전송(seq + ACK + 재전송 + dedup)
- **Firmware** — ESP32-S3 허브(BLE client · MQTT · OTA), nRF5340 디바이스(BLE 서비스 · 센서 · DFU)

</td>
</tr>
</table>

<br/>

## 🏗️ TalkTail Architecture

```mermaid
flowchart LR
    D["🐕 Device<br/>nRF5340 · Zephyr/NCS<br/>PPG · 온도 · IMU · MCUboot DFU"]
    H["📡 Hub<br/>ESP32-S3 · ESP-IDF<br/>BLE central · MQTT · OTA"]
    S["🖥️ Server<br/>Node.js · Express<br/>MySQL · Socket.IO · S3"]
    W["🌐 Web<br/>React · TypeScript<br/>Zustand · Recharts"]
    A["📱 App<br/>React Native · Expo<br/>BLE · Socket.IO"]
    D -- "BLE GATT" --> H
    H -- "MQTT / HTTP" --> S
    S -- "Socket.IO / REST" --> W
    S -- "Socket.IO / REST" --> A
    A -. "BLE 페어링" .-> D
    style D fill:#00A9CE,stroke:#00A9CE,color:#fff
    style H fill:#E7352C,stroke:#E7352C,color:#fff
    style S fill:#339933,stroke:#339933,color:#fff
    style W fill:#3178C6,stroke:#3178C6,color:#fff
    style A fill:#20232A,stroke:#61DAFB,color:#61DAFB
```

```mermaid
flowchart LR
    P["USB Serial<br/>3 Mbps · 3206 B frame"] --> F["SerialFrameParser<br/>header 탐색 · resync"]
    F --> C["PressureCalibrator<br/>median baseline · delta · threshold"]
    C --> E["TemporalSmoother<br/>EMA"]
    E --> R["Heatmap<br/>upsample · blur · colormap"]
    E --> G["Gait Engine<br/>contact · tracking · labeling"]
    R --> X["CSV · PDF · GIF · PNG"]
    G --> X
    style P fill:#FF8A00,stroke:#FF8A00,color:#fff
    style X fill:#FF8A00,stroke:#FF8A00,color:#fff
```

<br/>

## 🎯 Engineering Focus

<table>
<tr>
<td align="center" width="25%"><h3>🖥️</h3><b>Frontend</b><br/><sub>React + TypeScript<br/>상태 소유권 · 데이터 시각화<br/>Electron 데스크톱</sub></td>
<td align="center" width="25%"><h3>⚙️</h3><b>Backend</b><br/><sub>Express REST · 인증/인가<br/>MySQL · Socket.IO / MQTT<br/>PM2 운영</sub></td>
<td align="center" width="25%"><h3>📱</h3><b>Mobile</b><br/><sub>React Native · Expo<br/>BLE · Wi-Fi 프로비저닝<br/>백그라운드 알림</sub></td>
<td align="center" width="25%"><h3>🔌</h3><b>Embedded</b><br/><sub>ESP-IDF · Zephyr<br/>BLE GATT · OTA / DFU<br/>센서 파이프라인</sub></td>
</tr>
</table>

<br/>

## 📂 Selected Repositories

| Project | Description | Stack |
|---|---|---|
| [**talktail_gait_web**](https://github.com/bu-xl/talktail_gait_web) | 압력 매트 실시간 히트맵 + 반려견 보행 분석 뷰어 | ![](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![](https://img.shields.io/badge/-Electron-47848F?style=flat-square&logo=electron&logoColor=white) ![](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=vite&logoColor=white) |
| [**server-monitor**](https://github.com/bu-xl/server-monitor) | Ubuntu 서버 오류·상태를 매일 00시에 정리해 이메일로 보내는 데몬 | ![](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![](https://img.shields.io/badge/-SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) |
| [**h100_fastapi**](https://github.com/bu-xl/h100_fastapi) | Image-to-Image AI 웹 서비스 (Z-Image-Turbo) | ![](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![](https://img.shields.io/badge/-React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |
| [**kitae-backend**](https://github.com/bu-xl/kitae-backend) | 패션 이커머스 백엔드 — 인증 · 상품 · 장바구니 · 주문 | ![](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white) ![](https://img.shields.io/badge/-Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white) ![](https://img.shields.io/badge/-JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white) |
| [**inventory-management_backend**](https://github.com/bu-xl/inventory-management_backend) | 재고 관리 API | ![](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white) ![](https://img.shields.io/badge/-Sequelize-52B0E7?style=flat-square&logo=sequelize&logoColor=white) ![](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |
| [**print**](https://github.com/bu-xl/print) | 프린터 목록 조회·출력용 Windows 서비스, exe 패키징 | ![](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white) |
| [**gap-cli**](https://github.com/bu-xl/gap-cli) | `git add · commit · push`를 한 줄로 끝내는 CLI | ![](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) |

<br/>

## 📊 GitHub Activity

<div align="center">

<img src="https://streak-stats.demolab.com?user=bu-xl&hide_border=true&ring=FF8A00&fire=FF8A00&currStreakLabel=FF8A00&sideNums=1F2328&sideLabels=57606A&dates=57606A&currStreakNum=1F2328&background=FFFFFF00" alt="GitHub streak" />

<br/><br/>

<img src="https://ghchart.rshah.org/FF8A00/bu-xl" width="100%" alt="Contribution graph" />

</div>

<br/>

## 💬 Development Philosophy

> **Make the architecture simple enough to understand, and robust enough to survive production.**

<table>
<tr>
<td>🔒 <code>any</code> 대신 명시적 타입</td>
<td>👁️ 데이터 흐름은 관찰 가능하게</td>
<td>🧱 도메인 로직과 렌더링 분리</td>
</tr>
<tr>
<td>📐 클라이언트를 붙이기 전에 API 계약부터</td>
<td>⏱️ 측정한 뒤에 최적화</td>
<td>🔗 하드웨어 · 백엔드 · 프론트엔드를 하나의 시스템으로</td>
</tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF8A00,100:FF3D00&height=100&section=footer" width="100%" alt="footer" />
