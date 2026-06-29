<div align="center">

<img src="docs/logo.png" width="160">

# QFACE

### Enterprise Face Recognition Platform

High-performance face recognition, real-time monitoring, multi-camera management, and modern administration tools.

[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?logo=python&logoColor=white)]()
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)]()
[![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)]()
[![Electron](https://img.shields.io/badge/Electron-47848F?logo=electron&logoColor=white)]()
[![License](https://img.shields.io/badge/License-AGPLv3-red)]()

<img src="docs/dashboard.png" width="100%">

**QFACE is a complete face recognition ecosystem for building attendance systems, access control, visitor management, security monitoring, and AI-powered identity solutions.**

---

</div>

## Overview

QFACE is composed of three independent applications working together as a single platform.

```
                     QFACE Dashboard
                  React • Vite • Tailwind
                           │
                    REST API / WebSocket
                           │
                ┌──────────┴──────────┐
                │                     │
         QFACE Server          Recognition Engine
         FastAPI + Python      InsightFace / OpenCV
                │
         PostgreSQL / SQLite
                │
         Connected Clients
                │
     Cameras • RTSP • USB • IP Cameras
```

---

# Components

| Repository | Description |
|------------|-------------|
| **QFACE-server** | Backend API, authentication, face recognition engine, database, WebSocket services |
| **QFACE-dashboard-front** | Modern web dashboard for administration, monitoring, and system management |
| **QFACE-client** | Desktop application for camera streaming and connecting remote devices |

---

# Features

## Face Recognition

- Real-time recognition
- Face enrollment
- Face search
- Face embeddings
- Recognition history
- Confidence scoring

## Camera Management

- Multiple cameras
- USB cameras
- RTSP streams
- IP cameras
- Live preview
- Camera configuration

## Administration

- User management
- Role-based permissions
- Dashboard
- Logs
- Settings
- Monitoring

## API

- REST API
- WebSocket support
- Authentication
- JSON responses
- OpenAPI documentation

## Deployment

- Windows
- Linux
- Docker
- CPU
- GPU

---

# Technology Stack

| Backend | Frontend | Desktop | AI |
|----------|----------|----------|----|
| FastAPI | React | Electron | InsightFace |
| SQLAlchemy | Vite | Node.js | OpenCV |
| Python | TailwindCSS | Electron Builder | ONNX Runtime |

---

# Project Structure

```
QFACE
│
├── QFACE-server/
│   ├── api/
│   ├── recognition/
│   ├── database/
│   ├── websocket/
│   └── services/
│
├── QFACE-dashboard-front/
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── services/
│
└── QFACE-client/
    ├── electron/
    ├── renderer/
    ├── camera/
    └── updater/
```

---

# Typical Workflow

```
1. Register cameras

        ↓

2. Enroll people

        ↓

3. Start recognition

        ↓

4. Receive recognition events

        ↓

5. Monitor everything from Dashboard
```

---

# Screenshots

| Dashboard | Recognition |
|-----------|-------------|
| ![](docs/dashboard.png) | ![](docs/recognition.png) |

| Person Management | Cameras |
|-------------------|---------|
| ![](docs/persons.png) | ![](docs/cameras.png) |

| Logs | Settings |
|------|----------|
| ![](docs/logs.png) | ![](docs/settings.png) |

---

# Getting Started

Clone the repositories.

```bash
git clone https://github.com/salar-ziaei/QFACE-server

git clone https://github.com/salar-ziaei/QFACE-dashboard-front

git clone https://github.com/salar-ziaei/QFACE-client
```

Follow the setup instructions in each repository.

| Repository | Documentation |
|------------|---------------|
| QFACE-server | README.md |
| QFACE-dashboard-front | README.md |
| QFACE-client | README.md |

---

# Use Cases

- Access Control
- Smart Attendance
- Visitor Management
- Office Security
- School Attendance
- Factory Workforce Tracking
- Smart Buildings
- AI Surveillance
- Employee Verification
- Time & Attendance

---

# Roadmap

- [x] Face Recognition Engine
- [x] Dashboard
- [x] Desktop Client
- [x] WebSocket Communication
- [x] Multi-camera Support
- [ ] Docker Images
- [ ] Kubernetes Deployment
- [ ] Mobile Companion App
- [ ] Face Liveness Detection
- [ ] Distributed Recognition Cluster
- [ ] Analytics Dashboard
- [ ] SDK for Third-party Integrations

---

# Contributing

Contributions are welcome.

If you'd like to improve QFACE:

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a Pull Request.

Bug reports, feature requests, and documentation improvements are always appreciated.

---

# License

QFACE is licensed under the **GNU Affero General Public License v3.0 (AGPLv3)**.

Organizations that wish to integrate QFACE into proprietary software or commercial services without the obligations of the AGPL should obtain a commercial license.

For commercial licensing inquiries, please contact the project maintainer.

---

<div align="center">

### Built with ❤️ by Salar Ziaei

If QFACE helps your project, consider giving it a ⭐

</div>
