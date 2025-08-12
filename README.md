# Bathroom Motion Light Blueprint

---
# Description

💡 Advanced Motion-Activated Bathroom Light Blueprint – Now in English! V2.2

Say goodbye to basic “motion-on / timeout-off” automations – this blueprint gives you full and real control over your bathroom lighting.

✨ Features:
✅ Separate schedules for daylight and nightlight modes
✅ Custom active hours and weekdays – perfect for weekdays vs weekends
✅ Choice between scenes or direct light control for each mode
✅ Optional area-based snapshot to restore all lights in a room to their exact previous state
✅ Adjustable lux threshold – only turns on when it’s dark enough
✅ Dynamic failsafe timer for automatic turn-off after no motion
✅ Manual-friendly – won’t turn off lights you turned on yourself
✅ Fully UI-configurable – no YAML editing required

🔧 Changes Made in V2.2:
1️⃣ Separate time windows and weekdays for each scene

🌞 Daylight Scene: active start time day, active end time day, active weekdays day

🌙 Nightlight Scene: active start time night, active end time night, active weekdays night

2️⃣ Logic split for scene control – now respects both time and weekday for better precision

3️⃣ Added snapshot/restore feature:

Capture and restore a single light

Capture and restore a custom list of lights

Capture and restore all lights in a chosen area

🎯 Benefits of This Update:
💪 More flexibility – tailor lighting to your lifestyle
🎯 Better control – works great for night shifts, early risers, or lazy weekends
📈 Scalable – easy to extend (e.g., “Evening Relax Scene” or “Cleaning Mode”)
🌙 Smart night mode – switches scenes automatically outside your preferred schedule
💡 Adjustable lux threshold – only turns on when it’s actually dark enough
⏱ Failsafe timer – set your own timeout; light turns off only if no motion is detected
🙌 Manual-friendly – won’t shut off lights you turned on yourself
🛠 Designed to be fully UI-configurable – no YAML tweaking needed

📦 Installation:
1️⃣ Import the blueprint into Home Assistant via the UI
2️⃣ Link your devices: motion sensor, main light, lux sensor, and (optionally) scenes or direct light entities
3️⃣ (Optional) Select a snapshot area if you want to restore all lights in that room when motion ends
4️⃣ Configure times, weekdays, and lux threshold as desired
5️⃣ Save & enjoy smarter, more flexible bathroom lighting!

### Support  
Questions or suggestions? Please open an issue in the [GitHub repo](https://github.com/razzietheman/Smarter-Bathroom-Lighting-Blueprint).

---

## Author  
Rasmus Sjöberg (https://github.com/razzietheman @razzietheman)
2025

---

Thank you for using and sharing!
