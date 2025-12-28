# Formbot Voron Trident R1 Pro  
## Integrated Special Considerations Guide (All Sizes)

**Applies to:** Trident 250 / 300 / 350  
**Kit:** Formbot Voron Trident R1 Pro  
**Firmware Baseline:** Formbot-provided configs wherever possible  
**Hotend:** Rapido (hotend-dependent notes clearly marked)

This document integrates:
- The General Trident Build Guide (Steve / Pooch)
- Formbot kit-specific features and deviations
- Differences from a stock Voron Trident

---

## How to Use This Guide

1. Use the **official Voron Trident manual** for geometry and assembly order.
2. Use the **Steve/Pooch General Trident Build Guide** for sequencing and best practices.
3. Use **this document** where Formbot kits differ or add advanced systems.

---

## Scope & Size Applicability

- All guidance applies to **250 / 300 / 350**
- Differences between sizes are limited to:
  - Extrusion length
  - Belt length
  - Wire length

> ⚠️ Note  
> The Voron Trident **does not use a kirigami bed frame**.  
> Kirigami beds are specific to Voron V0 designs.

---

## Integrated Formbot-Specific Features & Considerations

### TAP Bed Leveling (Included)
- Replaces inductive / Klicky probes
- Requires precise Z alignment and clean wiring
- Use Formbot TAP firmware values first

### Filament Runout Sensor (Included)
- Optional in stock Trident
- Enable only after extrusion tuning

### LED Chamber Lighting (Included)
- Verify voltage (5V vs 12V)
- Plan routing to avoid gantry and panel pinch points

### Nevermore Air Filter (Included)
- Community mod, integrated by Formbot
- Treat as a system: fan, wiring, airflow

### PT1000 Temperature Sensor (Included)
- Higher accuracy than NTC
- Requires correct `sensor_type` in firmware

### DLC-Coated CW2 Gears (Included)
- Longer life than brass
- Start with conservative tension

### Toolhead Breakout PCB (Included)
- Reduces wiring back to mainboard
- Connector seating and orientation are critical

### CAN Toolhead Boards (Included)
- Requires CAN firmware flashing and UUID management
- Bring CAN up before closing the toolhead

### Brass Nozzle Brush (Included)
- Not stock
- Test wipe moves slowly to confirm clearance

### Metal Panel Hinges (Included)
- More rigid than printed hinges
- Align panels before final tightening

### Bakelite Isolation Columns (Included)
- Provide thermal and electrical isolation
- Do not substitute metal spacers

### HDMI 5" Touch Screen (Included)
- Rotation and permissions must be set correctly
- Follow Formbot docs first

### StealthBurner + CW2 (Included)
- Afterburner was original Trident default
- Dry-fit everything before final wiring

### Manta M8P + CB1 Controller (Included)
- CB1 ≠ Raspberry Pi
- Follow Formbot OS and jumper documentation

### Moons Stepper Motors (Included)
- Z motors include integrated lead screws
- Clean and verify straightness before installation

### Silicone Bed Heater w/ Thermal Fuse (Included)
- Mains voltage
- Do not bypass thermal fuse
- Aggressive strain relief required

### Genuine Gates Belts (Included)
- Stretch less than generic belts
- Tension gradually and evenly

---

## Rapido Hotend (Hotend-Dependent Section)

Applies **only** if using a Rapido hotend.

- Verify heater wattage vs firmware limits
- Confirm thermistor type (commonly PT1000)
- Add strain relief for rigid heater leads
- Dry-fit Rapido + StealthBurner before final wiring

---

## Formbot R1 Pro vs Stock Voron Trident

| Feature | Stock Voron Trident | Formbot R1 Pro |
|------|-------------------|---------------|
| Bed Probing | Inductive / Klicky / Omron | TAP load-cell |
| Toolhead Wiring | Direct wired | CAN EBB boards |
| Extruder | CW2 optional | CW2 w/ DLC gears |
| Lighting | Not included | LED lighting |
| Air Filtration | Optional mod | Nevermore included |
| Thermistor | NTC common | PT1000 |
| Controller | Builder choice | Manta M8P + CB1 |
| Belts | Vendor varies | Genuine Gates |
| Panel Hinges | Printed | Metal |

---

## Final Guidance

The Formbot R1 Pro is best treated as:

> **A Trident with multiple advanced systems integrated from day one**

Use:
- Voron manual → geometry
- Steve/Pooch guide → sequencing
- This document → Formbot-specific deviations

Early planning and staged testing will prevent rework.

---
