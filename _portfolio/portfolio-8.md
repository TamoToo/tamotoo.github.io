---
title: "PocketCompanion: Interactive ESP32 Embedded Avatar & Physics Companion"
excerpt: "Portable, touch- and motion-reactive digital companion powered by an ESP32-S3 circular touch display, featuring a custom 60 FPS LVGL multi-surface avatar engine, QMI8658 IMU physics, and a Python JSON-to-C++ code generator.<br/><img src='/images/pocket_companion.jpg' alt='PocketCompanion Device' style='max-width: 380px; width: 100%; border-radius: 12px; margin-top: 10px;'>"
collection: portfolio
category: "projects"
order: 2
---

{% include base_path %}

<div class="project-media-container" style="max-width: 480px; margin: 20px 0;">
  <img src="{{ base_path }}/images/pocket_companion.jpg" alt="PocketCompanion Interactive Device" style="width: 100%; border-radius: 12px;">
</div>

### 🌟 Overview
**PocketCompanion** is a tiny, portable, and highly customizable living digital companion built on the **Waveshare ESP32-S3 1.28" Circular IPS Touch LCD Badge** housed in a custom 3D-printed enclosure. Designed to sit on a desk or travel in a pocket, it combines an autonomous mood state machine, capacitive touch gestures, and real-time 6-axis IMU physics to bring an expressive character to life at 60 FPS.

- **GitHub Repository:** [github.com/TamoToo/PocketCompanion](https://github.com/TamoToo/PocketCompanion)

---

### 🛠 Hardware & Embedded Architecture

1. **Microcontroller & Display Pipeline:**
   - Powered by an **ESP32-S3** driving a **240×240 circular IPS LCD** via **LVGL** at a smooth **~60 FPS** frame rate using dirty-rectangle rendering.
   - Housed in a compact 3D-printed enclosure with an integrated rechargeable USB-C battery.

2. **6-Axis IMU Physics & Capacitive Touch Sensing:**
   - **Native I2C QMI8658 IMU Driver:** Reads 3-axis accelerometer and gyroscope telemetry at 1000 Hz to drive real-time gravity eye-parallax, shake detection (triggering dizzy/angry reactions above 1.8g), and face-down orientation sensing (automatically putting the companion to sleep and waking it when picked up).
   - **CST816S Capacitive Touch Engine:** Custom gesture recognizer distinguishing quick pokes/taps (with escalating annoyance streaks), horizontal petting strokes (joyful squint reactions), and long-press holds (relax/nap transitions).

3. **Autonomous Behavior & Procedural Animation Engine:**
   - **Finite State Machine & Smoothstep Interpolation:** Autonomously transitions across idle moods (*Searching, Idle, Curious, Bored, Playful*) with smooth keyframe cross-fading (`smoothstep` expression lerping), randomized natural blinking, and procedural 2.5D depth parallax across multi-node cloud/body surfaces.
   - **Python JSON-to-LVGL Code Generator (`json_to_lvgl.py`):** Custom build-time compiler that parses declarative `*.avatar.json` definitions (exported from [Avatar Lab](https://github.com/smontlouis/bible-strong-avatar-lab)), computes compound bounding boxes and z-sorted node hierarchies, converts hex palettes to `RGB565`, and emits zero-overhead `constexpr` C++ headers (`Avatar.h`).

---

### Tech Stack
`C++ (Embedded / PlatformIO)`, `ESP32-S3`, `LVGL`, `Python (Codegen)`, `I2C (QMI8658 IMU & CST816S Touch)`, `3D Printing`
