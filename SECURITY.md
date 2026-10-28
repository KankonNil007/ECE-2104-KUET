# Security and Safety Policy

## 🛡️ Supported Versions

As an academic laboratory project, this repository provides reference design files and documentation for the ECE 2104 course at KUET.

| Version / Branch | Supported | Notes |
|:---|:---:|:---|
| `main` | ✅ | Active reference release |
| Prior commits | ❌ | Historical lab drafts |

---

## ⚠️ Electrical & Laboratory Safety Guidelines

When replicating or testing the hardware circuit on a physical breadboard, adhere to standard electrical laboratory safety practices:

1. **Power Supply Ratings & Isolation:**
   - Ensure the DC power supplies are set strictly to their specified levels (**4.0 V** for logic ICs `74HC161` & `7408`, **9.0 V** for `LM358` / `LM393`, and **0–8.0 V** variable for $V_{in}$).
   - Exceeding the absolute maximum ratings ($V_{CC} > 6.0\text{ V}$ on $74\text{HC}$ series logic) will cause irreversible IC damage or overheating.
2. **Current Limiting:**
   - Always verify current-limiting resistors ($330\ \Omega$) are connected in series with all LED indicators to prevent excess current draw and damage to the counter output stages.
3. **Common Ground Connection:**
   - Maintain a unified common ground across all power supply channels, function generator, and oscilloscope/multimeter probes to avoid floating potentials and inaccurate threshold comparisons.
4. **Wiring Inspection:**
   - Always double-check connections prior to powering on the DC supply to prevent direct $V_{CC}$-to-GND short circuits on breadboard bus rails.

---

## 🔒 Reporting a Vulnerability or Issue

If you discover any security, calculation, or safety discrepancy in the design:

1. **Do not create a public issue** if it involves confidential institutional lab test data.
2. Reach out directly to the project maintainers:
   - **Kankon Mondal** & **Mst. Naznin Aktar**
   - Department of Electronics and Communication Engineering (ECE)
   - Khulna University of Engineering & Technology (KUET)
3. Include:
   - Description of the issue or calculation error
   - Steps or schematic modifications to reproduce
   - Potential impact on hardware or measurement accuracy

We will review reports promptly and publish corrective updates to the repository.

