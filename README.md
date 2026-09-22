# 🍅 Pomodoro Tracker Pro

**Pomodoro Tracker Pro** is a lightweight Java Swing desktop application designed for productivity, clean aesthetics, and seamless workflow integration. Built with a sleek dark theme and an aggressive alert system, it ensures you never miss a focus phase or break boundary—even when working across multiple fullscreen applications.

---

## 🎨 Key Features

- **Standard Pomodoro Cycles:**
  - 🔴 **Focus:** 25 minutes (`P1`, `P2`, `P3`, `P4`)
  - 🟢 **Short Break:** 5 minutes (`I1`, `I2`, `I3`)
  - 🟣 **Long Break:** 15 minutes (triggered after 4 completed focus cycles)
- **System-Wide Always-on-Top Overlay:** End-of-cycle popup dialog that stays above all OS windows (macOS), allowing you to start the next phase with a single click.
- **Predicted Completion Time:** Calculates and displays the exact time your current phase will end in real time (e.g., `Start 15:20:00 • End 15:45:00`).
- **Smart Audio Alarms:** Automatically plays `alarm.mp3` via macOS native process (`afplay`) with fallback audio handling and multi-path file detection.
- **Visual Flash Feedback:** Flashes the interface gold when a timer expires for immediate visual notice.
- **Terminal-Style Activity Log:** Keeps a real-time timestamped record of starts, pauses, and completions.
- **Modern Dark UI:** Color palette inspired by Catppuccin and Dracula themes, featuring anti-aliased typography and interactive hover states.

---

## 🛠️ Tech Stack

- **Language:** Java (JDK 11+)
- **GUI Framework:** Java Swing / AWT (Zero external UI library dependencies)
- **Audio Execution:** macOS Native Process (`afplay`)
- **Date/Time API:** `java.time.LocalTime` and `DateTimeFormatter`

---

## 📁 Project Structure

```text
.
├── src/
│   ├── Main.java          # Core application logic and UI
│   └── alarm.mp3          # Audio alarm file (optional inside src)
├── alarm.mp3              # Audio alarm file in project root
├── .gitignore             # Git ignore rule specifications
└── README.md              # Project documentation
