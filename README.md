# Bathroom Motion Light Blueprint

---
# Description

Advanced blueprint for bathroom lighting using a motion sensor, with separate day and night modes, customizable schedules, adjustable lux threshold, failsafe timer, and flexible control via scenes or direct light entities.
Includes smart snapshot/restore that can capture the state of a single light, a custom list of lights, or all lights in a chosen area before activation — restoring them exactly as they were when motion ends.

# Features

- Separate schedules for daylight and nightlight modes
- Choice between scenes or direct light control for each mode
- Optional area-based snapshot to restore all lights in a room to their exact previous state
- Customizable active weekdays for each mode
- Adjustable lux threshold to only turn on lights when it’s dark enough
- Dynamic failsafe timer for automatic turn-off after no motion
- Manual-friendly – won’t turn off lights you turned on yourself
- Fully UI-configurable, no YAML editing required

# Installation

1. Import the blueprint in Home Assistant via the UI.
2. Link your devices: motion sensor, main light, lux sensor, and (optionally) scenes or direct light entities.
3. (Optional) Select a snapshot area if you want to restore all lights in that room when motion ends.
4. Configure times, weekdays, and lux threshold as desired.
5. Save and enjoy smarter, more flexible bathroom lighting!

### Support  
Questions or suggestions? Please open an issue in the [GitHub repo](https://github.com/razzietheman/Smarter-Bathroom-Lighting-Blueprint).

---

## Author  
Rasmus Sjöberg (@razzietheman)  
2025

---

Thank you for using and sharing!  
