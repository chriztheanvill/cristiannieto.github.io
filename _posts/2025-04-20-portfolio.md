---
title: "Portfolio"
date: 2026-05-01
layout: page
categories: [portfolio]
tags: [zig, cpp, godot, raylib, sdl2, sqlite, emulation]
---

## Table of Contents

- [Portfolio — Systems Software Engineer](#portfolio--systems-software-engineer)
  - [About Me](#about-me)
  - [Featured Projects](#featured-projects)
    - [2D Lane Shooter — Godot 4](#2d-lane-shooter--godot-4)
    - [Zig Dev-Tools Suite](#zig-dev-tools-suite)
      - [CPU / Console Emulator Suite](#cpu--console-emulator-suite)
      - [Godot Resource Manager](#godot-resource-manager)
      - [DB Inspector / Query Profiler](#db-inspector--query-profiler)
      - [Audio Player](#audio-player)
      - [2D Game Engine / Renderer](#2d-game-engine--renderer)
  - [Professional Experience](#professional-experience)
    - [Freelance Work](#freelance-work)
    - [Hired Position](#hired-position)
  - [Technical Skills](#technical-skills)
  - [Contact](#contact)

---

# Portfolio — Systems Software Engineer

Welcome to my portfolio — a showcase of my projects and technical work with a focus on **Zig**, **C++**, **emulation**, **dev tools**, and **game development** on Linux.

---

## About Me

7+ years building high-performance systems software — emulators, desktop dev tools, Qt/C++ applications, and game engines. I gravitate toward low-level work: memory inspection, database tooling, and anything that benefits from tight control over allocation and execution. Currently focused on **Zig 0.16**, **Godot 4**, **Raylib**, **SDL2**, **SQLite**, and **PostgreSQL**.

→ [About me](/posts/about_me)

---

## Featured Projects

### 2D Lane Shooter — Godot 4

> Godot 4 · GDScript (strong typing) · SQLite · original IP

A lane-based action shooter blending Plants vs. Zombies-style strategy with Nioh/Borderlands loot and bullet-hell boss phases.

**Architecture highlights**

- Custom **6×10 grid** with DXA coordinates, influence maps and adjacency zones — own architecture, no TileMapLayer.
- **Three-rhythm gameplay loop**: normal lane mode, slow-motion puzzle chest-opening mechanic, and boss bullet-hell; per-entity time scaling.
- Centralised `WorldManager` for entity registration, state propagation and simultaneous actor orchestration.
- `PlayerHFSMMovement` — discrete column-snapping with lerp smoothing; `EntityBase → ObstacleBase → Trap/Barricade` hierarchy.
- **SQLite** integration for loot persistence, Disgaea-style stat progression and player save data.

---

### Zig Dev-Tools Suite

> Zig 0.16 · Raylib · raygui · ImGui · SQLite · PostgreSQL · Linux (X11)

A collection of desktop developer tools built in Zig with direct C bindings via `addTranslateC` — no intermediate abstraction layers.

#### CPU / Console Emulator Suite

Fetch/decode/execute architecture with memory state inspection and cycle-accurate timing.

| Emulator         | Status        | Notes                                                                     |
| ---------------- | ------------- | ------------------------------------------------------------------------- |
| **6502**         | ✅ Complete    | All addressing modes, cycle-accurate · NES / Atari compatible             |
| **CHIP-8**       | ✅ Complete    | 64×32 display, sound/delay timers, mapped keyboard                        |
| **Z80**          | ✅ Complete    | CB/DD/ED/FD extensions, full flag behaviour, I/O bus · CP/M / ZX Spectrum |
| **RISC-V RV32I** | ✅ Complete    | R/I/S/B/U/J decoding, basic pipeline, word-addressable memory             |
| **GBA**          | 🚧 In progress | ARM7TDMI core, Thumb ISA, memory-mapped I/O                               |

Idiomatic Zig 0.16 throughout: explicit allocators, tagged unions for opcodes, comptime dispatch tables — zero GC overhead.

#### Godot Resource Manager

Standalone desktop app (not a plugin) that connects to Godot 4 projects to create and manage Resources and SQLite databases. Visual interface for schema inspection, table browsing and record editing — a lightweight alternative to Navicat/DataGrip aimed at game developers.

#### DB Inspector / Query Profiler

Visual database browser with query execution, result inspection and per-query timing. Targets SQLite and PostgreSQL. Direct C bindings via `addTranslateC`; designed to grow into a DataGrip-style tool for developers who prefer native, lightweight tooling.

#### Audio Player

Desktop audio player built with raygui integrated as a header-only library through a `raygui_impl.c` wrapper compiled from `build.zig`. Architecture designed for easy drop-in of audio backends (miniaudio, dr_libs).

#### 2D Game Engine / Renderer

Custom entity architecture on SDL2 with ImGui integrated as a runtime debugger and live state inspector during development.

---

## Professional Experience

### Freelance Work

- [Halliburton / Ultrasist](/posts/halliburton) — qmake → CMake migration; Qt5 → Qt6 upgrade
- [Citi / Actinver](/posts/actinver) — high-performance C++17/20 for financial data analysis
- [KosmosGPS](/posts/kosmos_gps) — C++17 vehicle telemetry, MySQL, PHP Laravel dashboard

### Hired Position

- [MSC — Mediterranean Shipping Company](/posts/msc) — C++14 / Boost.Asio / WebSockets · Banco Santander account

---

## Technical Skills

| Category         | Skills                                                                                                                            |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Zig**          | 0.16 (master) · `@cImport` / `addTranslateC` · `DebugAllocator` · `ArrayListUnmanaged` · `comptime` · `build.zig` · C/C++ interop |
| **C++ / Qt**     | C++17/20/26 · Qt5/Qt6 (Core, GUI, OpenGL, QML) · STL · Boost (Asio, Filesystem) · CMake · Meson · Conan · Vcpkg                   |
| **Emulation**    | 6502 · Z80 · CHIP-8 · RISC-V · GBA — fetch/decode/execute, memory bus, cycle-accurate timing                                      |
| **Graphics**     | Raylib · raygui · SDL2 · SFML2 · ImGui · OpenGL (Core Profile) · GLSL · Vulkan (basics)                                           |
| **Databases**    | SQLite · PostgreSQL · MySQL · SQL Server · MongoDB · schema design · query optimization                                           |
| **Performance**  | Valgrind · VTune · Perf · multithreading · TCP/IP · WebSockets · Boost.Asio                                                       |
| **Architecture** | SOLID · RAII · PIMPL · MVC/MVVM · ECS · DOD · Singleton · Factory · Observer                                                      |
| **DevOps / OS**  | Linux (Fedora Kinoite, Debian, Arch, NixOS, 15+ distros) · Docker · Git · Shell scripting · cross-compilation                     |
| **Other**        | Python · Lua · GDScript (Godot 4) · PHP · Node.js · Windows/Linux desktop                                                         |

---

## Contact

- **Email:** [enriquenietohdz@gmail.com](mailto:enriquenietohdz@gmail.com)
- **GitHub:** [github.com/chriztheanvill](https://github.com/chriztheanvill/)
- **LinkedIn:** [cristian-nieto-363984307](https://www.linkedin.com/in/cristian-nieto-363984307)