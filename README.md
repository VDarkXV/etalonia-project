# ETALONIA

![Version](https://img.shields.io/badge/version-v0.0.13_PRE--BETA-black)
![Platform](https://img.shields.io/badge/platform-Windows_10_|_11_(64--bit)-black)
![License](https://img.shields.io/badge/license-Proprietary-black)

> **Enhanced Tools Animation Layers Overlay Navigation Interface Application**

 **Languages:** [English](README.md) | [Русский](README(RU).md)

**ETALONIA** is a local real-time visual control layer for live broadcasts and live production.  
It is designed to work **alongside OBS Studio**, not replace it.

OBS handles encoding, recording, and streaming.  
ETALONIA handles scene structure, cards, web sources, transitions, hotkeys, and safe live updates during broadcasts.

---

## What ETALONIA is for

ETALONIA is built for broadcasts that need more than a basic scene list.  
It helps manage visual logic, show states, cards, web sources, and scene structure from one place — without risking the editor appearing on stream.

Especially useful for:

- talk shows;
- VTuber and character-driven streams;
- tournaments and game shows;
- quiz formats;
- panel discussions;
- overlay-heavy productions;
- long broadcasts with many sources;
- setups where OBS scenes become difficult to manage comfortably.

---

## Why not just OBS?

OBS is excellent for encoding, recording, and streaming.  
ETALONIA handles the **production logic around the broadcast**.

With ETALONIA you can:

- build scenes outside OBS;
- keep a clean Output window for capture;
- edit live without exposing the interface on stream;
- reduce OBS scene overload by moving orchestration into a separate layer;
- manage cards, sources, overlays, and scene states from one workspace.

In short, ETALONIA acts as a control layer between your content and OBS.

---

## Typical workflow

1. Launch ETALONIA.
2. Build scenes, cards, layers, and sources in the **Editor**.
3. Capture the clean **Output** window in OBS.
4. Switch scenes using hotkeys.
5. Make live changes while the stream output stays clean.

**Editor** is for preparation and control.  
**Output** is for the broadcast itself.

---

## Dual-window architecture

### Editor

Workspace for building and managing scenes.

### Output

A clean render window intended for OBS capture.

The windows are separated intentionally:

- the Editor never needs to appear on stream;
- the Output remains visually clean;
- changes can be applied on the fly;
- live editing does not disrupt the final output.

---

## Main features

### Scene management

- create and switch scenes;
- configure transitions;
- lock scenes to prevent accidental edits before going live;
- use templates for different broadcast formats;
- save and load scene files.

### Layers and objects

Supported objects:

- text;
- images;
- video;
- audio;
- web / iframe sources;
- cards;
- grouped objects.

Objects support:

- layer ordering;
- selection;
- snapping;
- transforms;
- visibility states;
- optional enter / exit animation behavior.
- object's effects

### Scene backgrounds and effects

Scenes can use:

- solid colors;
- images;
- video backgrounds;
- blur and effect modes.

### Hotkeys

ETALONIA supports configurable hotkeys for fast Editor workflows and Output control.  
Hotkey profiles can be imported and exported.

---

## Cards: the core show-control system

Cards are one of the main production systems inside ETALONIA.  
They are especially useful for:

- players;
- guests;
- challenge states;
- topic cards;
- voting blocks;
- role cards;
- live show data;
- interactive formats of any kind.

Card features include:

- draggable and resizable webcam blocks;
- multiple rich-text lines;
- line visibility modes;
- swap / placeholder mode;
- per-line positioning and sizing;
- card background color, image, or video;
- save and load support;
- preview generation.

### Card Manager

Card Manager is built for fast live manipulation of many cards at once.

Features include:

- adaptive card grid;
- active-card or whole-scene mode;
- smart shuffle across cards;
- smart shuffle inside a single card;
- mass find and replace;
- regex and mask helpers;
- webcam URL replacement;
- undo for mass actions;
- quick hide / swap controls;
- drag-and-drop swapping between cards;
- card-set save and load.

### Card sets and arrays

ETALONIA also includes a lightweight show-data layer:

- **Card Set** — save/load groups of cards as `.esccs`;
- **Card Value Arrays** — reusable value collections for mass replacement;
- import/export support for text, `.escva`, and JSON-compatible collections;
- array tokens can be inserted using the `массив "Name"` form;
- optional no-repeat replacement for filling many cards without duplicate values.

The idea is simple: keep layouts as card sets, keep episode data as arrays, then apply everything before going live.

---

## Web sources

ETALONIA supports generic iframe sources and VDO / OBS Ninja style sources.

For VDO / OBS Ninja URLs, the application attempts to normalize useful viewing parameters where possible, such as clean output, cover, and transparency.

Available controls include:

- aspect ratio management;
- source resolution presets;
- custom source backgrounds;
- mute state;
- health / reconnect status;
- manual reload;
- optional scheduled Output maintenance.

This is especially useful for productions with many browser sources, remote guests, and live web content.

---

## Stream Mode

Stream Mode is a lightweight Editor mode for long or resource-heavy broadcasts.  
It keeps the Output window at full quality while reducing Editor load where possible.

Useful when:

- using many iframe or browser sources;
- running long broadcasts;
- working with limited CPU or RAM headroom;
- running a game, browser, OBS, and ETALONIA simultaneously;
- stability matters more than full preview detail.

---

## File formats

ETALONIA uses local files for scenes, cards, projects, and data collections.

- `.escf` — scene file
- `.escdf` — card file
- `.escprf` — project / preset file
- `.esccs` — card set
- `.escva`, `.txt`, `.json` — card value array collections

User files are stored locally.  
ETALONIA does not require a cloud account in the current PRE-BETA workflow.

---

## Local diagnostics

ETALONIA stores local diagnostic data to help with stability and troubleshooting.

Recorded data may include:

- application launch, restart, and shutdown events;
- renderer console events;
- IPC heartbeat and synchronization summaries;
- scene synchronization summaries;
- Output performance data;
- memory snapshots and guard events;
- hardware snapshots;
- key interface events related to Editor behavior.

### Storage

All logs are stored locally on the user’s device:

```
Documents/ETALONIA/logs
```
### Privacy
- no cloud uploads;
- no external telemetry;
- no hidden marketing or personal-data transmission;
- logs may be automatically deleted after 7 days or after 140 hours of total application runtime.

Logs are intended for personal diagnostics or voluntary submission to the developer during troubleshooting.

---

# System Requirements

| Parameter | Minimum | Recommended |
|-----|-------------------|-----------------|
| CPU | 4 threads | 8+ threads |
| RAM | 8 GB | 16 GB |
| GPU | DX11 / OpenGL 3.3 | Discrete GPU |

**OS:** Windows 10 / 11 (64-bit)  
**Third-party dependencies:** none required  


Large productions with many webcams or browser sources depend heavily on browser behavior, WebRTC stability, network conditions, and GPU memory availability.
Before important broadcasts, always test scenes on the same hardware and setup you plan to stream with.


### PRE-BETA notice

ETALONIA 0.0.13 is a PRE-BETA build.
The architecture is already usable, but some details may still change before Beta.

Do not rely on PRE-BETA builds for critical paid productions without rehearsal on the same hardware and scene setup.

---

# License

ETALONIA is proprietary software.

Usage is governed by the full license agreement.
See  [EULA 1.1](https://github.com/VDarkXV/etalonia-project/blob/main/EULA.md).


### License summary

This summary is informational only and does not replace the full [EULA](https://github.com/VDarkXV/etalonia-project/blob/main/EULA.md).

Prohibited:

- distributing the software or source code;
- modifying the code or creating unauthorized repacks;
- decompiling or reverse engineering;
- bypassing protection or security mechanisms.

All intellectual property, branding, assets, and scene-system logic belong to [Danylo Panysko (V_DarkX_V)](mailto:etalonia.dev@gmail.com).

Local diagnostic logs are created only for stability analysis and are not transmitted over the network.

Only the full version of [EULA 1.1](https://github.com/VDarkXV/etalonia-project/blob/main/EULA.md) has legal force.

---

# Closed beta testing

ETALONIA is currently in closed testing.


### How to join

Apply via the official [Discord Server](https://discord.gg/QhTCffCas6).

### Testing terms

All testers must comply with the [NDA / Closed Testing Agreement](https://github.com/VDarkXV/etalonia-project/blob/main/NDA%28Close%20Testing%20Agreement%29.md).

### Important

Public demonstration is allowed for the Output window only.

---

# © 2026 Danylo Panysko (V_DarkX_V) — ETALONIA Project 
# Contact: [etalonia.dev@gmail.com](mailto:etalonia.dev@gmail.com)

---
