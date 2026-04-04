# ⬛ ETALONIA

![Version](https://img.shields.io/badge/version-v0.0.12_pre--beta-black)
![License](https://img.shields.io/badge/license-Proprietary-black)
![Platform](https://img.shields.io/badge/platform-Windows_10_|_11_(64--bit)-black)

> **Enhanced Tools Animation Layers Overlay Navigation Interface App**

🌐 **Languages:** [English](README.md) | [Русский](README(RU).md)

**ETALONIA** is an isolated real-time scene composition environment for streaming and live production.  
It is not a replacement for OBS. It is a control layer that sits on top of it.

Design your broadcast's visual logic separately from encoding and transmission.  
No interface interference. No risk of ruining the final picture.

Recommended integration: **OBS Studio**.

---

# 🎯 Positioning

ETALONIA is:

- 🎥 **Broadcast Composition Engine** - 🧠 **Control Layer** for live production  
- 🛠 **Isolated Workspace** for the streamer  

**OBS handles:**
- encoding
- streaming
- recording

**ETALONIA handles:**
- scene structure
- layer management
- safe real-time editing
- architectural isolation of the visual signal

---

# ❓ Why not just OBS?

OBS is a tool for encoding and broadcasting.

**ETALONIA:**
- structures scene architecture
- isolates the workspace
- allows safe editing during live broadcasts
- reduces the risk of visual artifacts

It is not a competitor to OBS.  
It is an advanced add-on.

---

# 🖥 Dual-Window Architecture

### 🛠 Editor
The workspace for building scenes.

### 🎥 Output
A clean window for capture in OBS.

**Editor and Output are rendered independently.**

Editing does not affect the final signal. The interface never appears on stream. Changes are applied on-the-fly.

---

# 🔄 Typical Workflow

1. Create scenes: `Start`, `Gameplay`, `Break`, `Chat`.
2. Configure layers, cards, and sources.
3. Capture the **Output** window in OBS.
4. Switch scenes via hotkeys.
5. Make changes in the **Editor** without risking the broadcast.

---

# 🎬 Features

## Scene Management
- creation and switching
- hotkeys
- transitions
- scene locking (protection against accidental edits before airtime)
- templates for various broadcast formats

## Layer System
- text
- images
- video
- audio
- web sources
- cards
- grouping
- rendering order
- visibility management

## Scene Background
- color
- image
- video
- effects

## Preset Ecosystem
- `.escf` — scene  
- `.escdf` — card  
- `.escprf` — full project  

Quickly save and load complex configurations.

---

# ⚡ Architectural Highlights

- **Dual-Window Rendering Isolation**
- **Real-Time State Synchronization**
- **On-the-Fly Editing Engine**
- **Asset Decoupling Layer**
- **Lightweight Update Mode**
- **Preset-Based Scene Architecture**

Scene design is decoupled from final signal rendering.

---

# 🧩 Stream Mode (Lightweight Editor)

A mode for long and resource-intensive broadcasts.

### Behavior:
- heavy previews are replaced by Type + ID
- scene logic remains intact
- Output remains full-quality

### Use when:
- dealing with a high number of web sources
- 2+ hour streams
- limited hardware resources
- running a game and browser simultaneously

Menu: `Scene → Stream Mode (Lightweight Editor)`

---

# 🖥 System Requirements

| Parameter | Minimum | Recommended |
|-----|-------------------|-----------------|
| CPU | 4 threads | 8+ threads |
| RAM | 8 GB | 16 GB |
| GPU | DX11 / OpenGL 3.3 | Discrete GPU |

**OS:** Windows 10 / 11 (64-bit)  
**Third-party dependencies:** none required  

### Performance

- 4 threads — ~30 FPS live-update  
- ≤3 threads — Web Worker is disabled

---

# 🔐 Local Diagnostics

The software maintains an automatic event log for stability analysis and rapid bug fixing.

### 📋 What is recorded
* **System Snapshot:** hardware technical specifications (CPU/RAM/GPU) at session start.
* **Lifecycle:** application launch, restart, and shutdown events.
* **Error Tracking:** detailed capture of critical system errors and warnings.
* **Interface Events:** key user actions in the Editor (no personal data collection).
* **Performance:** reports on system load, memory consumption, and rendering speed.

### 📁 Storage and Path
All diagnostic data is stored **exclusively locally** on the user's device:  
`Documents/ETALONIA/logs`

### 🛡 Privacy Policy
* **Zero-Cloud:** data is never sent to external servers or third parties.
* **Auto-Purge:** log files are automatically deleted after **7 days** or upon reaching **140 hours** of total application runtime.
* **No Telemetry:** hidden transmission of marketing, statistical, or personal data is non-existent.

> [!IMPORTANT]
> Logs are intended only for personal analysis by the user or voluntary submission to the developer for resolving technical issues.

# ⚠ Alpha Notice

This version is currently in the **ALPHA** stage.  
Architecture and performance are subject to change. Testing is recommended before critical broadcasts.

---

# 🛡 License

ETALONIA is closed proprietary software.

**Prohibited:**
1. Code distribution
2. Decompilation
3. Reverse engineering
4. Bypassing protection mechanisms

Usage is governed by the EULA.  
Details — in [EULA 1.1](https://github.com/VDarkXV/etalonia-project/blob/main/EULA.md).

---

## ⚖️ License Summary

ETALONIA is proprietary software.  
Usage is governed by the full license (EULA 1.1).

**Overview (Informational, not legally binding):**
- Prohibited to distribute, copy, or modify code.
- Prohibited to reverse engineer or decompile.
- Prohibited to bypass security mechanisms.
- All intellectual property, branding, and scene logic belong to Danylo Panysko (V_DarkX_V).
- Logs are created locally for diagnostics and are not sent over the network.

> ⚠️ This summary is for informational purposes only. Only the full version of EULA 1.1 has legal force.

---

### 🧪 Closed Beta Testing
ETALONIA is currently in closed testing.
- **How to join:** Apply via our [Discord Server](https://discord.gg/QhTCffCas6).
- **Terms:** All testers must comply with the [NDA / Closed Testing Agreement](https://github.com/VDarkXV/etalonia-project/blob/main/NDA(Close%20Testing%20Agreement).md).
- **Important:** Public demonstration is allowed for the **Output** window only.

---

© 2026 Danylo Panysko (V_DarkX_V) — ETALONIA Project  
Contact: etalonia.dev@gmail.com
