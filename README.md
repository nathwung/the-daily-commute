# 🗺️ The Daily Commute

[![Built with C++](https://img.shields.io/badge/Built%20with-C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)](https://isocpp.org/)
[![GUI with GTK](https://img.shields.io/badge/GUI-GTK-4E9A06?style=for-the-badge&logo=gtk&logoColor=white)](https://www.gtk.org/)
[![Pathfinding](https://img.shields.io/badge/Includes-A%2A%20Pathfinding-FF9800?style=for-the-badge&logo=mapbox&logoColor=white)]()
[![Map Data](https://img.shields.io/badge/Data-OpenStreetMap-7EBC6F?style=for-the-badge&logo=openstreetmap&logoColor=white)](https://www.openstreetmap.org/)

**The Daily Commute** is an interactive **desktop map application** built in **C++ using GTK and EZGL**, designed to simulate real-world urban navigation. Users can explore city maps, search for intersections, display POIs, and plan optimized routes using **A\*** pathfinding — all enhanced with **live traffic conditions**, **weather data**, and **transit overlays** for an immersive commute experience.

---

## 🚀 Features

### 🕹️ Arrow Navigation
- Move around the map using **arrow keys**
- Zoom using scroll wheel or trackpad

### 🌍 Pick Map
- Load any city map from a **dropdown menu**
- Supports over 15 global cities

### 🗺️ Find Path
- Click **two intersections** to draw the optimal route
- Or use **Find Path** dialog to enter two intersection name pairs
- Supports **partial street names** and **autocomplete dropdowns**
- Uses **A\*** pathfinding with turn penalties
- Route is **color-coded** by live traffic:
  - 🔴 Heavy  
  - 🟠 Moderate  
  - 🔵 Light
- Sidebar displays:
  - 🕒 Estimated travel time  
  - 📏 Total distance  
  - 🚗 Turn-by-turn directions

### 🔍 Find Intersection
- Enter **two street names** to zoom to their intersection
- Works with **partial name matches**
- Includes **live autocomplete suggestions**

### 📌 Clear All Pins
- Removes all selected intersections, paths, and POI pins

### 🧹 Clear Path
- Clears the current path and sidebar instructions

### 🚲 Transportation Routes
- Toggle:
  - 🚇 **Subway lines** (color-coded by line)
  - 🚴 **Bike routes** (highlighted in green)

### 🚦 Show Traffic Lights
- Displays traffic light **icons** at intersections where they exist
- Visible when zoomed in for better detail

### 🌙 Night Mode
- Switch between **light** and **dark** map themes

### 🏙️ POI Display
- Shows **points of interest (POIs)** like:
  - 🍕 Restaurants  
  - 🏦 Banks  
  - 📚 Libraries  
- Click a POI to view:
  - 🏷️ Name  
  - 🏠 Address  
  - 🗂️ Category/type  
  *(Info fetched via OpenStreetMap Nominatim API)*

### 🛣️ Street Info
- Click on any street to:
  - Drop a pin at the nearest intersection
  - View:
    - 🚦 Live traffic speed & congestion  
    - 🌦️ Weather data  
    - 🚧 Road closure status  
  *(Info pulled from TomTom & OpenWeatherMap APIs)*

### 🆘 Help Panel
- Access help from a **dedicated button**
- Emoji-labeled guide with usage tips and traffic color legend

---

## 🛠 Tech Stack

- **Language**: C++  
- **GUI Framework**: GTK  
- **Graphics/Rendering**: EZGL  
- **Pathfinding**: A\* with turn penalties & traffic weighting  
- **Map Data**: OpenStreetMap  
- **Live APIs**:
  - 🛣️ TomTom Traffic API  
  - 🌦️ OpenWeatherMap API  
  - 🏷️ OpenStreetMap Nominatim API  
- **Team Size**: 3

---

## 🚚 Courier Routing Backend (M4 Optimization)

A fully optimized **multi-location delivery routing algorithm** was developed in C++ for the Traveling Courier Problem, though it is not integrated into the GUI.

### 🔧 Features:
- **Multithreaded Dijkstra all-pairs precomputation**
- **Shared-mutex concurrent caching** for path and travel times
- **Greedy randomized routing** with tunable parameters:
  - Pickup and dropoff weighting
  - Density bonuses
- **2-opt optimization** for legality-preserving improvements
- **Multiple parallel trials** to ensure low-quality-of-result (QoR)
- **Dynamic trial count** based on problem size
- **Guaranteed legal solution** returned within **45 seconds**
