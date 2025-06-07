---
title: "Kosmos_GPS"
date: 2025-04-21
categories: [portfolio]
tags: [linux,cpp]
---

## 🧾 **Kosmos GPS - Embedded & Backend Development**

### Project Title: Vehicle Tracking System - Embedded Device & Backend Communication  
**Duration:** 2 years  
**Role:** Sole Developer  

---

### 🔧 Technologies Used:
- **C++17**
- **CMake** – Build system
- **Conan** – Package management
- **Sockets** – TCP/IP communication
- **Multi-threading** – For concurrent tasks
- **MySQL Connector/C++** – Database integration
- **Arduino-based hardware**

---

### 📌 Overview:

This project involved designing and implementing a complete vehicle tracking system from scratch. It included developing an embedded device to be installed in vehicles, capable of gathering real-time data such as geolocation and vehicle diagnostics. The collected data was then transmitted securely to a backend server for processing and storage.

The backend, also developed by me, handled incoming data streams, stored them in a MySQL database, and provided APIs for the frontend application.

---

### 🛠️ Key Features:

- **Embedded Device Setup**: Custom Arduino-like board programmed in C++17 to interface with GPS modules and vehicle OBD-II systems.
- **Data Acquisition**:
  - Real-time geolocation using GPS (compatible with Google Maps).
  - Vehicle diagnostics including speed, fuel level, engine status, etc.
  - Bidirectional communication between driver and control center via custom message protocol.
- **Communication Layer**:
  - Implemented TCP socket programming for stable client-server communication.
  - Multi-threaded architecture to handle GPS reading, vehicle sensor input, and network transmission concurrently.
- **Database Integration**:
  - Connected C++ backend to MySQL using MySQL Connector/C++.
  - Designed schema and wrote queries to store and update vehicle telemetry efficiently.

---

### 🏗️ Development Tools & Practices:
- **CMake** for cross-platform build configuration.
- **Conan** for dependency management.
- Version control with Git.
- Modular code structure for maintainability and scalability.

---

### ⚠️ Challenges & Solutions:

1. **Real-Time Data Synchronization**:
   - *Problem:* Handling multiple threads without data race conditions or performance bottlenecks.
   - *Solution:* Used mutexes and condition variables to safely share resources across threads. Prioritized critical sections and optimized thread sleep intervals.

2. **Unreliable Network Conditions**:
   - *Problem:* Intermittent connectivity caused data loss.
   - *Solution:* Implemented local caching on the device and automatic retry logic when connection was restored.

3. **GPS Signal Loss in Urban Areas**:
   - *Problem:* Inaccurate or missing location data in tunnels or dense cities.
   - *Solution:* Added dead reckoning logic using vehicle speed and heading data to estimate position until GPS signal reappeared.

4. **Cross-Platform Compilation**:
   - *Problem:* Building and testing on different OS environments.
   - *Solution:* Leveraged CMake and Conan to manage dependencies and automate builds across Linux and Windows.

---

### 🎯 Result:
A robust and scalable vehicle tracking system used in fleet management operations. The system improved operational visibility and allowed for better route planning, maintenance scheduling, and driver communication.

---

## 🧾 **Kosmos GPS - Web Interface & Fleet Management Dashboard**

### Project Title: Fleet Management Dashboard – PHP Laravel Web Application  
**Duration:** 2 years  
**Role:** Sole Developer  

---

### 🔧 Technologies Used:
- **PHP Laravel**
- **MySQL**
- **Google Maps API**
- **RESTful APIs**
- **Blade Templates**
- **JavaScript / jQuery**
- **HTML5 / CSS3**

---

### 📌 Overview:

As the sole developer, I designed and built a web-based dashboard to visualize and manage all tracked vehicles in real time. This dashboard served as the central hub for operators to monitor vehicle locations, set destinations, send messages, and analyze historical data.

---

### 🛠️ Key Features:

- **Real-Time Map Visualization**:
  - Integrated **Google Maps JavaScript API** to display live positions of vehicles.
  - Markers updated dynamically using AJAX calls.
- **Vehicle Status Panel**:
  - Displayed current vehicle info: location, destination, speed, fuel level, ignition status, and more.
- **Message Center**:
  - Operators could send and receive text messages to/from drivers through the embedded device.
- **Historical Tracking**:
  - Stored GPS logs in MySQL and allowed replay of past routes.
- **User Authentication & Roles**:
  - Admin and operator roles with protected routes using Laravel middleware.
- **APIs for Mobile Integration**:
  - RESTful endpoints for future mobile app integration.

---

### 🏗️ Development Tools & Practices:
- Built with **Laravel 8+**, using Eloquent ORM for clean database interactions.
- Blade templates for dynamic views.
- Structured controllers and services for maintainable code.
- Used Artisan commands for cron jobs and data cleanup.
- Deployed on Apache/Nginx with SSL support.

---

### ⚠️ Challenges & Solutions:

1. **Real-Time Updates Without WebSockets**:
   - *Problem:* Needed frequent updates without heavy polling.
   - *Solution:* Implemented long-polling technique with AJAX to reduce load while keeping UI responsive.

2. **Map Performance with Many Vehicles**:
   - *Problem:* Lag when rendering large numbers of markers.
   - *Solution:* Used marker clustering and only fetched visible vehicles based on zoom level and map bounds.

3. **Time Zone & Localization Issues**:
   - *Problem:* Users in different regions saw incorrect timestamps.
   - *Solution:* Used Laravel’s localization features and converted timestamps on the backend using user preferences.

4. **Secure Communication**:
   - *Problem:* Prevent unauthorized access to vehicle data.
   - *Solution:* Enforced strict API authentication using tokens and rate limiting.

---

### 🎯 Result:
A fully functional and intuitive dashboard that empowered operators to manage fleets effectively. The system is currently used by logistics companies for real-time monitoring and decision-making.

---
