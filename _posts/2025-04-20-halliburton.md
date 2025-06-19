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
- **Optimize 3D rendering** Using Qt 3D & OpenGL.  

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

## **Results & Impact**  
✔ **20% faster builds** (CMake + Ninja).  
✔ **Future-proof codebase** (Qt6, Qwt6).  
✔ **Easier maintenance** (modular CMake).  

---  

# **About Halliburton**  

Halliburton is one of the world's largest providers of products and services to the energy industry. With operations in over **70 countries**, it specializes in:

- **Oilfield drilling & exploration**  (drilling, evaluation, completion) 
- **Digital solutions** (AI, real-time data analytics)  
- **Hydraulic fracturing & reservoir management**  
- **Sustainable Energy Innovations**  

Our project modernized **critical geoscience visualization tools**, enabling engineers to analyze subsurface data more efficiently.  

---  

## **Technologies Used**  
- **Languages:** C++20 (STL)  
- **Frameworks:** Qt6 (QML), Qwt6  
- **Build System:** CMake  

---  
