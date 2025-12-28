# Voron Trident – Comprehensive Build Guide & Checklist
*(Compiled from Steve / Pooch official Trident build streams, Videos 1–6)*

> This checklist is intended to be used **alongside** the official Voron Trident Assembly Manual.  
> It focuses on **preparation, sequencing, pitfalls, and build-quality improvements** learned during real builds.

---

## Printer Context
- Printer: **:contentReference[oaicite:0]{index=0}**
- Applies to: Trident 250 / 300 / 350
- Notes include **LDO kit–specific differences** where applicable

---

# PHASE 0 – BEFORE YOU START (CRITICAL PREP)

## 0.1 Read ALL Documentation First 🟥
- Official Voron Trident Manual
- Your **kit vendor documentation**
  - **LDO kits include intentional deviations**
- LDO docs: https://docs.ldomotors.com

**Manual reference**
- *“Before You Begin”*
- *“Kit Variations / Notes”*

---

## 0.2 Organize Extrusions (DO THIS FIRST) 🟥
- Lay out all extrusions on a large surface
- Sort by:
  - Length
  - Orientation (front / rear / vertical / gantry)
- Label with painter’s tape:
  - `FRONT_BOTTOM`
  - `REAR_VERTICAL`
  - `Y_GANTRY_LEFT`

**Why**
- Several extrusions look identical but are not
- Orientation mistakes cause silent frame errors

---

## 0.3 Pre-Install T-Nuts and Nut Bars 🟥

### LDO-Specific 🟦
- LDO provides **pre-drilled T-nut bars**
- These **must be installed before frame assembly**

Install **before bolts touch anything**:
- Z-axis nut bars
- Linear rail nut bars
- Any extrusion that *might* need a nut later

> Undoing the frame to add a missing T-nut is one of the most common Trident mistakes.

---

## 0.4 Prepare Heat-Set Inserts 🟥
- Identify **all printed parts** requiring inserts
- Install inserts **before assembly**, not mid-step

**Recommended**
- Press-style tools (Naomi Wu / Atom / similar)
- ~300 °C for ABS / ASA

---

## 0.5 Workspace Setup 🟥
- Flat reference surface (granite, quartz, thick MDF)
- Clamps
- Painter’s tape
- Digital calipers
- Anti-fatigue mat (you’ll be standing a lot)

---

# PHASE 1 – FRAME ASSEMBLY

**Manual reference**
- *“Frame Assembly”*

## 1.1 Build on a Flat Surface 🟥
- Let gravity help seat extrusions
- Rotate frame frequently during assembly

---

## 1.2 Use the “Snug → Settle → Tighten” Method 🟥
For blind joints:
1. Snug bolts lightly
2. Let extrusion shift naturally
3. Loosen once
4. Final tighten

Prevents twist locked into the frame.

---

## 1.3 Add Washers to Blind Joints (Advanced) 🟦
- Washer under bolt head:
  - Reduces friction
  - Prevents extrusion rotation
- **Especially important for Y-gantry supports**

---

## 1.4 Measure Critical Spacing Early 🟥
- Y-gantry extrusion spacing
- Z vertical alignment

**Techniques used**
- Printed spacers
- Temporary extrusion spacers with painter’s tape

> Do not eyeball gantry spacing.

---

## 1.5 Do NOT Chase Perfect 🟨
- Sub-millimeter variance is normal
- Flat + consistent > theoretically perfect

---

# PHASE 2 – LINEAR RAILS & MOTION

**Manual reference**
- *“Linear Rails”*
- *“Motion System”*

## 2.1 Clean Rails 🟥
- Wipe shipping oil
- Relube with light machine oil

---

## 2.2 Install Rail End-Stops 🟥
- Install immediately after rails
- Prevents carriage overruns during early testing

---

## 2.3 LDO Rail Differences 🟦
- LDO kits may mix:
  - MGN9
  - MGN12
- Hole spacing differs
- Follow **LDO documentation**, not generic assumptions

---

# PHASE 3 – Z DRIVE & BED

**Manual reference**
- *“Z Drive Assembly”*
- *“Bed Assembly”*

## 3.1 Install Z Nut Bars BEFORE Z Drive 🟥
Easy to forget. Painful to fix later.

---

## 3.2 Optional Kinematic Bed Mount 🟦
- Not stock Trident
- Adds thermal expansion compliance
- Especially useful for high-temp builds

Decide early—affects assembly order.

---

# PHASE 4 – STEALTHBURNER / TOOLHEAD

**Manual reference**
- *“StealthBurner Toolhead”*

## 4.1 Expect Fitment Changes with Glass-Filled Filament 🟥
- Slightly oversized prints
- Fixes:
  - Reduce extrusion multiplier
  - Light sanding / filing

**Always dry-fit StealthBurner before final assembly**

---

## 4.2 LED Installation Order Matters 🟥
- LEDs must be installed sequentially
- Orientation is **not intuitive**
- Printed bridges must be clipped for wire routing

---

## 4.3 Toolhead PCB Notes (LDO) 🟦
- LDO PCB is adapted from Afterburner
- Wiring exits differ from stock StealthBurner
- Follow **LDO wiring diagrams**

---

## 4.4 Don’t Assume Symmetry 🟨
- Toolhead channels look mirrored
- Only one side is valid for wiring

---

# PHASE 5 – WIRING & CABLE CHAINS

**Manual reference**
- *“Wiring”*
- *“Cable Chains”*

## 5.1 Remove ALL Packaging Restraints 🟥
Before routing wires:
- Remove **all velcro**
- Remove **all zip ties**

Leaving them:
- Causes chain binding
- Fatigues wires
- Creates hidden strain points

---

## 5.2 Remove Cable Chain End Caps During Routing 🟨
- Prevents pinched wires
- Makes routing smoother
- Reinstall after cables are seated

---

## 5.3 Multi-Pin Connector Seating 🟥
- “Soft click” ≠ seated
- Visually inspect connector depth

---

## 5.4 Use Zip-Tie Anchors 🟨
- Strain relief near cable chain ends
- Prevents connector fatigue during motion

---

# PHASE 6 – ELECTRONICS & POWER

**Manual reference**
- *“Electronics Installation”*

## 6.1 Ground the Frame 🟥
- Do this **before first power-up**
- Prevents:
  - EMI issues
  - USB disconnects
  - Static buildup

---

## 6.2 Pi Power from Octopus (Optional) 🟨
- Clean wiring
- Fewer cables
- Requires correct jumper placement

---

# PHASE 7 – KLINNER, SCREEN & FIRMWARE

**Manual reference**
- *“Firmware Installation”*
- *“Initial Power-On”*

## 7.1 KlipperScreen Black Screen Fix 🟥
Symptom:
- Screen powers
- No UI
- No logs

Fix:
- Follow **KlipperScreen Troubleshooting → Virtual Console**
- Permission issue, not wiring

---

## 7.2 Screen Rotation (LDO) 🟥
- Use **LDO touchscreen docs**
- Edit `config.txt`
- Set correct overlay + invert flags

Generic Klipper docs are insufficient here.

---

## 7.3 First Klipper Error Is Normal 🟨
- Occurs before `printer.cfg` exists
- Not a wiring fault

---

# PHASE 8 – HIGH-TEMP & ADVANCED OPTIONS

## 8.1 PT100 vs PT1000 🟥
- **PT100 requires amplifier**
- **PT1000 works directly** on many boards

Verify before installing hotend.

---

## 8.2 High-Temp Builds Benefit From 🟦
- Kinematic bed mounts
- Extra toolhead wire slack
- Early strain relief planning

---

# SPECIAL TOOLS & FILES MENTIONED

## Tools
- Heat-set insert press (Naomi Wu / Atom style)
- Precision square (used mainly as flat reference)
- Side cutters (LED bridge removal)
- Tweezers (washers, inserts)
- Rubber mallet (gentle persuasion only)

## Files / Docs
- Voron Trident Assembly Manual
- LDO Trident Build Notes
- KlipperScreen Troubleshooting Page
- LDO Touchscreen Rotation Guide

---

# FINAL PRE-POWER CHECKLIST 🟥
- [ ] Frame square and flat
- [ ] All rails secured with end-stops
- [ ] Z nut bars installed
- [ ] Toolhead fully wired and strain-relieved
- [ ] Cable chains move freely
- [ ] Frame grounded
- [ ] Correct thermistor type installed
- [ ] No leftover “mystery” screws

---

## End of Checklist
