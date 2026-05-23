# Apple Watch — Josh's AI-Connected Wearable ⌚

The Apple Watch is one of the most powerful ADHD management tools available. Haptic taps on the wrist cut through distraction in a way phone notifications never can. Here's everything we can do with it.

---

## 🧠 ADHD Superpowers

### Time Blindness Fix
ADHD brains are notorious for losing track of time completely. The watch fights this:
- **Taptic time** — enable "Taptic Time" in Watch settings: the watch *taps morse code for the time* on your wrist every hour. You always know roughly what time it is without looking.
- **Chime every hour** — subtle audio/haptic chime so time never sneaks away
- **Custom interval timers** — "check in with the kids in 20 min" without breaking focus

### Focus Session Timer (Pomodoro on Wrist)
- Set a 25-min timer via Siri: *"Hey Siri, 25 minute timer"*
- Watch taps you when done — no phone needed, no distraction
- Works while coding, doing Saimek AI work, etc.

### Discrete Reminders
- Haptic notifications don't disturb Allison or the kids
- Can receive important alerts (TOWER down, calendar event) without pulling out phone
- Great for Costco shifts — check alerts without getting caught on your phone

---

## 🏠 Family Automation via Apple Watch

### Alexa + Shortcuts Integration
Apple Shortcuts can trigger Alexa routines via webhook. This means your watch can:

| Watch Action | What Happens |
|---|---|
| Tap a complication | Starts Avery's bedtime routine on Alexa |
| "Hey Siri, kids to bed" | Triggers full bedtime sequence (lights + story) |
| Double-tap (gesture) | Starts Elias's focus timer + ambient music |
| "Hey Siri, family meeting" | Sends a notification to Allison's iPhone |

### TOWER / Saimek AI Alerts
- Get a wrist tap if a TOWER service goes down (SABnzbd, Plex, Sonarr)
- Download complete notification when Radarr/Sonarr grabs something
- Ollama job complete alert when a long inference finishes on project-insight

---

## 💤 Sleep Tracking

The watch can track Josh's sleep — and since Avery's sleep affects the whole family:

- **Sleep score correlation** — track how Avery's rough nights affect Josh's sleep quality
- **Heart rate during sleep** — stress indicator, useful for ADHD/anxiety pattern awareness
- **Sleep consistency** — the watch will nudge you toward a consistent bedtime (also helps ADHD)
- **Wind-down reminder** — watch taps you 30 min before target bedtime

### To enable:
1. Watch app on iPhone → Sleep → Set a Sleep Schedule
2. Enable "Track Sleep with Apple Watch"
3. Wear it to bed (charge it during morning routine instead)

---

## 💓 Health & Stress Monitoring

| Feature | Why It Matters for Josh |
|---|---|
| **Heart Rate** | High HR = stress spike — know when you need a break |
| **Mindfulness app** | 1-min breathing exercises, helpful during stressful Costco shifts |
| **ECG** | One-tap heart check |
| **Noise levels** | Alerts if environment is too loud (useful with two kids!) |
| **Activity rings** | Gamified movement — ADHD brains respond well to visual goals |
| **Irregular rhythm notification** | Passive health monitoring |

---

## ⌚ Best Complications to Set Up

Complications are the small widgets on your watch face. Recommended layout:

| Position | Complication | Why |
|---|---|---|
| Top left | **Timer** | One-tap Pomodoro |
| Top right | **Calendar** | Next event always visible |
| Middle | **Time + date** | Obviously |
| Bottom left | **Activity rings** | Daily movement motivation |
| Bottom right | **Weather** | Quick glance |

**Best watch face for ADHD**: **Modular** or **Infograph** — maximum information density, no distractions.

---

## 🔧 Shortcuts to Build

These are Apple Shortcuts that run on iPhone/Watch:

### 1. Avery Bedtime 🌙
```
Trigger: Watch tap or "Hey Siri, Avery bedtime"
Actions:
  1. Send webhook → Alexa "avery-bedtime" routine
  2. Start 30-min timer on watch
  3. Send notification to Allison's phone: "Avery bedtime starting"
```

### 2. Focus Mode 🎯
```
Trigger: Watch tap or "Hey Siri, focus time"  
Actions:
  1. Enable iPhone Focus mode (silence notifications)
  2. Start 25-min timer
  3. Play ambient music on HomePod/Alexa
```

### 3. TOWER Status 🖥️
```
Trigger: "Hey Siri, tower status"
Actions:
  1. Fetch http://tower:80 (health check)
  2. Speak result: "Tower is up" or "Tower is down"
```

### 4. Brain Dump 🧠
```
Trigger: Watch tap or "Hey Siri, brain dump"
Actions:
  1. Open Voice Memos — record a thought
  2. Later: AI transcribes and organizes into tasks in life-os notes/
```

---

## 📲 Settings to Change Now

In the **Watch app** on iPhone:

1. **Taptic Time** → My Watch → Sounds & Haptics → Taptic Time → turn ON
2. **Raise to Speak** → turn ON (Siri without saying "Hey Siri")
3. **Haptic Alerts** → set to Prominent
4. **Notifications** → only let through Calendar, Reminders, and important apps
5. **Sleep** → set a sleep schedule and enable sleep tracking
6. **Theater Mode shortcut** → useful for Costco (silences without turning off)

---

## 🔮 Future Ideas

- **Custom watch app** — a simple complication that shows Avery's bedtime countdown
- **Stress-based focus alerts** — if heart rate spikes during work, watch suggests a 2-min break
- **Family location glance** — see that Elias got home from school via watch complication
- **Saimek AI job monitor** — long AI inference running on project-insight → watch tap when done
