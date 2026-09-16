<div align="center">

# 김신우 · bu-xl

**Product Engineer — Web · Mobile · Backend · IoT/Embedded**

웹 프론트엔드에서 시작해 모바일 앱, 백엔드, 실시간 통신, 펌웨어까지
하나의 제품으로 이어 붙이는 개발을 합니다. 현재 크림오프(cream-off)에서
반려동물 생체신호 모니터링 제품 **TalkTail**을 만들고 있습니다.

</div>

---

## Tech Stack

| 영역 | 실제 사용 중 |
|---|---|
| Frontend | React, TypeScript, Vite, Zustand, Recharts, Electron |
| Mobile | React Native (Expo), BLE (`react-native-ble-manager`), Socket.IO client |
| Backend | Node.js, Express, MySQL (Sequelize / Prisma), JWT, Socket.IO, MQTT, S3 |
| Realtime / IoT | MQTT, WebSocket, BLE GATT, Web Serial, OTA |
| Firmware | ESP32-S3 (ESP-IDF, FreeRTOS), nRF5340 (Zephyr / nRF Connect SDK, MCUboot) |
| Ops | Linux, Nginx, PM2, Docker, GitHub |

---

## Featured Projects

### 🐾 TalkTail Gait Viewer — [bu-xl/talktail_gait_web](https://github.com/bu-xl/talktail_gait_web)

40×40 USB-Serial 압력 매트를 실시간으로 읽어 히트맵으로 그리고, 기록한 보행 데이터로 반려견 보행 분석(canine gait analysis)을 수행하는 뷰어입니다. 기존 Qt6/C++ 수집 프로그램을 TypeScript 파이프라인으로 다시 구현해 **브라우저(Web Serial)와 Electron(node-serialport)이 같은 처리 코드**를 씁니다.

```text
USB Serial (3 Mbps, 3206-byte frame)
      ↓  SerialFrameParser — header 탐색 · resync · 부분 프레임 처리
40×40 raw matrix
      ↓  PressureCalibrator — per-cell median baseline · delta · threshold
      ↓  TemporalSmoother — EMA
Heatmap (Canvas: upsample → Gaussian blur → colormap)
      ↓
Stats (max / avg / contact area)  ·  Gait engine (contact → tracking → labeling → features)
      ↓
CSV · PDF · GIF · PNG export
```

- 보행 엔진: Hungarian tracking, contact hysteresis, CoP 회귀 기반 진행 방향, LF/RF/LH/RH 발 라벨링, 좌우·전후 균형 지표
- 라이브 발 라벨 오버레이 + 기록 후 일괄 분석 결과를 모든 export에 동일하게 적용
- 외부 의존성 없이 직접 만든 one-page PDF writer, GIF 인코딩
- `node --test` 기반 테스트 41개 (프레임 resync, 멀티 프레임 버퍼, PDF 컨테이너)
- Windows / macOS 배포 빌드 (electron-builder)

### 🐶 TalkTail Platform (회사 제품 · 소스 비공개)

웨어러블 디바이스에서 PPG · 온도 · IMU를 수집해 허브를 거쳐 서버와 웹/앱으로 전달하는 실시간 IoT 플랫폼입니다. 프론트엔드·백엔드·모바일 앱을 주로 담당하고, 허브·디바이스 펌웨어 작업에도 참여합니다.

```text
Device  nRF5340 · Zephyr/NCS · PPG/온도/IMU · MCUboot DFU
   │  BLE GATT (custom NUS)
Hub     ESP32-S3 · ESP-IDF · BLE central + MQTT client · OTA
   │  MQTT / HTTP
Server  Node.js · Express · MySQL · Socket.IO · S3
   │  Socket.IO / REST
Web     React · TypeScript · Zustand · Recharts · MQTT over WebSocket
App     React Native (Expo) · BLE 페어링 · Socket.IO
```

**직접 만든 것**

- 웹 대시보드 (React + TypeScript): 실시간 생체 데이터 차트, 디바이스/허브 관리, i18n, 브라우저에서 허브 펌웨어 플래싱(esptool-js)
- 백엔드 (Express + MySQL): 허브 제어 API, MQTT 브로커 연동, Socket.IO 실시간 브로드캐스트, JWT 인증, S3 파일 저장, OTA 배포 API
- 모바일 앱 (React Native / Expo): BLE 디바이스 페어링 및 Wi-Fi 프로비저닝, 실시간 스트리밍, 푸시 알림
- 프로토콜 계약: BLE 패킷 · MQTT 토픽 · REST · Socket 이벤트 · OTA 절차를 문서로 고정하고 계층 간 무유실(seq + ACK + 재전송 + dedup) 규칙 정의
- 펌웨어: ESP32-S3 허브(BLE GATT client, MQTT, OTA, FreeRTOS task 구조), nRF5340 디바이스(BLE 서비스, 센서 드라이버, DFU) 유지보수

---

## Engineering Focus

```text
Frontend   React + TypeScript · 상태 소유권 · 데이터 시각화 · Electron 데스크톱
Backend    Express REST · 인증/인가 · MySQL 스키마 · Socket.IO / MQTT · PM2 운영
Mobile     React Native · BLE · 백그라운드 알림
Embedded   ESP-IDF · Zephyr · BLE GATT · OTA/DFU · 센서 파이프라인
Reliability 무유실 전송 · 자동 재연결 · 정직한 상태 표시(유령 온라인 금지, 무한 스피너 금지)
```

---

## Selected Repositories

| Project | Description | Stack |
|---|---|---|
| [talktail_gait_web](https://github.com/bu-xl/talktail_gait_web) | 압력 매트 실시간 히트맵 + 반려견 보행 분석 뷰어 | TypeScript · Vite · Electron · Canvas · Web Serial |
| [server-monitor](https://github.com/bu-xl/server-monitor) | Ubuntu 서버 오류·상태를 매일 00시에 정리해 이메일로 보내는 데몬 | TypeScript · Node.js · node-cron · systeminformation · SQLite · nodemailer |
| [h100_fastapi](https://github.com/bu-xl/h100_fastapi) | Image-to-Image AI 웹 서비스 (Z-Image-Turbo) | FastAPI · Python · React · Vite · TypeScript · Docker |
| [kitae-backend](https://github.com/bu-xl/kitae-backend) | 패션 이커머스 백엔드 — 인증, 상품, 장바구니, 주문 | Node.js · Express · Prisma · JWT · Zod |
| [inventory-management_backend](https://github.com/bu-xl/inventory-management_backend) | 재고 관리 API | Node.js · Express · Sequelize · MySQL |
| [print](https://github.com/bu-xl/print) | 프린터 목록 조회·출력용 Windows 서비스, exe 패키징 | Node.js · Express · node-windows · pkg |
| [gap-cli](https://github.com/bu-xl/gap-cli) | `git add · commit · push`를 한 줄로 끝내는 CLI | Node.js |

---

## GitHub Activity

<div align="center">

<img src="https://streak-stats.demolab.com?user=bu-xl&hide_border=true" alt="GitHub streak" />

</div>

---

## Development Philosophy

> **Make the architecture simple enough to understand, and robust enough to survive production.**

- `any` 대신 명시적 타입
- 데이터 흐름은 관찰 가능하게
- 도메인 로직과 렌더링 분리
- 클라이언트를 붙이기 전에 API 계약부터
- 측정한 뒤에 최적화
- 하드웨어·백엔드·프론트엔드를 하나의 시스템으로
