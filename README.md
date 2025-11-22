# Path Drawer 
It is a lightweight desktop application for designing, editing and exporting robot routes. I developed this application so my university robotics team wouldn't have to spend time manually programming routes. This README summarizes the application's purpose, main features, usage, and the planned v2.0 professional refactor.

## Quick summary
- **Language & stack**: Python (PyQt / Qt), YAML for route export, small helper scripts for node integration.
- **Primary use**: interactive route design for competition/field robots, with exportable route actions.

## What this app does
- Visual route editor: draw and edit paths on a grid or background map.
- Set the robot's turning angle: set the robot's turning angle at each waypoint.
- Grid precision: change the number of grid cells to increase or decrease route precision.
- Route & background management: load previously saved routes, load a different board/background image, and continue editing.
- Appearance controls: change the grid color and toggle angle indicators for waypoints.
- Export: generate YAML / simple formats consumable by robot control nodes.
- Lightweight node integration: example ROS2 node code is included for quick testing and simulation.

## Project structure
- `path_drawer_app_code/`: main PyQt application source (UI windows, Route model, helpers)
- `path_drawer_node/`: example ROS2 node and packaging for robot-side integration

## Screenshots
- Start window:
<p align="center">
  <img src="Screenshoots/Start_window.png"/>
</p>
    
- Main window:
<p align="center">
  <img src="Screenshoots/Main_window.png"/>
</p>
  
- Color window:
<p align="center">
  <img src="Screenshoots/Color_window.png"/>
</p>

## Version 2.0 — professional refactor (current roadmap)

I am actively developing a v2.0 with the following goals and improvements:

- **SOLID principles applied**: the codebase is being refactored to follow Single Responsibility, Dependency Inversion and other SOLID principles so that components are decoupled and testable.
- **Modular, professional file layout**: files will be reorganized into clear packages (`src/`, `ui/`, `core/`, `resources/`, `controllers/`) to match industry standards and ease maintenance.
- **Polished UI**: redesign of colors, typography and iconography to present a professional product. 
- **Route actions and automation**: full route authoring workflow — users will be able to create an entire route with ordered robot actions (e.g., drive to point, wait, actuate mechanism) and export a single, robot-ready plan. This enables immediate competition usage.

## Contact & hiring note
If you're interested in hiring or reviewing more of my work, please check the public repos in my GitHub profile or contact me directly. I originally developed this project as tooling for my university robotics team; additional robot-specific integrations live in private team repositories.

If you need more details, feel free to contact me via my GitHub profile.


