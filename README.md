# 🗺️ The Daily Commute

[![Built with C++](https://img.shields.io/badge/Built%20with-C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)](https://isocpp.org/)
[![GUI with GTK](https://img.shields.io/badge/GUI-GTK-4E9A06?style=for-the-badge&logo=gtk&logoColor=white)](https://www.gtk.org/)
[![Pathfinding](https://img.shields.io/badge/Includes-A%2A%20Pathfinding-FF9800?style=for-the-badge&logo=mapbox&logoColor=white)]()
[![Map Data](https://img.shields.io/badge/Data-OpenStreetMap-7EBC6F?style=for-the-badge&logo=openstreetmap&logoColor=white)](https://www.openstreetmap.org/)

The Daily Commute is an interactive desktop map application built in C++ using GTK and EZGL, designed to simulate real-world urban navigation. Users can explore city maps, search for intersections, display POIs, and plan optimized routes using A* pathfinding — all enhanced with live traffic conditions, weather data, and transit overlays for an immersive commute experience.

---

## 🚀 Features

### 🕹️ Arrow Navigation
- Pan across the map using **arrow keys**
- Zoom using scroll wheel or touchpad

### 🌍 Pick Map
- Select a city map via a **dropdown menu**
- Supports over 15+ global cities

### 🗺️ Find Path
- Click **two intersections** to find the **optimal path**
- Pathfinding uses **A\*** algorithm with turn penalties
- Path is **color-coded by live traffic data**:
  - 🔴 Heavy  
  - 🟠 Moderate  
  - 🔵 Light
- Sidebar displays:
  - 🕒 Estimated travel time  
  - 📏 Total distance  
  - 🚗 Step-by-step directions (turns included)

### 🧹 Clear Path
- Clears the current route and instructions panel

### 🚲 Transportation Routes
- Toggle overlays for:
  - 🚇 **Subway Lines** (color-coded by line)  
  - 🚴 **Bike Routes** (highlighted green)

### 🚦 Show Traffic Lights
- Renders traffic light **icons** at intersections
- Only visible when zoomed in

### 🌙 Night Mode
- Toggle between **light** and **dark** map themes

### 📍 Clear All Pins
- Clears all dropped pins, selected intersections, and overlays

### 🔍 Find Intersection
- Enter two **street names** to automatically zoom to their intersection

### 🏙️ POI Display
- Shows Points of Interest (POIs) like:
  - 🏫 Libraries  
  - 🍽️ Restaurants  
  - 🏧 Banks  
- Click to view:
  - 🏷️ Name  
  - 🏠 Address  
  - 🗂️ Category/type  
  *(fetched via OpenStreetMap API)*

### 🛣️ Street Info
- Click any street to:
  - Drop a pin at its **nearest intersection**
  - View:
    - 📊 Live traffic speed & congestion  
    - 🌦️ Real-time weather info  
    - 🚧 Road closure status  
  *(fetched via TomTom and OpenWeatherMap APIs)*

### 🆘 Help Panel
- One-click **Help** button shows:
  - 📖 Quick-start instructions  
  - 🧭 Traffic legend & usage guide  
  - Emoji-labeled features

---

## 🛠 Tech Stack

- **Language**: C++  
- **GUI Framework**: GTK  
- **Rendering**: EZGL  
- **Pathfinding**: A\* with turn penalties & traffic weighting  
- **Map Data**: OpenStreetMap (`StreetsDatabaseAPI`, `OSMDatabaseAPI`)  
- **Live APIs**:
  - 🚦 TomTom Traffic API  
  - 🌦️ OpenWeatherMap API  
  - 🗺️ OpenStreetMap Nominatim API

---

## 🔗 Links

- 💻 **Source Code**: [GitHub Repository](https://github.com/nathwung/the-daily-commute)  
- 🎥 **Demo Video**: *Coming Soon*
