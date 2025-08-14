# # Motion-Activated Lighting Blueprint (v3.0)

![Home Assistant](https://www.home-assistant.io/images/favicon-192x192.png)

## Description
This Home Assistant blueprint lets you control your lights based on:

- Motion sensors
- Optional manual switches
- Day/Night schedules or sunrise/sunset
- Adjustable lux threshold
- Optional workday sensor
- Snapshot restore of previous light states
- Dynamic failsafe timer with gradual turn-off

### Features
- Automatic Day and Night modes
- Ability to use scenes or direct light control
- Lux threshold to prevent unnecessary light activation
- Optional workday sensor logic
- Failsafe timer for automatic light turn-off
- Logging of all events in Home Assistant Logbook
- Gradual light turn-off for smooth transitions

---

## Inputs

| Name | Description |
|------|------------|
| Motion Sensor(s) | Motion sensors that trigger the automation |
| Optional Manual Switch | Switches that can also trigger the lights manually |
| Lights | Lights to control if no scenes are set |
| Day Scene / Night Scene | Scenes to activate during day/night |
| Day Lights / Night Lights | Lights to turn on during day/night if no scenes are set |
| Lux Sensor | Optional sensor for light level (lx) |
| Lux Threshold | Maximum lux value for activating lights |
| Use Sunrise/Sunset | Enable to determine day/night based on the sun |
| Workday Sensor | Optional sensor for workday logic |
| Failsafe Timer | Timer for automatic light turn-off |
| Input Text – Last Scene | Tracks the last activated scene/mode |
| Light Duration Day/Night | Duration lights stay on after motion stops |

---

## Installation

1. Copy the blueprint YAML into Home Assistant via:  
   `Configuration > Blueprints > Import Blueprint`.
2. Create an automation based on the blueprint.
3. Fill in all inputs according to your setup:
   - Motion sensors
   - Lights or scenes
   - Optional lux sensor and threshold
   - Day/Night times or sun-trigger
   - Optional workday sensor
   - Failsafe timer and light duration

---

## Tips

- Using both lux sensor and sun-trigger provides automatic adaptation to both daylight and sun position.
- Scenes are optional – if not using scenes, the blueprint will control Day/Night Lights directly.
- The failsafe timer prevents lights from staying on too long.
- All automation events can be tracked via **Logbook** in Home Assistant.

---

## Example Use Cases

- **Hall or Entrance**:
  - Day: Turn on lights when motion is detected if lux < 100
  - Night: Turn on dimmed lighting at night
- **Kitchen**:
  - Use scenes for different moods (day/night)
  - Failsafe timer of 10 minutes to automatically turn off lights

---

## License
This blueprint is open-source and free to use, modify, and share.

---

### Support  
Questions or suggestions? Please open an issue in the [GitHub repo](https://github.com/razzietheman/Advanced-Motion-Activated-Light-Blueprint).

---

## Author  
Rasmus Sjöberg @razzietheman (https://github.com/razzietheman)
2025

---

Thank you for using and sharing!
