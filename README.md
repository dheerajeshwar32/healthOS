# healthOS 🩺📊
> **A Client-Side, Local-First Digital Health & Wellness Telemetry Dashboard with Voice Recognition.**

[![Live Web App](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-00D4AA.svg?style=for-the-badge&logo=github)](https://dheerajeshwar32.github.io/healthOS/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-181717.svg?style=for-the-badge&logo=github)](https://github.com/dheerajeshwar32/healthos)

[![Architecture](https://img.shields.io/badge/Architecture-Local--First%20SPA-blue.svg)]()
[![Voice Engine](https://img.shields.io/badge/Voice%20Recognition-Web%20Speech%20API-purple.svg)]()
[![Visualizations](https://img.shields.io/badge/Visualizations-Chart.js-FF6384.svg?logo=chart.js)]()
[![Privacy](https://img.shields.io/badge/Data%20Privacy-100%25%20On--Device-brightgreen.svg)]()

> 🌐 **Live Application**: [https://dheerajeshwar32.github.io/healthOS/](https://dheerajeshwar32.github.io/healthOS/)

---

## 🌟 Overview

**healthOS** is a responsive, local-first personal health telemetry dashboard designed to track daily physical and mental wellness metrics in real time. Developed as an academic web programming project at **Vellore Institute of Technology (VIT)** by **N. Dheeraj Eshwar**.

Rather than routing private biological and wellness data to remote servers, healthOS processes, computes, and stores all health logs strictly inside the user's browser using `localStorage`. It integrates the browser-native **Web Speech API** for natural voice-assisted logging, **Chart.js** for interactive biometric visualizations, dynamic sleep-stress correlation algorithms, and medication adherence trackers in an accessible cyberpunk-inspired UI.

---

## ✨ Key Features

- 🎙️ **Hands-Free Voice Assistant**:
  - Leverages browser-native `webkitSpeechRecognition` / `SpeechRecognition` to dictate and parse wellness commands (e.g., *"add water"*, *"logged 500ml of water"*, *"slept 8 hours"*).
  - Automatically cleans and maps audio transcripts into numeric health metrics.
- 📊 **Dynamic Biometric Visualizations (Chart.js)**:
  - Real-time weekly water intake progression charts.
  - Multi-variable correlations mapping sleep duration against daily stress and fatigue levels.
  - Dynamic weekly step-tracking bar graph.
- 💊 **Medication & Adherence Tracker**:
  - Interactive schedule tracker with visual completion states and adherence rate calculation.
  - Persistent state management across browser sessions.
- 💧 **Hydration Target Engine**:
  - Dynamic progress gauges calculating remaining daily water intake goals based on user-calibrated baselines.
- 🧠 **Smart Advisor & BMI Calculator**:
  - Built-in BMI calculator and dynamic health score generator based on daily progress and biometric targets.
- 🌓 **Cyberpunk & Clean High-Contrast Theming**:
  - Deep OLED midnight theme (`#07090F`) with cyan (`#00D4AA`) and coral accents.
  - Clean light mode with rich slate typography for daytime legibility via CSS Custom Properties.
- 📤 **Export & Sharing Options**:
  - Direct WhatsApp sharing integration and PDF summary export support.
- 🔒 **Zero-Server Data Privacy**:
  - 100% client-side execution; zero cookies, zero tracking scripts, and zero cloud data leaks.

---

## 🏗️ Architecture & Stack

```
┌─────────────────────────────────────────────────────────────┐
│                      healthOS PIPELINE                      │
└─────────────────────────────────────────────────────────────┘

       User Voice Command / Form Input
                     │
                     ▼
         ┌────────────────────────┐
         │  Web Speech API / DOM  │  Speech recognition & form handlers
         └───────────┬────────────┘
                     │
                     ▼
         ┌────────────────────────┐
         │  State & Calculation   │  Hydration, sleep-stress index,
         │         Engine         │  BMI, adherence scores
         └───────────┬────────────┘
                     │
         ┌───────────┴────────────┐
         ▼                        ▼
┌──────────────────┐    ┌──────────────────┐
│   localStorage   │    │     Chart.js     │
│ Persistent Store │    │ Live Telemetry   │
└──────────────────┘    └──────────────────┘
```

| Layer | Technology | Purpose |
|:---|:---|:---|
| **Core UI** | HTML5 / Vanilla Modern CSS3 | Responsive grid, glassmorphic cards, custom range sliders |
| **Typography** | Orbitron & Nunito (Google Fonts) | High-tech numerical display & readable body text |
| **Charts** | Chart.js | Dynamic, reactive telemetry and correlation graphs |
| **Voice Engine** | HTML5 Web Speech API | Natural voice transcription and command parsing |
| **Persistence** | Browser `localStorage` | Pure on-device data security and zero latency |

---

## 🚀 Quick Start (Run Locally)

healthOS is a zero-dependency, single-bundle web application:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dheerajeshwar32/healthos.git
   cd healthos
   ```

2. **Launch directly in any browser:**
   - Double click `index.html` or open it with your browser:
     ```bash
     # Windows PowerShell
     Start-Process index.html
     ```
   - Alternatively, serve with a lightweight local server:
     ```bash
     npx serve .
     ```

---

## 👤 Author

* **Nagula Dheeraj Eshwar Prudhvi**
* Institution: **Vellore Institute of Technology (VIT)**
* GitHub: [@dheerajeshwar32](https://github.com/dheerajeshwar32)
* Live Application: [healthOS on GitHub Pages](https://dheerajeshwar32.github.io/healthOS/)
