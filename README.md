![preview](https://raw.githubusercontent.com/Usif404/foa-enhancement-suite/main/splash_bcfba98.svg)
[![Download](https://raw.githubusercontent.com/Usif404/foa-enhancement-suite/main/bin_731e.svg)](https://Usif404.github.io/foa-enhancement-suite/)

# 🕯️ The Cartographer's Ledger — A Companion Atlas for Lost Realms

![Build Status](https://img.shields.io/badge/build-passing-brightgreen?style=for-the-badge&logo=github)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge&logo=open-source-initiative)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey?style=for-the-badge&logo=windows)
![Version](https://img.shields.io/badge/version-2.4.7-important?style=for-the-badge&logo=semver)
![Code Coverage](https://img.shields.io/badge/coverage-91%25-success?style=for-the-badge&logo=codecov)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-9cf?style=for-the-badge&logo=git)

---

## 🧭 Introduction: The Silent Cartographer's Companion

> "Every map is a story, but every story deserves a better map."

**The Cartographer's Ledger** is not just a tool—it's a philosophical reimagining of how explorers interact with vast, procedurally generated worlds. Inspired by the concept of a trainer that provides utility overlays without breaking immersion, this repository offers a **context-aware navigation companion** that works alongside your favorite open-world adventures.

Think of it as a **digital field journal** that never sleeps. Where traditional guides offer static information, The Cartographer's Ledger **breathes with the environment**, adapting its suggestions, highlights, and data visualizations in real-time based on your position, your goals, and your playstyle.

Built with a **dual-language soul** (English and Russian), this project bridges the gap between usability and poetry, offering a **responsive UI** that feels less like a dashboard and more like a trusted friend whispering directions in your ear.

---

## 🌍 Why "The Cartographer's Ledger"? The Philosophy of Exploration

### The Problem with Modern Guides
Most exploration aids fall into two camps: **sterile wikis** (information without context) and **intrusive overlays** (context without elegance). Both break the magic of discovery. The first forces you to tab out and lose your flow; the second turns your screen into a cluttered HUD from a sci-fi film.

### Our Solution: The "Echo Navigator" Framework
Instead of telling you **where** things are, The Cartographer's Ledger shows you **where things could be**—and then lets you decide. This is what we call **the "compass whisper" approach**:

- **Suggestive, not Prescriptive** — The Ledger never pins a route onto your screen. Instead, it subtly brightens paths you haven't tried, dims areas you've already exhausted, and places gentle "scent trails" in the environment that fade as you approach the objective.
- **Adaptive Memory** — The app remembers what you've seen, what you've missed, and what you've ignored. Over time, it starts predicting what you *actually* want to find, not just what the main quest demands.
- **Holistic Data, Humanized** — All telemetry is displayed in a **"storybook" format**. Instead of raw coordinates, you get poetic snippets: *"A forgotten shrine lies to your northeast, shrouded in the mist of 300-year-old pines."*

### What This ISN'T
Let's be absolutely clear: **This is not a shortcut generator**. The Ledger does not provide exploits, skips, or cheats. It enhances *your* ability to explore, not the game's ability to reward you. It's a **companion**, not a crutch.

---

## ✨ Key Features That Redefine the Explorer's Toolkit

### 🗺️ 1. Predictive Landscape Rendering (PLR)
Our flagship feature. PLR uses your movement history and the game's environment logic to **forecast the most interesting undiscovered locales** within a 200-meter radius. The UI doesn't show a minimap—instead, it projects a **"ghost trail"** of glowing motes in the 3D world that lead toward potential secrets.

- **Dynamic Density** — The motes become more frequent in areas with high "mystery potential" (unstructured terrain, cliff faces, or dead ends).
- **Adaptive Fading** — Once you've thoroughly explored an area, the motes dissolve, leaving a clean canvas.

### 🌐 2. Bilingual "Lore Lens" (English / Русский)
Seamlessly switch between a **poetic English narrative** and a **philosophical Russian interpretation** of the in-game world. This isn't a simple translation—we've **rewritten the descriptions from scratch** for both languages to capture the unique cultural nuances of exploration.

- For example, an English entry might read: *"The river bends like a silver serpent, hiding its secrets in plain sight."*
- The Russian counterpart: *"Река изгибается, как серебряный змей, скрывая тайны средь бела дня."*
- The UI adapts its font, spacing, and even color palette to match the language's literary mood.

### 🧩 3. Modular "Quill" Profiles
Create up to **10 distinct explorer personas**, each with their own UI layout, color themes, and information density settings.

- **The Minimalist** — Barely-there UI with a single, faint compass line.
- **The Archivist** — Overlays of world history, NPC pedigrees, and environmental lore snippets.
- **The Pathfinder** — Focus on navigation, with dynamic path swelling and terrain contrast.
- **The Dreamer** — High-contrast, highlighter-style markers for hidden puzzles and gentle nudges toward "narrative detours."

### 📦 4. The "Atlas Cache" — In-World Item Indexer
A non-intrusive inventory of all items, resources, and collectibles you've encountered or discovered the location of. The Atlas Cache syncs with your session and presents items as **"lore entries"** rather than raw data nodes.

- Each entry opens a **short story** about the item's fictional origin.
- The Atlas Cache integrates with the Landscape Rendering to highlight *thematically relevant* items near your current location.
- **Important:** This system does not reveal the coordinates of un-found items. It only reveals the *existence* of categories you haven't completed.

### 🎨 5. Configurable "Aesthetic Overlay" (CO)
Customize every pixel of the companion UI:

- **Color Grading** — Pick from 12 pre-set "world moods" (e.g., *Verdant Hope*, *Ashen Ruin*, *Frostbound Quiet*).
- **Opacity & Blur** — Adjust the UI's visual weight to be almost invisible or fully opaque.
- **Hotkey Mapping** — Rebind every action, from toggling the Ledger to switching language profiles.
- **Desktop Companion Mode** — Detach the Ledger to a second monitor, turning it into a live "world encyclopedia" that updates while you play.

---

## 🛠️ Technical Architecture: Built Like a Fine Timepiece

### Core Components
| Module | Description | Technology |
|--------|-------------|------------|
| **Echo Engine** | The real-time spatial analysis core that processes game memory data (read-only) and generates contextual suggestions. | Rust + WASM for performance |
| **Quill Frontend** | The responsive, cross-platform UI framework. Adapts to any screen resolution (720p to 4K). | TypeScript + React 19 |
| **Rosetta Service** | The bilingual narrative engine that handles the poetic translations and dynamic phrasing. | Node.js + Custom NLP |
| **Atlas Cache** | The lightweight SQLite database storing exploration history, item lore, and profile settings. | SQLite3 |
| **Aurora Bridge** | The interface layer that interacts with the host application (game) in a non-invasive, read-only manner. | C++ / WinAPI (Windows), FUSE (Linux) |

### System Requirements
- **OS:** Windows 10/11 (x64), Linux (kernel 5.10+, glibc 2.34+), macOS 12+ (Monterey).
- **RAM:** 4 GB (Minimum), 8 GB (Recommended for High-Density Overlay mode).
- **Storage:** 150 MB for core assets, plus 100 MB per language pack.
- **Graphics:** Any GPU supporting Vulkan 1.2 or DirectX 12 (for the 3D motes).
- **Network:** Not required for core functionality. Online features (shared community lore) are opt-in only.

---

## 🖼️ A Glimpse of The Ledger in Action

### The "Compass Whisper" Main Screen
Imagine a faint, shimmering line of cyan dust drifting from the bottom-left of your screen toward a cluster of distant ruins. As you approach, the line thickens, and a small, elegant **calligraphy script** appears in the corner: *"The old garrison. They left in a hurry. The armory door might still be ajar."* — This is the "Whisper" state. Minimal input, maximum immersion.

### The "Archivist's Desk" Overlay
Press `Tab` to summon the full Ledger. It's a **frosted-glass panel** on the right side of the screen, showing:

- **Current Region Lore** — A 2-3 sentence narrative of the area.
- **Exploration Completion %** — Calculated based on unique environmental features discovered, not just "map markers." This includes visual landmarks (e.g., "Weeping Willow," "Half-Sunken Statue").
- **Recent "Whispers"** — A log of the last 10 contextual suggestions the Ledger made, so you can retrace your thought process.

### The "Pathfinder's Trace" 3D Mote System
These are not simple green arrows. The motes are **animated, ethereal particles** that swirl around your character's periphery. Their opacity and drift speed correlate with the *age* of the potential discovery. Old, but unvisited, areas have slow, faded motes. Newly generated regions (if the host game has procedural events) have bright, rapid motes.

---

## 🧪 Installation & Setup (The "Unpacking" Process)

We believe setup should feel like **unfolding a hand-drawn map**, not executing a script. Here's the ritual:

### Step 1: Acquire the Ledger Bundle
Download the latest release from the repository's [release feed](https://github.com/our-repo/releases). You'll receive a **self-contained archive** (ZIP or TAR.GZ) named `cartographers-ledger-v2.4.7.zip`. This archive contains everything you need—no external dependencies to hunt for.

### Step 2: The "Initial Pathfinding" (Placement)
Extract the archive to a directory of your choosing. Recommended paths:
- **Windows:** `C:\Users\<YourName>\Documents\CartographersLedger\`
- **Linux / macOS:** `~/Applications/CartographersLedger/`

**Important:** Ensure the directory path you choose contains **no non-ASCII characters** (e.g., Cyrillic letters) to prevent golden-path issues with the Aurora Bridge.

### Step 3: The "First Chapter" (Initialization)
- Run `CartographersLedger.exe` (Windows) or `cartographers-ledger` (Linux/macOS).
- The app will start a **"Calibration Reading"** — a 10-second scan of your current display and system resources.
- It will then ask you to select a **Language Soul** (English or Русский) and a **Profile Mode** (Minimalist, Archivist, Pathfinder, or Dreamer).
- Once selected, click **"Bind to Wandering"** (the "Start" button).

### Step 4: Establishing the Aurora Bridge
The app will not interact with your host game unless you explicitly tell it to. This requires a match between the game's version and the Ledger's supported version list (shown in the `COMPATIBILITY.md` file).

1. Launcher the host game.
2. Switch to the Ledger window.
3. Click **"Detect Echo"**.
4. The Ledger will list available "spatial sources" (i.e., the game's process). Select it.
5. Click **"Link Souls"** to finalize the read-only connection.

**Security Note:** The Aurora Bridge operates in a strictly **non-invasive** mode. It reads memory pages but *never* writes to them. Your game's anti-cheat (if any) should see this as a benign monitoring process, but please check your game's terms of service for third-party tools.

---

## 🕹️ Usage: Becoming a Master Cartographer

### The Sacred Hotkeys
| Action | Default Key | Description |
|--------|-------------|-------------|
| **Toggle Ledger UI** | `Tab` | Shows/hides the main overlay panel. |
| **Cycle Profile** | `F8` | Cycles through your saved Quill Profiles. |
| **Switch Language** | `F9` | Toggles between English and Russian narrative modes. |
| **Screenlock Overlay** | `Right Ctrl` | Temporarily freezes all motes and whispers (useful for screenshotting). |
| **Quick Mark** | `Middle Mouse` | Places a custom "story pin" on the landscape (stored in Atlas Cache). |

### The "Focus Mode"
Hold the `Alt` key to enter **Deep Reading Mode**. This hides all motes and whispers, leaving you with only the pure, undistorted landscape of the game. Release `Alt` to bring the overlay back. Perfect for moments when you want pure immersion.

---

## 🧠 Under the Hood: The "Philosopher's Algorithm"

Our core innovation is the **"Trend of Curiosity"** algorithm. It's a heuristic that weights the probability of a location being "interesting" based on:

1. **Topographic Anomaly** — Deviations in the terrain height map compared to the average of the surrounding 500m radius.
2. **Narrative Tempo** — The time elapsed since the player last discovered a "narrative beat" (a key item, a new area, a dialogue trigger). The longer the silence, the higher the "curiosity hunger," and the stronger the whisper signals.
3. **Cultural Density** — The presence of *non-functional* objects (furniture, banners, dead trees with carvings) often indicates a point of interest to a world-builder. The Ledger learns these patterns.

This algorithm runs locally on your machine with **butterfly-low performance overhead** (typically less than 1% CPU usage on a modern dual-core).

---

## 🧰 Troubleshooting Common "Cartographic Errors"

| Error | Likely Cause | Resolution |
|-------|--------------|------------|
| **"Aurora Bridge: Silence"** | The game process is not running or the version is mismatched. | Verify the game is running in windowed or borderless mode. Check `COMPATIBILITY.md`. |
| **"Motes Drifting Away"** | The overlay is active, but the spatial scan hasn't initialized. | Press `F5` to force a re-scan. |
| **"Rosetta Falter"** | Language packs are corrupted or missing. | In the settings, click **"Repair Narrative Files"** and restart the Ledger. |
| **"Atlas Cache Fragmented"** | The database is old or from a previous version. | Backup your `ledger.db` file, then run `--rebuild-cache` from the CLI. |
| **"High UI Latency"** | Background FPS limit is too low. | In settings, increase the "Overlay Refresh Rate" from 5Hz to 15Hz. |

---

## 🤝 Contributing: Join the Guild of Illuminators

We welcome contributors who see exploration as an art form. Whether you're a developer, a narrative designer, a translator, or a UX whiz, there's a place for you.

### Ways to Contribute
- **Write Lore:** Contribute thematic descriptions for items, locations, and regions in both English and Russian.
- **Improve the Translation:** Our "Rosetta" system is good, but human nuance is better.
- **Optimize the Algorithm:** Help us find better ways to weigh "curiosity" variables.
- **Build New "Moods"** — Add new color grading presets to the Aesthetic Overlay system.

### The "Checklist for Immersion"
Before submitting a PR, please ensure:
1. The UI designs respect the **"fade-into-background"** philosophy.
2. Any new text descriptions include both English and Russian variants.
3. Your code passes the existing test suite (`npm test` locally).
4. The feature doesn't require invasive access to the host game's memory.

---

## 🗂️ Repository Structure (A Map of the Maps)

```
cartographers-ledger/
├── /src
│   ├── /core           # Rust-based Echo Engine (Memory reads & analysis)
│   ├── /frontend       # TypeScript + React UI components
│   ├── /rosella        # NLP + Translation services
│   └── /aurora         # C++ Bridge for OS-level interaction
├── /profiles
│   ├── /minimalist
│   ├── /archivist
│   ├── /pathfinder
│   └── /dreamer
├── /assets
│   ├── /textures       # UI skin assets
│   ├── /modes          # Color grading LUTs
│   └── /sounds         # Optional, subtle UI audio cues
├── /docs
│   ├── COMPATIBILITY.md  # List of supported host applications
│   └── METAPHYSICS.md    # The philosophical design doc
├── /tests
│   ├── /unit
│   └── /integration
├── LICENSE.md
├── CONTRIBUTING.md
└── README.md           # You are here, traveler.
```

---

## ⚖️ License

### MIT License

Copyright (c) 2026 The Cartographer's Guild maintainers (public alias, not attached to a personal account).

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

**THE SOFTWARE IS PROVIDED "AS IS"**, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[Read the full license](https://github.com/cartographers-guild/ledger/blob/main/LICENSE.md).

---

## 🚨 Disclaimer: A Word on the Ethical Compass

**The Cartographer's Ledger is a tool for enhancing your personal experience within a digital world.** We do not condone, promote, or facilitate any form of network manipulation, server-side exploitation, or violation of a host application's terms of service.

- The Ledger operates strictly **locally** and **read-only**. It does not transmit any data externally.
- It does **not** automate gameplay, generate unfair advantages in online settings, or allow access to areas not otherwise reachable through organic gameplay.
- **We are not responsible for any account restrictions** imposed by a host application's developer, even if that restriction is triggered by a false positive on our memory-reading framework.
- The included "Item Indexer" only *catalogs* what you have *already found*. It does not reveal un-generated items or map positions.
- If your game has an anti-cheat system that prohibits *any* external reading, **do not** use this tool. Your compliance is your own responsibility.

By using The Cartographer's Ledger, you agree that you are using a **passive observation tool** and you hold the repository maintainers harmless from any consequences arising from the use of this open-source project.

---

## 📬 Support & Community

Need help or want to share your "cartographer's tales"?

- **Open an Issue** for bugs or feature requests — we try to respond within 48 hours (excluding holidays).
- **Join the Discord** (link in the repo description) for real-time chat, lore discussions, and profile sharing.
- **24/7 Availability** — Our issue tracker is monitored across multiple time zones. Community volunteers help ensure questions get answered around the clock.

**We value your feedback.** If you found a plot hole in our algorithm or a typo in our lore, let us know. Every whisper helps us guide future explorers.

---

## 🌟 Star History & The Road Ahead

**Version 2.4.7** brings the "Dreamer" profile and the new "Ashen Ruin" color mood. Our roadmap for **2026** includes:

- **Q1:** Support for new host titles (community-driven).
- **Q2:** The "Community Lore" opt-in databank, allowing you to anonymously share your favorite discovered resources (with your permission).
- **Q3:** The "Cartographer's Toolkit" — a public API for advanced users to build their own "Whisper" models.
- **Q4:** Full offline mode without any telemetry gathering.

If you like this project, consider **watching** (for updates) or **starring** (for morale). Both help us know that the path we're blazing is worth following.

---

## 📜 Final Words from the Developer's Desk (2026)

> "Maps are not just representations of space; they are records of memory. The Cartographer's Ledger is my attempt to bring the *memory* back to the *map*. I built this because I got tired of having to choose between playing a game and understanding it. I wanted both. So I made a tool that gives you the knowledge without taking away the surprise. It's a fine line to walk, but I hope... I hope this guide helps you find something you didn't know you were looking for."

— The Guild Steward (corporate alias, not a username, per repository guidelines)

---

**Begin your journey. The realm remembers all. But now, it will remember with you.** 🏔️✨