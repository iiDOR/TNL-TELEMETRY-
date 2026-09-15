# TamilNadu Logistics VTC Tracker

**TNL Hub** — A modern desktop application for tracking and managing vehicle telemetry data for Euro Truck Simulator 2, with Discord Rich Presence integration and real-time monitoring.

![Version](https://img.shields.io/badge/version-0.1.0-blue)
![License](https://img.shields.io/badge/license-Proprietary-red)
![Status](https://img.shields.io/badge/status-Active%20Development-green)

## 🎯 About

TNL Hub is a comprehensive fleet management and telemetry tracking application designed for TamilNadu Logistics VTC (Virtual Trucking Company). It provides real-time monitoring of vehicle telemetry, automatic telemetry injection via DLL plugin, and seamless Discord integration for community engagement.

Built with **Tauri** (Rust + React), the app offers a lightweight, cross-platform desktop experience with native OS integration.

## ✨ Features

- **🚚 Real-time Telemetry Tracking** — Monitor vehicle speed, location, damage, cargo, and more
- **🎮 ETS2 Integration** — Auto-detect Euro Truck Simulator 2 installation and inject telemetry DLL
- **💬 Discord Rich Presence** — Display real-time VTC activity on Discord profile
- **⚙️ Customizable Settings** — Avatar decorations, animation speed, notification preferences
- **🔐 Secure Authentication** — Encrypted credential storage with 7-day token expiry
- **💾 Multi-Layer Caching** — SQLite + memory caching for optimal performance
- **🔄 Auto-Update System** — Automatic detection and installation of new versions
- **📊 Dashboard** — Sync and view convoy, job, and event data
- **🌓 Dark Theme** — Modern, sleek UI with customizable decorations

## 🚀 Getting Started

### Requirements

- **Windows 10/11** (64-bit)
- **Euro Truck Simulator 2** (ETS2 installed)
- **Node.js 18+** (for development)
- **Rust 1.70+** (for building from source)

### Installation

#### Download Installer (Recommended)

1. Go to [Releases](https://github.com/CrypterENC/TNL-TELEMETRY-/releases)
2. Download the latest `TamilNadu.Logistics_x.x.x_x64-setup.exe`
3. Run the installer and follow the prompts
4. Launch the app from Start Menu

## 📖 Usage

### First Launch

1. **Setup ETS2 Path** — App will auto-detect your ETS2 installation
2. **Install Telemetry DLL** — Click "Install DLL" to inject telemetry plugin
3. **Login** — Sign in with your TNL account
4. **Configure Settings** — Customize avatar decoration and notifications

### Running the App

1. Open **TamilNadu Logistics** from your applications
2. The **splash screen** will check for updates automatically
3. **Login** with your credentials (encrypted and stored locally)
4. **Monitor** your VTC activity, convoy data, and telemetry

### Managing Settings

Navigate to **Settings** (⚙️) to configure:
- **Avatar Decoration** — Choose style (Electric, Glowing, Glitch, Nitro, Aura)
- **Decoration Settings** — Customize colors, intensity, glow, animation speed
- **Notifications** — Toggle event reminders, leaderboard updates, damage alerts
- **Animation Speed** — Slow (0.5x) to Fast (5x)

## 🔧 Development

### Tech Stack

**Frontend:**
- React 18 with TypeScript
- Vite (build tool)
- Zustand (state management)
- Tailwind CSS + Radix UI
- Framer Motion, GSAP, Lottie (animations)

**Backend:**
- Tauri 2 (desktop framework)
- Rust 1.70+
- SQLx (database)
- Reqwest (HTTP client)
- Tokio (async runtime)

## 📝 Changelogs

### v0.0.2 (Latest) — 2026-05-16

**Features:**
- ✨ Add TNL logo to titlebar with dark black background
- ⚙️ Fix settings persistence (density field now saves correctly)
- 🎨 Improved titlebar styling with pure black background

**Fixes:**
- 🐛 Settings no longer lose density field on save
- 🐛 Backend AppSettings struct now includes density field for proper serialization

**Known Issues:**
- GitHub releases must be created from committed version changes for updater to work properly

### v0.0.1 — 2026-05-16

**Initial Release:**
- 🚀 Core telemetry tracking and monitoring
- 🎮 ETS2 DLL injection and plugin management
- 💬 Discord Rich Presence integration
- ⚙️ Settings panel with avatar decorations
- 🔐 Encrypted credential storage
- 💾 Multi-layer caching system (SQLite + memory)
- 🔄 Auto-update system via GitHub releases
- 📊 Dashboard with event and convoy data
- 🌓 Dark theme with modern UI

**Features:**
- Real-time telemetry data synchronization
- Configurable API endpoints and VTC ID via environment variables
- Multi-language support for notifications
- Drag-and-drop task management
- Animated avatar decorations (5 styles)
- Performance optimizations with lazy loading

## 🔐 Security

- **Credentials** are encrypted with AES-GCM and stored in Windows AppData
- **API tokens** expire automatically after 7 days
- **No passwords** are transmitted unencrypted
- **DLL injection** is sandboxed within ETS2 plugin directory

## 🐛 Bug Reports

Found a bug? Please report it on [GitHub Issues](https://github.com/CrypterENC/TNL-TELEMETRY-/issues)

Include:
- App version (check in titlebar)
- Steps to reproduce
- Screenshots/error logs

## 📄 License

This project is proprietary software. All rights reserved © 2026 TamilNadu Logistics VTC.

## 👤 Author

Created by **@CrypterENC** for TamilNadu Logistics VTC

## 🙏 Acknowledgments

- Tauri framework for providing an excellent desktop app solution
- ETS2 community for telemetry standards
- Discord API for Rich Presence integration

---

**Latest Release:** [v0.0.2](https://github.com/CrypterENC/TNL-TELEMETRY-/releases/tag/Testingv0.0.2)  
**Repository:** [CrypterENC/TNL-TELEMETRY-](https://github.com/CrypterENC/TNL-TELEMETRY-)
