# 💡 Advanced Motion-Activated Light Blueprint!

---
# Description

# 🌞🌙 Motion-Activated Lighting (Scene or Direct Lights) with Schedules, Night Mode, Sun Control & Failsafe

This Home Assistant blueprint allows you to control your lights using one or more motion sensors, with **day/night schedules**, **lux threshold**, **optional scenes**, **sunrise/sunset control**, and a **failsafe timer**. Includes snapshot restore of previous light states.

---

## ⚙️ Features

- ✅ Multiple motion sensors
- ✅ Optional manual switches to trigger lights
- ✅ Day and night modes (time-based or sun-based)
- ✅ Lux threshold control (optional)
- ✅ Scenes or direct lights
- ✅ Snapshot restore for previous light states
- ✅ Failsafe timer (automatically turns off lights after timeout)

---

## 🛠️ Inputs

| Input | Description | Default |
|-------|------------|---------|
| `motion_sensors` | Motion sensor(s) to trigger lights | None |
| `optional_switches` | Optional switches that can also trigger lights | [] |
| `light_entity` | Lights to control (used if no scene) | None |
| `scene_day` | Scene to activate during day (optional) | [] |
| `scene_night` | Scene to activate during night (optional) | [] |
| `day_lights` | Lights to turn on during day if no scene is set | [] |
| `night_lights` | Lights to turn on during night if no scene is set | [] |
| `lux_sensor` | Optional lux sensor | [] |
| `lux_threshold` | Only turn on lights if lux is below this | 50 lx |
| `use_sun_times` | Use sunrise/sunset instead of fixed times | false |
| `day_start` / `day_end` | Start and end times for day | 07:00 / 22:00 |
| `night_start` / `night_end` | Start and end times for night | 22:00 / 07:00 |
| `active_weekdays_day` | Active days for day mode | All days |
| `active_weekdays_night` | Active days for night mode | All days |
| `failsafe_timer` | Minutes before automatic light off | 30 |
| `input_text_last_scene` | Tracks last activated scene | None |

---

## 🏃‍♂️ How It Works

1. **Day Mode 🌞**
   - Motion detected during day time (or sunrise/sunset if enabled)
   - Lux below threshold (optional)
   - Activates either **day scene** or **day lights**
   - Snapshots current light state
   - Updates `input_text_last_scene` to `"day"`

2. **Night Mode 🌙**
   - Motion detected during night time (or sunset/sunrise if enabled)
   - Lux below threshold (optional)
   - Activates either **night scene** or **night lights**
   - Snapshots current light state
   - Updates `input_text_last_scene` to `"night"`

3. **Turn Off 💡**
   - When motion stops and lights are on
   - Restores previous snapshot after delay:
     - Day mode: 2 minutes
     - Night mode: 1 minute

4. **Failsafe ⏱**
   - Ensures lights do not stay on indefinitely
   - Activates after `failsafe_timer` if motion is gone and lights are still on
   - Turns off lights and logs action

---

## 🔗 Notes

- Works with **multiple motion sensors**.
- Optional **manual switches** can trigger lights.
- Supports **scenes or direct lights**.
- Can be used **with or without lux sensor**.
- Supports **sunrise/sunset timing** if enabled.

---

## 📌 Example Use Cases

- Hallway lights that turn on at night but only if dark 🌙
- Living room lights that react to motion during day and night 🌞🌙
- Kitchen lights that automatically turn off if forgotten ⏱
- Snapshots previous lighting state to restore ambience 🎨

---

**Enjoy your smart motion-controlled lighting!** 💡🚀



# 📦 Installation:

1️⃣ Import the blueprint into Home Assistant via the UI

2️⃣ Link your devices: motion sensor, main light, lux sensor, and (optionally) scenes or direct light entities

3️⃣ (Optional) Select a snapshot area if you want to restore all lights in that room when motion ends

4️⃣ Configure times, weekdays, and lux threshold as desired

5️⃣ Save & enjoy smarter, more flexible bathroom lighting!


### Support  
Questions or suggestions? Please open an issue in the [GitHub repo](https://github.com/razzietheman/Advanced-Motion-Activated-Light-Blueprint).

---

## Author  
Rasmus Sjöberg @razzietheman (https://github.com/razzietheman)
2025

---

Thank you for using and sharing!
