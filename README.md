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

## Synthetic XR

The headset may not need onboard XR cameras if the experience is driven by a **synthetic XR scene**—for example, rendering from a tracked **ROI point cloud** or **proxy geometry** instead of real-world passthrough video. This can reduce headset weight and complexity.

For limited real-world context, a simple approach is to mount a **single RGB camera** (centered between the stereo cameras) and use it only to add **lightweight color information** to the ROI—e.g., **colored points** or a sparse texture overlay—rather than streaming full-resolution passthrough.

> **Note:** Full real-world integration is possible, but works best when the environment is **mostly static**. In highly dynamic scenes (moving objects, changing lighting, fast motion), the reconstruction becomes more constrained and passthrough fidelity may be limited.

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

## Roadmap

**Coming soon.**

---

## Status

Early development / prototyping stage.  
Hardware designs and documentation will be released incrementally.
