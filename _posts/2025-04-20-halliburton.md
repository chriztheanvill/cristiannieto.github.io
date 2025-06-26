
---
title: "Halliburton"
date: 2025-04-20
layout: page
categories: [portfolio]
tags: [linux,cpp]
---

# **Software Modernization at Halliburton**

**Role:** C++ Developer | **Team Size:** 2 | **Duration:** 2 Years  
**Technologies:** C++20, Qt, Qwt6, CMake, 3D Rendering, Linux Migration  

## **Project Overview**  

Halliburton, a global leader in energy services, required modernization of its legacy software to improve performance, maintainability, and compatibility with newer systems. My responsibilities included:  
- **Porting from Qwt5 to Qwt6** – Ensured compatibility with modern Qt while maintaining visualization accuracy.  
- **Migration from qmake to CMake** – Improved build system efficiency and cross-platform support.  
- **Migrate from Debian to RHEL-based Linux** Improving security & maintainability.  
- **Optimize 3D rendering** Using Qt 3D & OpenGL.  
- **Frontend & Backend Optimization** – Refactored legacy code in C++20 for better maintainability.  
- **Refactor legacy C++ into modern C++20** Improving performance & maintainability.  

### **Key Contributions & Technical Challenges**  

#### **1. Migration from Qwt5 to Qwt6**  
- **Challenge:**  
  - Qwt6 introduced **breaking API changes**, particularly in **plot rendering and scaling**.  
  - The legacy code relied on **deprecated Qwt5 features** (e.g., `QwtPlotZoomer`, `QwtPlotCurve`).  
- **Solution:**  
  - Developed **wrapper classes** to maintain compatibility with existing code.  
  - Implemented **automated regression tests** (using **Google Test**) to verify rendering accuracy.  
  - Optimized **real-time data plotting** by reducing unnecessary redraws.  

#### **2. Transition from qmake to CMake**  
- **Challenge:**  
  - The **monolithic qmake build** was slow (~15 min full rebuild) and hard to maintain.  
  - Dependency management was **manual** (`.pro` files with hardcoded paths).  
- **Solution:**  
  - Modularized the project into **logical CMake targets** (libraries, executables, tests).  
  - Integrated **FetchContent** for third-party dependencies (e.g., Boost, Eigen).  
  - Reduced build times **by 20%** using **Ninja** and **ccache**.  

#### **3. Linux Migration (Debian → RHEL-based Distro)**  
- **Challenge:**  
  - The legacy system relied on **Debian-specific packages** (`libssl1.0`, old glibc).  
  - Some proprietary drivers were **incompatible** with newer kernels.  
- **Solution:**  
  - Used **Docker containers** to test compatibility before deployment.  
  - Replaced deprecated system calls with **POSIX-compliant alternatives**.  
  - Worked with IT to ensure **secure package signing** for enterprise deployment.  

#### **4. High-Performance 3D Rendering (Qt 3D & OpenGL)**  
- **Challenge:**  
  - The existing **software-based renderer** struggled with large seismic datasets (>1M points).  
  - Frequent **UI freezes** during data updates.  
- **Solution:**  
  - Implemented **GPU-accelerated rendering** using **Qt 3D** and **OpenGL shaders**.  
  - Added **Level-of-Detail (LOD)** to dynamically reduce mesh complexity.  
  - Introduced **asynchronous data loading** (threaded QML workers).  

#### **5. Modern C++20 Refactoring**  
- **Applied:**  
  - **Concepts** (for safer template metaprogramming).  
  - **Coroutines** (for async data processing).  
  - **RAII & smart pointers** (eliminating memory leaks).  

## **Results & Impact**  
✔ **20% faster builds** (CMake + Ninja).  
✔ **Smoother 3D rendering** (60 FPS with OpenGL optimizations).  
✔ **Future-proof codebase** (C++20, Qt6, Qwt6).  
✔ **Easier maintenance** (modular CMake).  

---  

# **About Halliburton**  

Halliburton is one of the world's largest providers of products and services to the energy industry. With operations in over **70 countries**, it specializes in:

- **Oilfield drilling & exploration**  (drilling, evaluation, completion) 
- **Digital solutions** (AI, real-time data analytics)  
- **Hydraulic fracturing & reservoir management**  
- **Sustainable Energy Innovations**  

Our project modernized **critical geoscience visualization tools**, enabling engineers to analyze subsurface data more efficiently.  

### **Why This Project Mattered**  
- **Small team, big impact:** Despite only **two developers**, we delivered a **production-ready upgrade**.  
- **Performance-critical:** The software is used in **real-time drilling decisions**.  
- **Long-term sustainability:** The move to **CMake, C++20, and Qt6** extended the software’s lifespan.  

---  

### **Final Notes**  
This project was a **deep technical challenge**, requiring expertise in:  
✅ **Legacy modernization** (without breaking existing workflows).  
✅ **Cross-platform builds** (CMake, Docker).  
✅ **High-performance 3D graphics** (Qt3D, OpenGL).  
✅ **Linux system integration** (RHEL, security hardening).  

---  

## **Technologies Used**  
- **Languages:** C++20 (STL, Concepts)  
- **Frameworks:** Qt6 (QML, 3D), Qwt6  
- **Build System:** CMake  
- **OS:** RHEL-based Linux  

---  
