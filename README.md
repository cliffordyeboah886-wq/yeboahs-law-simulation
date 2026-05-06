# ⚠️ DEPRECATED / ARCHIVED
This repository is part of the early development phase of Yeboah's Law. 
It is no longer maintained. 

**Please visit the latest version here:** 
👉 [Yeboah’s Law Digital Twin v2.0](https://cliffordyeboah886-wq.github.io/yeboahs-law-digital-twin/)
---
# yeboahs-law-simulation
Interactive simulation of Yeboah's Law of Cutting Efficiency

# Yeboah's Law of Cutting Efficiency - Interactive Simulation

Welcome to the interactive simulation for **Yeboah's Law of Cutting Efficiency**. This repository hosts a web-based thermodynamic and kinetic calculator designed to model the mechanics of material severance during dynamic impact.

You can access the live interactive simulation here: 
👉 **[https://cliffordyeboah886-wq.github.io/yeboahs-law-simulation/]**

---

## 🔬 The Physics Behind the Simulation

At its core, material cutting via impact is a battle between the **kinetic energy** of the striking tool and the **mechanical resistance** of the target material. Yeboah's Law of Cutting Efficiency mathematically models this interaction to determine whether a strike will result in total severance or if the tool will be arrested by the material.

The governing equation is defined as:

$$
\eta = k_Y \left( \frac{m v^2}{2 d \tau A} \right)
$$

### Variable Breakdown:
*   **\(\eta\)** (Eta): The Cutting Efficiency Ratio (dimensionless).
*   **\(k_Y\)**: The Yeboah Constant / Energy Recovery Factor (\(0 < k_Y \le 1\)).
*   **\(m\)**: Mass of the cutting tool (kg).
*   **\(v\)**: Impact velocity of the cutting tool (m/s).
*   **\(d\)**: Depth or thickness of the target material (m).
*   **\(\tau\)** (Tau): Shear resistance of the material (Pa or N/m²).
*   **\(A\)**: Contact area between the tool edge and the material (m²).

---

## ⚙️ Understanding the Mechanics

The equation elegantly balances two opposing forces:

**1. The Kinetic Driver (Numerator: \(m v^2\))**
This represents the driving force of the tool, derived from the standard kinetic energy formula (\(E_k = \frac{1}{2}mv^2\)). Velocity is squared, meaning that a faster strike contributes exponentially more to cutting potential than simply using a heavier tool.

**2. The Material Resistance (Denominator: \(2 d \tau A\))**
This represents the total work required to force the tool through the material. It accounts for the material's inherent shear strength (\(\tau\)), the thickness that must be penetrated (\(d\)), and the surface area of the blade's edge (\(A\)). A sharper blade (smaller \(A\)) drastically reduces the resistance.

**3. The Yeboah Constant (\(k_Y\))**
In a perfect, frictionless vacuum, all kinetic energy would transfer directly into severing the material. However, in the real world, energy is lost upon impact due to:
*   Acoustic dispersion (sound)
*   Thermal dissipation (heat)
*   Plastic deformation of the tool or surrounding material

The **Yeboah Constant (\(k_Y\))** acts as the *Energy Recovery Factor*, scaling the theoretical efficiency down to account for these stochastic thermodynamic losses. 

---

## 📊 Interpreting the Results

The simulation calculates the Efficiency Ratio (\(\eta\)) in real-time as you adjust the kinetic and material variables.

*   **Severance (\(\eta \ge 1\)):** The kinetic energy, even after real-world losses, successfully overcomes the material's shear resistance. The target is cut.
*   **Arrested (\(\eta < 1\)):** The material's resistance absorbs the kinetic energy before the tool can pass completely through. The cut fails or gets stuck.

---

## 🛠️ How to Use the Simulator
1. Open the [live simulation link].
2. Adjust the **Kinetic Input** sliders (Mass, Velocity) to simulate the tool's strike.
3. Adjust the **Energy Recovery** slider (\(k_Y\)) to simulate the efficiency of the impact.
4. Adjust the **Material Resistance** sliders (Shear Resistance, Area, Thickness) to define the target.
5. Watch the gauge update in real-time to see if your parameters result in a successful cut!
