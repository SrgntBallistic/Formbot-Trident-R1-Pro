# Formbot Trident R1 Pro Build Guide & Special Considerations

## Overview

This document supplements the general Voron Trident build checklist with **kit-specific notes for the Formbot Voron Trident R1 Pro** kit.  
It references:

- Official Voron Trident manual (primary source of truth)
- Formbot’s own diagrams and documentation
- Community enhancements and observations
- Our general build guide

This guide assumes a **250mm build**, but is generally applicable to the **300mm/350mm trims**.

---

## ⚠️ Kit Scope & What’s Included

**Formbot R1 Pro kits include:**
- Core mechanical hardware, rails, belts
- BTT Manta M8P V2.0 Board & HDMI V1.2 Touchscreen :contentReference[oaicite:7]{index=7}  
- Pre-crimped wiring harness (USB-C between Pico and Pi) :contentReference[oaicite:8]{index=8}  
- Panels and structural parts

**Important note:**
- The kit *does not include* 3D-printed parts — you must source them separately (official PIF or other sources) :contentReference[oaicite:9]{index=9}

---

## 🧰 Pre-Build Kit Verification

Before beginning assembly:

### 1. Complete Parts and Diagrams
- Download the **Formbot Voron-Trident GitHub repo** (Diagrams folder included) :contentReference[oaicite:10]{index=10}
- Compare all parts to:
  - Official Voron Bill of Materials
  - Kit packing lists
- Verify rail lengths and extrusion counts

### 2. Missing Consumables / Small Parts
- Community notes that:
  - **BAT85 diode for Omron probe may *not* be included** — purchase separately if you plan to use that probe type :contentReference[oaicite:11]{index=11}
  - Extra hardware bags are often included — but verify lengths carefully

### 3. Tools & Materials
- Standard Hex/Wrench set
- Soldering iron / crimper (for minor harness modifications)
- Multimeter for polarity verification

---

## 📌 Wiring & Electronics Notes

### Pre-Crimped Harness
- Formbot harness:
  - Includes pre-crimped USB wiring for **BTT SKR Pico → BTT Pi 1.2**
  - Works, but polarity and cable management should be verified before routing

### Wiring Best Practice
- Use a multimeter to verify:
  - **Thermistor polarity**
  - **Fan polarity**
  
  Some connectors **may be pinned backwards** in the harness — confirm continuity before powering up :contentReference[oaicite:12]{index=12}

### Connectors for Bed & Probe
- Formbot does *not* typically include:
  - Wago bed connectors
  - Diode for Omron probe
- Community builds recommend adding:
  - Wago connectors for ease of bed removal
  - Inline connectors for thermistor and heater wiring :contentReference[oaicite:13]{index=13}

---

## 🔩 Mechanical / Frame Notes

### Kirigami Bed Frame
- Formbot includes a **Kirigami bed frame** instead of multiple extrusions
- Users report:
  - It is rigid but sometimes requires small adjustments for printed parts to fit perfectly :contentReference[oaicite:14]{index=14}

### StealthBurner / Hotend Integration
- As in general guide:
  - Dry-fit all components
  - Expect minor sanding or tolerance tweaks if using glass-filled filaments
- Pay attention to wire routing — Formbot harness may not match official diagrams exactly

---

## 🛠️ Firmware / Configuration

### BTT Manta & HDMI Touchscreen
- Formbot R1 Pro includes:
  - **BTT Manta M8P V2.0**
  - HDMI V1.2 touchscreen :contentReference[oaicite:15]{index=15}

### Klipper / Screen Setup
- Follow Formbot’s **configuration directory** on GitHub for firmware base
- Adjust based on:
  - Trident size
  - Probe/bed level sensor choice
  - Any mods (Tap, CanBus, etc.)

---

## 🚨 Common Community-Reported Gotchas

### Probe / Endstop Hardware
- Formbot kits may omit diode for Omron probe input — check before purchase/insert :contentReference[oaicite:16]{index=16}

### Wiring Polarity
- Kit wiring is pre-crimped — but polarity issues have been seen
  - Use multimeter to confirm before plugging components in :contentReference[oaicite:17]{index=17}

### Use Official Voron Manual for Geometry
- Formbot diagrams can differ from the official layout — always cross-verify with:
  - Voron Trident assembly manual
  - Formbot diagrams as a *reference*, not a replacement

---

## 🧾 References

- Voron Trident official documentation — **VoronDesign/Voron-Trident GitHub** :contentReference[oaicite:18]{index=18}  
- Formbot Trident manual/diagrams — **Formbot/Voron-Trident GitHub** :contentReference[oaicite:19]{index=19}  
- Formbot product page details — **formbot3d.com** :contentReference[oaicite:20]{index=20}  

---

*(End of Formbot-specific content.)*

