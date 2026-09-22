# ArogyaEdge – Digital Prototype Lab (SIH 2026)

**Custom Wearable Health Monitoring Band with On-Device Edge AI**

This is an interactive **software simulation** of the ArogyaEdge wearable for Smart India Hackathon 2026 (Hardware Category).

Judges and team members can explore the device, trigger heat-stress / fall / dehydration scenarios, switch between fully offline (Mode A) and hybrid (Mode B) operation, and inspect the internal hardware via cutaway view — without needing the physical prototype.

## Live Demo

After pushing to GitHub, enable **GitHub Pages** (Settings → Pages → Deploy from branch `main` / root).

Then open:

```
https://YOUR-USERNAME.github.io/ArogyaEdge-Lab/
```

Or open `index.html` directly in Chrome / Edge / Firefox (double-click or drag into browser).

> **Note:** Some browsers restrict ES modules when opening via `file://`. Prefer GitHub Pages or a local server (`python -m http.server`).

## Features

- **3D interactive band** – orbit, zoom, cutaway view showing ESP32-S3, MAX30102, MPU6050, battery, vibration motor
- **Live telemetry** – Heart rate, SpO₂, skin temperature, ambient temperature, risk score
- **Demo scenarios**
  - Normal (healthy baseline)
  - Heat Wave (outdoor worker)
  - Fall Event (elderly)
  - Dehydration (high activity)
- **Operating modes**
  - Mode A – Fully On-Band Edge AI (offline)
  - Mode B – Hybrid (band + phone)
- **Actions** – Start/pause monitoring, go offline, haptic test, reset
- **Event log** with privacy-first messaging

## How to Demo for Judges

1. Open the lab → click **Enter the lab**
2. Drag to orbit the band → click **Cutaway** to reveal internals
3. Select **Heat Wave** scenario → watch risk rise + alert
4. Click **Go Offline** → confirm system still works
5. Trigger **Fall Event** → SOS-style alert
6. Switch between Mode A / Mode B

## Tech

- Single-file HTML + Three.js (no build step)
- Runs entirely in the browser
- No backend / no account required

## Project Context

- **Problem Statement:** SIH 2026 – Secure, AI-powered Personal Health Companion (privacy-preserving, edge AI, heat-wave resilience)
- **Category:** Hardware
- **Key claim:** Low-cost (₹900–1600 prototype), offline-first, privacy-preserving wearable for Indian outdoor workers and elderly

---

**Simulation only · Not a medical device · All AI designed for on-device (ESP32-S3) inference**
