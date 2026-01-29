# HMDone

**HMDone** is a minimal, professional **PC-VR headset** designed for **external stereo-camera tracking**.  
It deliberately removes internal tracking complexity to achieve **deterministic, low-latency, and reproducible VR workflows**.

HMDone connects to the PC via a **single DisplayPort cable** and relies entirely on **external tracking systems** (e.g. EdgeTrack).

---

## Design Philosophy

HMDone focuses on doing **one thing well**:

- Display only
- No onboard tracking logic
- No heuristics
- No cloud dependency

All pose estimation is handled externally.

---

## Key Characteristics

- **No internal IMU**
- **No integrated cameras**
- **No inside-out tracking**
- **No cloud or account dependency**
- **PC-VR first**

HMDone is tracked in the same way as other tools such as **Pen3D** — purely via **stereo camera geometry**.

---

## Tracking Concept

- External **stereo camera system** (e.g. EdgeTrack)
- Optical markers mounted on the headset
- Full **6DoF pose estimation**
- Deterministic, geometry-based tracking
- Identical tracking pipeline for:
  - Headset
  - Pen3D
  - Other tracked tools

---

## Connectivity

- **DisplayPort (DP)** — video output
- Optional USB (power / EDID / future extensions)

No USB is required for tracking.

---

## Intended Use Cases

- Professional VR authoring
- CAD / DCC workflows
- Motion capture & R&D
- Simulation & training
- Deterministic VR input research

HMDone is **not** intended as a consumer all-in-one headset.

---

## Ecosystem

HMDone is designed to work as part of the **xtan.ai / EdgeTrack ecosystem**:

- **EdgeTrack** — external stereo tracking
- **CoreFusion** — multi-view fusion & calibration
- **MotionCoder** — semantic interaction layer
- **Pen3D** — precision 3D input device

---

## Roadmap

**Coming soon.**

---

## Status

Early development / prototyping stage.  
Hardware designs and documentation will be released incrementally.
