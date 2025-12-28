# Formbot Voron Trident R1 Pro  
## Special Considerations Guide (All Sizes)

**Applies to:** Trident 250 / 300 / 350  
**Kit:** Formbot Voron Trident R1 Pro  
**Firmware Baseline:** Formbot-provided configs wherever possible  
**Hotend:** Rapido (hotend-dependent notes clearly marked)

---

## How to Use This Guide

This document is a **supplement**, not a replacement, for:

1. **Official Voron Trident Assembly Manual** (primary source of truth)
2. **General Trident Build Guide (Steve / Pooch)**  
   – preparation, sequencing, and best practices
3. **Formbot documentation** (kit-specific deviations)

Use this guide **only where Formbot kits differ or need clarification**.

---

## Scope & Size Applicability

- All procedures apply equally to **250 / 300 / 350**
- Differences between sizes are limited to:
  - Extrusion length
  - Belt length
  - Wire length
- Assembly order and concepts remain identical

> ⚠️ Note:  
> The Voron **Trident does NOT use a kirigami bed frame**.  
> Kirigami beds are specific to **Voron V0** designs.

---

## Kit Overview (Formbot R1 Pro)

**Included:**
- Frame extrusions & hardware
- Linear rails
- Belts and pulleys
- Pre-crimped wiring harnesses
- Controller + display (kit-dependent)
- Panels

**Not included:**
- 3D printed parts (must be sourced separately)
- Some consumables (diodes, wagos, optional connectors)

Always inventory parts against:
- Voron BOM
- Formbot packing list
- Formbot GitHub diagrams

---

## Firmware & Configuration (Formbot Baseline)

🟦 **Formbot-specific**

- Use the **Formbot-supplied `printer.cfg`** as your baseline
- Treat Formbot configs as authoritative unless you know why you’re changing them
- Verify:
  - MCU type and pins
  - Stepper pin assignments
  - Endstop logic
  - Heater and fan definitions

### CAN Bus
- If Formbot provides CAN bus configs:
  - Use them as-is initially
  - Verify UUIDs and bus wiring before power-up
- Do not substitute generic Voron CAN configs blindly

---

## Wiring & Harness Considerations

🟦 **Formbot-specific**

- Harnesses are pre-crimped
- **Always verify polarity** with a multimeter:
  - Fans
  - Thermistors
  - Heater cartridge
- Remove **all shipping zip ties and velcro**
  before routing through cable chains
- Add strain relief near:
  - Toolhead
  - Controller board
  - Cable chain ends

> Best practice: trust documentation, not connector color.

---

## Rapido Hotend (Hotend-Dependent Section)

🟨 **Applies ONLY if using a Rapido**

- Verify heater cartridge wattage matches firmware limits
- Confirm thermistor type (commonly **PT1000**) in `printer.cfg`
- Ensure extra strain relief:
  - Rapido heater leads are stiff
- StealthBurner compatibility is supported, but:
  - **Dry-fit before final wiring**
  - Check clearance and cable exit path

> If using a different hotend (Revo / Dragon / V6),  
> skip this section and follow the general Trident guide.

---

## Common Formbot Kit Gotchas

🟥 **Critical checks**

- Some kits may omit small consumables:
  - Diodes (probe-dependent)
  - Wago connectors
- Connector pinouts may differ from expectations
- Always cross-check:
  - Formbot diagrams
  - Voron manual geometry

When in doubt:
> Voron manual defines geometry  
> Formbot docs define *how the kit implements it*

---

## Cross-Reference Map

| Topic | Reference |
|-----|----------|
| Mechanical assembly | Voron Trident Manual |
| Build sequencing & best practices | Steve / Pooch General Trident Guide |
| Wiring pinouts & configs | Formbot GitHub |
| Firmware baseline | Formbot `printer.cfg` |
| Hotend specifics | Hotend manufacturer docs |

---

## Final Advice

- Use **Formbot firmware first**
- Use **Steve / Pooch guide** to avoid mistakes
- Use **Voron manual** to validate geometry
- Verify everything electrical before power-up

This combination yields the smoothest Formbot Trident build experience.

---
