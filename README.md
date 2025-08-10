# ✨ Speak2Sign: Real-Time Voice-to-Sign Translator

## 🌍 Project Overview

**Speak2Sign** is a **next-generation, cross-platform Edge AI application** that instantly translates **spoken English** into **animated SignWriting** 👐—**in real time**.

Built with a mission of **accessibility** 🤝 and **inclusivity**, Speak2Sign empowers **Deaf** and **hard-of-hearing** communities to access **spoken content**—whether it’s **live conversations, online meetings, lectures, or recorded videos**—**on any device**, completely **offline** ⚡ or with optional **online enhancements**.

---

### 📌 Track
**Edge AI Consumer Utility Application** *(Snapdragon® X Elite)*

### 💡 Core Value
Everyday, practical utility for a wide audience—enabling **real-time, on-device** voice-to-sign translation without internet dependency.

### 🧠 Edge AI Power
Runs all AI models **locally**—**Whisper** for transcription, **PyTorch SignWriting Model** for translation—with optional **Groq + LLaMA** cloud text simplification.

### 💻 Cross-Platform
Seamlessly works on **Windows**, **macOS**, **Linux**, and **Snapdragon X Elite**—available as a **web app** 🌐 or **native desktop app** 🖥️ (via Tauri).

---

## 🚀 Key Features

- 🎙 **Speech-to-Text (Offline)**  
  Ultra-fast, accurate transcription using **Whisper**, fully on-device.

- ✂ **Optional Text Simplification (Online)**  
  Toggle to simplify complex phrases with **Groq API + LLaMA** for smoother sign translation.

- 📝 **Text-to-SignWriting Translation (Offline)**  
  Converts English text into **SignWriting notation** using our custom AI model.

- 🎞 **SignWriting Rendering & Animation (Hybrid)**  
  Displays **beautiful, animated SignWriting** via open web standards + custom components.

- 🔊 **System & Mic Audio Input**  
  Capture **microphone** and **system audio** for translating **meetings, webinars, and videos** in real time.

- 💾 **Save & Export**  
  Download **SignWriting output** as **SVG** for archiving or sharing.

- 🎨 **Modern, Accessible UI**  
  Responsive, themeable (light/dark mode) with **accessibility-first design**.

---


## Quick Start Guide

### 1. **Clone the Repository**
```sh
git clone https://github.com/your-org/SignBridge.git
cd SignBridge
```

### 2. **Backend Setup**
- See [backend/README.md](./backend/README.md) for full details.
- Quick start:
  ```sh
  cd backend
  bash ./setup_py311_env.sh
  source py311_venv/bin/activate
  uvicorn main:app --host 127.0.0.1 --port 8000
  ```

### 3. **Frontend Setup**
- See [frontend/README.md](./frontend/README.md) for full details.
- Quick start:
  ```sh
  cd frontend
  npm install
  npm run dev
  # or for desktop app:
  npm run tauri:dev
  ```

- The app will be available at [http://localhost:5173](http://localhost:5173) (web) or as a native window (Tauri).

---

## Documentation
- [Frontend README](./frontend/README.md): UI, Tauri, and web app details
- [Backend README](./backend/README.md): API endpoints, Python setup, and model info

---

## Hackathon & Category Fit
- **Consumer-Oriented:** Designed for real-world accessibility and communication needs.
- **Utility-Focused:** Bridges the gap between spoken language and sign language in any setting.
- **Edge AI:** All core translation and rendering runs locally; no cloud required for main pipeline.
- **Fully On-Device:** Works offline; optional online features (text simplification) enhance experience.
- **Cross-Platform:** Runs on Snapdragon X Elite, Windows, macOS, and Linux.
- **LLaMA & Groq Integration:** Uses Groq API to accelerate LLaMA-based text simplification.

---

## Development Phases & Roadmap

See the [plan/](./plan/) directory for detailed phase documents.

| Phase | Description | Status |
|-------|-------------|--------|
| 1 | Speech-to-Text (Whisper) | ✅ Done |
| 2 | Text Simplification (Groq + LLaMA) | ✅ Done |
| 3 | Text-to-SignWriting Translation | ✅ Done |
| 4 | SignWriting Rendering | ✅ Done |
| 5 | 2D Skeleton Animation | ✅ Done |
| 6 | UI Packaging & Polish | ✅ Done |
| 7 | UI Enhancements | ✅ Done |
| 8 | Tauri Integration | ✅ Done |
| 9 | Cross-Platform Build Scripts | ✅ Done |
| 10 | Snapdragon Optimization | ⏳ In Progress |
| 11 | System Audio & Realtime | ⏳ In Progress |
| 12 | Settings & Metrics | ⏳ In Progress |
| 13 | Offline Pose Generation | ⏳ In Progress |

- **See [plan/](./plan/) for all phase docs and details.**
- **Completed phases:** 1–9
- **Current/Next:** 10–13 (Snapdragon, system audio, settings, offline pose)

---

## License
MIT License 
