# Physics-Based Compact Models in Verilog-A

Coursework, EE5341 MOS Device Modelling, IIT Madras (Aug – Oct 2026)

📄 **[Read the full report (PDF)](report.pdf)**

Physics-based Verilog-A models written from first principles and simulated in Qucs Studio.

## Models

| Model | Physics included | Validation |
|---|---|---|
| Silicon resistor | Temperature-dependent mobility and resistivity | R(T) against analytical expression |
| Diode | Shockley equation with series resistance | Used in a full-wave bridge rectifier |
| MOS capacitor | Depletion, inversion, flat-band shift | High- and low-frequency C-V; Debye length against theory |

## MOS capacitor sweeps

- Substrate doping: 10¹⁷ – 5×10¹⁸ cm⁻³
- Oxide thickness: 5 – 15 nm
- Flat-band voltage shift modelled; extrinsic Debye length checked against the analytical value

## Tools

Verilog-A · Qucs Studio
