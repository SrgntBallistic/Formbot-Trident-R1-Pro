# Formbot Voron Trident R1 Pro  
## Build Checklist (All Sizes)

**Applies to:** Trident 250 / 300 / 350  
**Kit:** Formbot Voron Trident R1 Pro  
**Assumptions:**  
- Formbot-provided firmware/configs  
- TAP probing  
- CAN toolhead  
- Rapido hotend  

This checklist is intended to be used **during the build**, alongside:
- Official Voron Trident Manual
- General Trident Build Guide (Steve / Pooch)
- Formbot Special Considerations Guide

---

## Phase 0 – Pre-Build Verification

- [ ] Read Voron Trident manual
- [ ] Read Formbot GitHub documentation
- [ ] Inventory all hardware, electronics, and panels
- [ ] Confirm all printed parts are complete
- [ ] Install all heat-set inserts
- [ ] Verify inclusion of:
  - TAP probe
  - CAN toolhead boards
  - Nevermore filter
  - LED lighting
  - HDMI touchscreen

---

## Phase 1 – Frame Assembly

- [ ] Sort and label all extrusions
- [ ] Pre-install all T-nuts and nut bars
- [ ] Assemble frame on a flat surface
- [ ] Use snug → settle → tighten method
- [ ] Verify frame is square and flat

---

## Phase 2 – Linear Rails & Motion

- [ ] Clean and lubricate all rails
- [ ] Install rails with correct orientation
- [ ] Install rail end-stops
- [ ] Verify smooth motion by hand

---

## Phase 3 – Z Drive & Bed

- [ ] Install Z nut bars before Z drive
- [ ] Clean Z lead screws
- [ ] Verify parallel Z motion
- [ ] Install bed heater and thermal fuse
- [ ] Add aggressive strain relief to heater wiring

---

## Phase 4 – Toolhead (StealthBurner + Rapido)

- [ ] Dry-fit all StealthBurner printed parts
- [ ] Install Rapido hotend
- [ ] Confirm PT1000 thermistor configuration
- [ ] Install TAP probe
- [ ] Verify TAP mechanical movement
- [ ] Leave toolhead open until CAN is verified

---

## Phase 5 – Wiring & CAN Bus

- [ ] Remove all shipping zip ties and velcro
- [ ] Route wiring through cable chains
- [ ] Add strain relief at toolhead and controller
- [ ] Flash CAN firmware
- [ ] Verify CAN UUIDs and communication

---

## Phase 6 – Electronics & Screen

- [ ] Install Manta M8P and CB1 per Formbot docs
- [ ] Verify power jumpers and fuses
- [ ] Install HDMI touchscreen
- [ ] Route HDMI and USB cables safely
- [ ] Configure screen rotation and permissions

---

## Phase 7 – Enclosure & Accessories

- [ ] Install metal hinges loosely
- [ ] Mount panels and align before tightening
- [ ] Install Nevermore filter
- [ ] Verify airflow direction
- [ ] Install LED lighting
- [ ] Verify LED voltage before power

---

## Phase 8 – Firmware & First Power-On

- [ ] Verify printer.cfg matches hardware
- [ ] Confirm motor directions
- [ ] Confirm heater and fan polarity
- [ ] Power on with heaters disabled
- [ ] Verify endstops, TAP, and motion

---

## Phase 9 – Final Validation

- [ ] Verify TAP repeatability
- [ ] Perform Z-tilt adjustment
- [ ] Level bed
- [ ] Set belt tension gradually
- [ ] Perform low-speed test print
- [ ] Re-check fasteners after initial prints

---

## Final Notes

The Formbot R1 Pro integrates many advanced systems by default.  
Proceed slowly, validate often, and avoid closing assemblies until systems are verified.

---
