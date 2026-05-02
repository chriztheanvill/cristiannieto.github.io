---
title: "Portfolio"
date: 2026-05-01
layout: page
categories: [portfolio]
tags: [zig, cpp, godot, raylib, sdl2, sqlite, emulation]
---

## Table of Contents

- [Portfolio - Systems Software Engineer](#portfolio---systems-software-engineer)
  - [About Me](#about-me)
  - [Featured Projects](#featured-projects)
    - [2D Action RPG - Godot 4](#2d-action-rpg---godot-4)
    - [Zig Dev-Tools Suite](#zig-dev-tools-suite)
      - [CPU / Console Emulator Suite](#cpu--console-emulator-suite)
      - [Godot Resource Manager](#godot-resource-manager)
      - [DB Inspector / Query Profiler](#db-inspector--query-profiler)
      - [Audio Player](#audio-player)
  - [Professional Experience](#professional-experience)
    - [Freelance Work](#freelance-work)
    - [Hired Position](#hired-position)
  - [Technical Skills](#technical-skills)
  - [Contact](#contact)

---

# Portfolio - Systems Software Engineer

Welcome to my portfolio — a showcase of my projects and technical work with a focus on **Zig**, **C++**, **emulation**, **dev tools**, and **game development** on Linux.

---

## About Me

7+ years building high-performance systems software, emulators, desktop dev tools, Qt/C++ applications, and game engines. I gravitate toward low-level work: memory inspection, database tooling, and anything that benefits from tight control over allocation and execution. Currently focused on **Zig 0.16**, **Godot 4**, **Raylib**, **SDL2**, **SQLite**, and **PostgreSQL**.

→ [About me](/cristiannieto.github.io/posts/about_me)

---

## Featured Projects

### 2D Action RPG - Godot 4

> Godot 4 | GDScript (strong typing) | SQLite | original IP

A lane-based action shooter blending Plants vs. Zombies-style strategy with Nioh/Borderlands loot and bullet-hell boss phases.

**2D Action RPG, Godot 4 / GDScript (Static Typing)**

- Top-down 2D action RPG with Souls-like combat: stamina management.
- Borderlands-style/Ni-oh procedural loot system: weapons and equipment with randomized stats, rarities, and prefixes.
- Data persistence with SQLite: inventory, player progress, and stats saved to a local database.
- Boss stages with bullet-hell mechanics: projectile patterns, dynamic phases, and difficulty scaling.
- Component-oriented architecture with statically typed GDScript, reducing runtime errors.
- Hierarchical State Machine (HFSM) for entity control: player, enemies, and bosses.

---

### Zig Dev-Tools Suite

> Zig 0.16 | Raylib | Raygui | SQLite | PostgreSQL | Linux (X11)

A collection of desktop developer tools built in Zig with direct C bindings via `addTranslateC` no intermediate abstraction layers.

#### CPU / Console Emulator Suite

Fetch/decode/execute architecture with memory state inspection and cycle-accurate timing.

| Emulator         | Status        | Notes                                                                   |
| ---------------- | ------------- | ----------------------------------------------------------------------- |
| **6502**         | ✅ Complete    | All addressing modes, cycle-accurate, NES / Atari compatible            |
| **CHIP-8**       | ✅ Complete    | 64×32 display, sound/delay timers, mapped keyboard                      |
| **Z80**          | ✅ Complete    | CB/DD/ED/FD extensions, full flag behaviour, I/O bus CP/M / ZX Spectrum |
| **RISC-V RV32I** | ✅ Complete    | R/I/S/B/U/J decoding, basic pipeline, word-addressable memory           |
| **GBA**          | 🚧 In progress | ARM7TDMI core, Thumb ISA, memory-mapped I/O                             |

Idiomatic Zig 0.16 throughout: explicit allocators, tagged unions for opcodes, comptime dispatch tables, zero GC overhead.

#### Godot Resource Manager

Standalone desktop app (not a plugin) that connects to Godot 4 projects to create and manage Resources and SQLite databases. Visual interface for schema inspection, table browsing and record editing, a lightweight alternative to Navicat/DataGrip aimed at game developers.

#### DB Inspector / Query Profiler

Visual database browser with query execution, result inspection and per-query timing. Targets SQLite and PostgreSQL. Direct C bindings via `addTranslateC`; designed to grow into a DataGrip-style tool for developers who prefer native, lightweight tooling.

#### Audio Player

Desktop audio player built with raygui integrated as a header-only library through a `raygui_impl.c` wrapper compiled from `build.zig`. Architecture designed for easy drop-in of audio backends (miniaudio, dr_libs).

---

## Professional Experience

### Freelance Work

- [Halliburton / Ultrasist](/cristiannieto.github.io/posts/halliburton) - qmake -> CMake migration; Qt5 -> Qt6 upgrade
- [Citi / Actinver](/cristiannieto.github.io/posts/actinver) - high-performance C++17/20 for financial data analysis
- [KosmosGPS](/cristiannieto.github.io/posts/kosmos_gps) - C++14 vehicle telemetry, MySQL, PHP Laravel dashboard

### Hired Position

- [MSC - Mediterranean Shipping Company](/cristiannieto.github.io/posts/msc) - C++14 / Banco Santander account

---

## Technical Skills

| Category         | Skills                                                                                                                            |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Zig**          | 0.16 (master) , `@cImport` / `addTranslateC` , `DebugAllocator` , `ArrayListUnmanaged` , `comptime` , `build.zig` , C/C++ interop |
| **C++ / Qt**     | C++17/20/26 , Qt5/Qt6 (Core, GUI, OpenGL, QML) , STL , Boost (Asio, Filesystem) , CMake , Meson , Conan , Vcpkg                   |
| **Emulation**    | 6502 , Z80 , CHIP-8 , RISC-V , GBA - fetch/decode/execute, memory bus, cycle-accurate timing                                      |
| **Graphics**     | Raylib , raygui , SDL2 , OpenGL (Core Profile) , GLSL , Vulkan (basics)                                                           |
| **Databases**    | SQLite , PostgreSQL , MySQL , SQL Server  MongoDB                                                                                 |
| **Performance**  | Valgrind , Perf , multithreading , TCP/IP , WebSockets , Boost.Asio                                                               |
| **Architecture** | SOLID , RAII , PIMPL , MVC/MVVM , ECS , DOD , Singleton , Factory , Observer                                                      |
| **DevOps / OS**  | Linux (Fedora Kinoite, Debian, Arch, NixOS) , Docker , Git , Shell scripting , cross-compilation                                  |
| **Other**        | Python , Lua , GDScript (Godot 4) , PHP , Node.js , Windows/Linux desktop                                                         |

---

## Contact

- **Email:** [enriquenietohdz@gmail.com](mailto:enriquenietohdz@gmail.com)
- **GitHub:** [github.com/chriztheanvill](https://github.com/chriztheanvill/)
- **LinkedIn:** [cristian-nieto-363984307](https://www.linkedin.com/in/cristian-nieto-363984307)

