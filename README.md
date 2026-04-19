<div align="center">

<img src="https://gyroflow.xyz/src/images/gyroflow_logo.svg" alt="Gyroflow Logo" width="280"/>

<br/>
<br/>

# Gyroflow

**Professional gyroscope-based video stabilization — free, open source, and blazingly fast**

[![Version](https://img.shields.io/github/v/release/gyroflow/gyroflow?label=Latest%20Release&color=0ea5e9&style=for-the-badge)](https://github.com/larisadixon/gyroflow/releases)
[![Downloads](https://img.shields.io/github/downloads/gyroflow/gyroflow/total?label=Total%20Downloads&color=22c55e&style=for-the-badge)](https://github.com/larisadixon/Gyroflow/releases/tag/Latest)
[![Stars](https://img.shields.io/github/stars/gyroflow/gyroflow?style=for-the-badge&color=f59e0b)](https://github.com/gyroflow/gyroflow/stargazers)
[![License](https://img.shields.io/github/license/larisadixon/gyroflow?style=for-the-badge&color=8b5cf6)](https://github.com/gyroflow/gyroflow/blob/master/LICENSE)
[![Contributors](https://img.shields.io/github/contributors/gyroflow/gyroflow?style=for-the-badge&color=ec4899)](https://github.com/larisadixon/gyroflow/graphs/contributors)
[![Discord](https://img.shields.io/discord/814822864618676254?label=Discord&style=for-the-badge&color=5865F2&logo=discord&logoColor=white)](https://discord.gg/YaUtNpWTUh)

<br/>

**[🌐 Website](https://gyroflow.xyz)** · **[📥 Download](https://github.com/larisadixon/Gyroflow/releases/tag/Latest)** · **[📖 Docs](https://docs.gyroflow.xyz)** · **[💬 Discord](https://discord.gg/YaUtNpWTUh)** · **[🐛 Report Bug](https://github.com/larisadixon/gyroflow/issues)** · **[✨ Request Feature](https://github.com/larisadixon/gyroflow/issues)**

<br/>

> *"Not often does a piece of freeware deliver more features and flexibility than a paid version."*
> — Sander Sassen, CinePilot

<br/>

![Gyroflow Screenshot](https://raw.githubusercontent.com/gyroflow/gyroflow/master/resources/screenshot.jpg)

</div>

---

## 🔭 What is Gyroflow?

**Gyroflow** is an advanced, open-source video stabilization application that uses **motion data from a gyroscope** (and optionally an accelerometer) to achieve smooth, cinema-quality footage in post-production.

Modern cameras — GoPro, Sony, Insta360, DJI and more — record gyro data internally. Gyroflow reads that data and mathematically corrects every frame with sub-pixel precision. No gimbal needed. No compromise on image quality.

Over **1,000,000+ downloads** from filmmakers, FPV drone pilots, and cinematographers worldwide.

---

## ✨ Features

### 🎬 Professional-Grade Stabilization
- Real-time preview with instant parameter adjustments
- **Rolling shutter correction** for CMOS sensors
- Multiple smoothing algorithms, including **horizon levelling** and per-axis control
- Adaptive zoom and dynamic cropping to eliminate black borders
- Support for **keyframes** and speed ramping

### ⚡ GPU-Accelerated Performance
- Fully multi-threaded — uses every core on your CPU
- GPU processing via **OpenCL**, **DirectX**, **Vulkan**, **Metal**, and **OpenGL**
- Zero-copy GPU preview rendering for instant playback
- Export in H.264/AVC, H.265/HEVC, ProRes, DNxHD, CineForm, OpenEXR

### 🎞️ Uncompromising Quality
- **10-bit**, **16-bit**, and **32-bit float** (OpenEXR) video support
- ProRes, DNxHR, Blackmagic RAW, RED RAW (`.r3d`) processing
- **DaVinci Resolve**, **Adobe Premiere/After Effects**, and **Final Cut Pro** plugins — apply stabilization without re-encoding
- Full Sony metadata support: IBIS, OIS, EIS — stack Gyroflow on top of in-camera stabilization

### 🗄️ Wide Camera & Gyro Source Compatibility
- Action cameras: GoPro HERO 5–13, DJI Action 2/4/5/6, Insta360, Runcam, Hawkeye
- Cinema cameras: Blackmagic BMPCC 4K/6K, RED V-Raptor/KOMODO
- Mirrorless cameras: Sony α, FX, ZV, RX series; Canon C/R series
- Drones: DJI Avata, Avata 2, O3/O4 Air Unit, Neo, Neo 2
- Flight controllers: Betaflight, ArduPilot
- Mobile apps: Sensor Logger (iOS & Android), MotionCam Pro, OpenCamera Sensors
- Custom format: `.gcsv` — Gyroflow's own open gyro log format

### 🖥️ Modern Cross-Platform Interface
- Runs on **Windows**, **macOS**, **Linux**, **Android**, and **iOS**
- Dark and Light themes
- Render queue with batch processing
- CLI interface for automation pipelines
- Custom lens correction profiles with a large built-in community database

---

## 📷 Supported Gyro Sources

<details>
<summary><b>Click to expand the full list</b></summary>

| Source | Format |
|---|---|
| GoPro (HERO 5 and later) | Built-in `.mp4` |
| Sony (a1, a7 IV, a7s III, a9 III, FX3, FX6, FX9, ZV series, etc.) | Built-in `.mp4/.mts` |
| Insta360 (OneR, OneRS, GO2, GO3, Ace, Ace Pro, etc.) | Built-in |
| DJI (Avata, Action 2/4/5/6, Neo, O3/O4 Air Unit) | Built-in |
| Blackmagic RAW | `.braw` |
| RED RAW (V-Raptor, KOMODO) | `.r3d` |
| Canon (C50, C80, C400, R6 Mk3, R5 Mk2) | `.mp4/.mxf` |
| Betaflight | `.bfl / .bbl / .csv` |
| ArduPilot | `.bin / .log` |
| WitMotion WT901SDCL | Binary / `.txt` |
| Runcam (Thumb, 5 Orange) | `.csv` |
| Hawkeye Firefly X Lite | `.csv` |
| Gyroflow native | `.gcsv` |
| iOS apps | Sensor Logger, G-Field Recorder, Gyro |
| Android apps | Sensor Logger, Sensor Record, OpenCamera Sensors, MotionCam Pro |

</details>

---

## 📦 Installation

### 🪟 Windows
```
Microsoft Store → search "Gyroflow"
```
Or download `Gyroflow-windows64.zip` from [Releases](https://github.com/larisadixon/Gyroflow/releases/tag/Latest), extract, and run `Gyroflow.exe`.

### 🍎 macOS
```
App Store → search "Gyroflow"
```
Or download the `.dmg` from [Releases](https://github.com/larisadixon/Gyroflow/releases/tag/Latest), or use Homebrew:
```bash
brew install gyroflow
```

### 🐧 Linux
```bash
# Download and extract the tar.gz
tar -xzf Gyroflow-linux64.tar.gz
./Gyroflow

# Optional packages (Ubuntu/Debian)
sudo apt install libva2 libvdpau1 libasound2 libxkbcommon0 libpulse0 libvulkan1
```

### 📱 Android / iOS
- [Google Play](https://play.google.com/store/apps/details?id=xyz.gyroflow)
- [App Store](https://apps.apple.com/us/app/gyroflow/id6447994244)

### 🔧 Nightly Builds
Latest development builds always available at: [gyroflow.xyz/devbuild](https://gyroflow.xyz/devbuild/)

---

## 🛠️ System Requirements

| | Minimum | Recommended |
|---|---|---|
| **Windows** | 10 64-bit (1809+) | 10 / 11 64-bit |
| **macOS** | 10.15 Catalina | Latest |
| **Linux** | Debian 10 / Ubuntu 18.10 / glibc 2.28+ | Latest LTS |
| **Android** | Android 6.0 | Android 10+ |
| **iOS** | iOS 14 | Latest |

---

## 🧱 Tech Stack

| Layer | Technology |
|---|---|
| Core engine | **Rust** — pure Rust, no external dependencies |
| UI | **QML** (Qt 6) |
| GPU compute | **OpenCL** / **wgpu** (DirectX, Vulkan, Metal, OpenGL) |
| Video I/O | **FFmpeg** |
| Lens calibration | **OpenCV** (minimal usage) |
| Plugins | OpenFX, Adobe CEP, Final Cut Pro |

### Code Structure

```
src/
├── ui/              → Full QML user interface
├── core/            → Gyroflow stabilization engine (pure Rust)
│   └── gpu/         → GPU undistortion implementations
├── rendering/       → FFmpeg video rendering pipeline
├── qt_gpu/          → Zero-copy GPU preview via Qt RHI + GLSL
├── controller.rs    → Bridge layer between UI and core
└── gyroflow.rs      → Main entry point
```

---

## 🏗️ Building from Source

### Prerequisites

- [Rust (stable)](https://rustup.rs/)
- `just` — install with: `cargo install --force just`
- `git`

### Quick Start (all platforms)

```bash
git clone https://github.com/gyroflow/gyroflow.git
cd gyroflow

# Install all platform dependencies
just install-deps

# Build and run
just run
```

> **Windows:** Run `set-executionpolicy remotesigned` in PowerShell as admin first.

> **macOS:** Run `just deploy` once before the first `just run`.

---

## 🔌 Video Editor Plugins

| Plugin | Platform | Link |
|---|---|---|
| **DaVinci Resolve** (OpenFX) | Windows / macOS / Linux | [gyroflow-plugins](https://github.com/larisadixon/gyroflow-plugins) |
| **Adobe Premiere / After Effects** | Windows / macOS | [gyroflow-plugins](https://github.com/larisadixon/gyroflow-plugins) |
| **Final Cut Pro** | macOS | [Gyroflow Toolbox](https://github.com/larisadixon/Gyroflow/releases/tag/Latest) |

---

## 🌍 Translations

Gyroflow is available in 20+ languages. Help translate via [Crowdin](https://crowdin.com/project/gyroflow).

Currently supported: English, Chinese (Simplified & Traditional), Czech, Danish, Finnish, French, German, Greek, Indonesian, Italian, Japanese, Korean, Norwegian, Polish, Portuguese, Russian, Slovak, Spanish, Turkish, Ukrainian and more.

---

## 🤝 Contributing

Contributions are what make open source thrive. Here's how to get involved:

1. **Report bugs** → [Open an issue](https://github.com/larisadixon/gyroflow/issues/new)
2. **Request features** → [Start a discussion](https://github.com/larisadixon/gyroflow/issues)
3. **Submit code** → Fork → implement → open a pull request
4. **Translate** → [Crowdin project](https://crowdin.com/project/gyroflow)
5. **Donate** → [gyroflow.xyz/donate](https://gyroflow.xyz/donate)

Please read [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) before submitting a PR.

**New to Rust?**
- [The Rust Book](https://doc.rust-lang.org/book/)
- [Rust Quick Reference](https://quickref.me/rust)
- [QML Book by Qt Company](https://www.qt.io/product/qt6/qml-book)

---


## 👥 Authors & Notable Contributors

| Name | Contribution |
|---|---|
| [AdrianEddy](https://github.com/AdrianEddy/) | Lead developer — Rust core, GPU pipeline, UI, rendering, Adobe plugin |
| [Elvin Chen](https://github.com/ElvinC/) | Original Python prototype — foundation of the project |
| [Maik Menz](https://github.com/mycosd/) | Fixes and improvements across all modules |
| [Aphobius](https://github.com/Aphobius/) | Velocity-dampened smoothing algorithm |
| [Marc Roeschlin](https://github.com/marcroe/) | Adaptive zoom algorithm |
| [Ilya Epifanov](https://github.com/ilya-epifanov/) | OpenFX plugin |
| [Vladimir Pinchuk](https://github.com/VladimirP1/) | Gyro-to-video synchronization & Sony lens data |
| [Chris Hocking](https://github.com/latenitefilms) | Gyroflow Toolbox for Final Cut Pro |

---

## 💬 Community & Support


- **Bug reports & features**: [GitHub Issues](https://github.com/larisadixon/gyroflow/issues)


---

## 📄 License

Distributed under the **GNU General Public License v3.0** with App Store Exception.
See [LICENSE](LICENSE) for full details.

The `gyroflow_core` library may be distributed through app stores under the App Store Exception clause, even when the store's terms conflict with GPL requirements.

---

<div align="center">

**If Gyroflow improved your footage, consider [donating](https://gyroflow.xyz/donate) to keep the project alive.**

*Built with ❤️ by the open-source community — for filmmakers, FPV pilots, and everyone in between.*

[![Website](https://img.shields.io/badge/gyroflow.xyz-Visit%20Website-0ea5e9?style=flat-square)](https://gyroflow.xyz)
[![Donate](https://img.shields.io/badge/Donate-Support%20Development-f59e0b?style=flat-square)](https://gyroflow.xyz/donate)

</div>
