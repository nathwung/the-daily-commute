# 🗺️ The Daily Commute

[![Built with C++](https://img.shields.io/badge/Built%20with-C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)](https://isocpp.org/)
[![GUI with GTK](https://img.shields.io/badge/GUI-GTK-8BC34A?style=for-the-badge&logo=gnome&logoColor=white)](https://www.gtk.org/)
[![Pathfinding](https://img.shields.io/badge/Includes-A%2A%20Pathfinding-FF9800?style=for-the-badge&logo=mapbox&logoColor=white)]()
[![Map Data](https://img.shields.io/badge/Data-OpenStreetMap-7EBC6F?style=for-the-badge&logo=openstreetmap&logoColor=white)](https://www.openstreetmap.org/)

**The Daily Commute** is a fully interactive desktop map application built in **C++ with GTK** and rendered using **EZGL**. It provides a rich set of features to explore maps, plan routes, visualize real-time traffic, view points of interest, and simulate a full daily navigation experience — all with a clean and intuitive sidebar UI.

---

## 🚀 Features

### 🧭 Arrow Navigation
- Move around the map using the **arrow keys**
- Zoom with scroll or touchpad gestures

### 🗺️ Pick Map
- Select a city map from the **dropdown menu** to load its map

### 🧭 Find Path
- Click **two intersections** on the map to automatically draw the **optimal path**
- Uses **A\* pathfinding with turn penalties**
- Route is **color-coded based on live traffic**:
  - 🔴 Heavy  
  - 🟠 Moderate  
  - 🔵 Light
- A **sidebar panel** shows:
  - 🕒 Estimated travel time  
  - 📏 Total distance  
  - 🚦 Turn-by-turn driving instructions

### 🧹 Clear Path
- Clears the current path and sidebar route display so a new one can be planned

### 🚲 Transportation Routes
- Toggle **subway lines** and **bike routes** on the map for easier commute planning

### 🚦 Show Traffic Lights
- Adds a traffic light image at every intersection where a light is present  
- Visible when zoomed in closely for detailed navigation

### 🌙 Night Mode
- Switch between day and night themes to reduce eye strain

### 📌 Clear All Pins
- Removes all selected pins, intersections, and POIs from the map

### 🔎 Find Intersection
- Type two street names to automatically zoom to their **intersection location**

### 📍 POI Display
- Shows **points of interest** (POIs) such as restaurants, libraries, banks, etc.
- Clicking a POI opens a popup with:
  - 🏷️ Name  
  - 🏠 Address  
  - 🏷️ Category/type

### 🛣️ Street Info
- Click on any **street** to:
  - Drop a pin at the nearest intersection
  - View current **live traffic**, **weather**, and **road closure** status in the sidebar

### 🆘 Help Panel
- Accessible from the “Help” button
- Displays a quick-start guide with:
  - Emoji-labeled instructions  
  - Feature usage breakdown  
  - Visual key for traffic color coding

---

## 🛠 Tech Stack

- **Language**: C++  
- **GUI Framework**: GTK  
- **Rendering**: EZGL  
- **Pathfinding Algorithm**: A* with turn penalties and live traffic weighting  
- **Map Data**: OpenStreetMap (via `StreetsDatabaseAPI`)  
- **Features**: Real-time traffic, transit overlays, POI popups, directions, themes

---

## 🔗 Links

- 💻 **Source Code**: [GitHub Repository](https://github.com/nathwung/the-daily-commute)  
- 🎥 **Demo Video**: *Coming Soon*
  
