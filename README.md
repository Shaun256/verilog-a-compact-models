# Physics-Based Compact Models in Verilog-A

Coursework, EE5341 MOS Device Modelling & Characterisation, IIT Madras (Aug – Sep 2026)
Assignments 2 and 3 done with M Kalanidhi Maran and Sri Gayathri V.

| Model | Physics | Result | Report |
|---|---|---|---|
| Silicon resistor (intrinsic and n-doped) | n_i(T) from N_c, N_v, E_g; phonon-limited mobility μ ∝ T^-1.5 | Intrinsic: R falls ~5 orders of magnitude from 300 to 600 K. n-doped (N_D = 2×10¹⁷ cm⁻³): R rises from 115.7 to 327.4 Ω as mobility drops | [A1](Assgn_1.pdf) |
| Diode | Shockley equation | Full-wave bridge rectifier, 5 V / 50 Hz input: 3.7 V peak output after two diode drops | [A2](Assgn_2.pdf) |
| MOS capacitor | Surface potential solved by Newton–Raphson; quasi-static gate charge | LF and HF C-V across N_a = 10¹⁷–5×10¹⁸ cm⁻³ and t_ox = 5–15 nm; Debye-length extraction; V_FB = −1 V shift | [A3](Assgn_3.pdf) |

## Numerical note

The Newton–Raphson loop for the surface potential originally used a relative error, which diverges at flat band (ψ_s → 0). The final model uses an absolute error metric, which stays stable through V_gb = V_FB.

## Tools

Verilog-A · Qucs Studio
