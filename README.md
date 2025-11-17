# 🚀 High-Speed Gigabit Ethernet Interface

Welcome! This repository contains the complete hardware design files for a custom-built, 6-layer Gigabit Ethernet interface board.

The design is centered around the powerful **STM32F746NGH6** (an ARM Cortex-M7 MCU) and the **DP83867IR** Gigabit PHY. The entire layout was planned to meet strict high-speed design rules, featuring a robust multi-rail power supply and controlled impedance routing for 1Gbps performance.

## 🛠️ Key Features & Components

* **Brain (MCU):** `STM32F746NGH6` (ARM Cortex-M7)
* **Translator (PHY):** `DP83867IRPAPT` (10/100/1000 Mbps Gigabit PHY)
* **Data Interface:** `RGMII`
* **Port (Connector):** `ARJM11D7-502-AB-EW2` (A shielded Gigabit MagJack with integrated LEDs)
* **Power Supply:** 5V USB-C input, feeding a "power tree" of four independent LDOs for ultra-clean `+3.3V`, `+2.5V`, `+1.8V`, and `+1.1V` rails.
* **PCB:** Custom 6-layer, 80x50mm board with controlled impedance routing.
* **Debug:** Standard 10-pin ARM SWD (Serial Wire Debug) header.

## ✅ Hardware Project Status: Complete!

This repository covers the complete hardware design and manufacturing file generation. All phases of the hardware build are finished.

* ✅ **Phase 1: Component Selection**
    * *Selected and verified the core MCU, PHY, MagJack, and all power components for Gigabit-speed requirements.*
* ✅ **Phase 2: Schematic Design**
    * *Created the full electronic blueprint, connecting all components and defining all power and signal nets.*
* ✅ **Phase 3: Pre-Layout Checks**
    * *Ran a full Electrical Rules Check (ERC) and assigned all physical component footprints.*
* ✅ **Phase 4: PCB Layout**
    * *Designed the 6-layer stackup, floorplanned all components, poured all ground and power planes, and hand-routed all 17 critical high-speed differential and RGMII traces.*
* ✅ **Phase 5: Manufacturing File Generation**
    * *Generated the final Gerber and Drill files (`.zip`) required for fabrication.*
