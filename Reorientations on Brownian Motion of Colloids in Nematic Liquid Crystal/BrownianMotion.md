# 1. Brownian motion 
Random displacements of a small particlein a fluid are controlled by kinetic energydissipation (1). The mean displacement iszero but the average mean squared displacement(MSD) is finite, growing linearly with time lag $\tau$

## Reference
[Effect of Collective MolecularReorientations on Brownian Motion ofColloids in Nematic Liquid Crystal](https://www.science.org/doi/epdf/10.1126/science.1240591)

## 1.1 Theory and Concept:

### 1. Basic Brownian Motion:
- A particle suspended in a fluid, due to the constant bombardment by fluid molecules, undergoes random motion known as **Brownian motion**.
- The average movement or displacement (`Δr`) over time is zero (since the motion is random). But the **mean squared displacement (MSD)** isn't. It grows linearly with the time lag `τ`.

### 2. Diffusion Coefficient:

The self-diffusion coefficient (`D`) of a random walker in a fluid is described by the **Stokes-Einstein relation**. It is given by:

$$D = \frac{k_B T}{6 \pi \eta R}$$

Where:
- $k_B$ is the Boltzmann constant.
- $T$ is the temperature.
- $\eta$ is the viscosity of the fluid.
- $R$ is the radius of the random walker (or particle).

This relation arises from the balance between the thermal energy (given by $k_B T$) and the viscous drag (related to $\eta$ and $R$) that the particle experiences in the fluid.

- The equation `⟨Δr^2(τ)⟩ = 6Dτ` relates the mean squared displacement with the time lag using the **diffusion coefficient `D`**.
- `D` gives a measure of how quickly a particle spreads out in the fluid. 


### 3. Anomalous Behavior:
- In some fluids, the growth isn't linear. This deviation is termed as **"anomalous behavior"**.
- When `α < 1`, it's called **subdiffusion**. This is observed in polymer networks, F-actin networks, and surfactant dispersions.
- When `α > 1`, it's called **superdiffusion**. Seen in concentrated bacterial suspensions and polymer-like micelles.

### 4. Orientational Order & Nematic Fluids:
- Some fluids have molecules with a predominant orientation, described using a **"director"**. 
- A **uniaxial nematic fluid** is a simple fluid where molecules have a dominant orientation.
- Different viscosities for motions parallel and perpendicular to the director make the diffusion **anisotropic**, resulting in different diffusion coefficients `D_||` and `D_⊥`.
### 5. Anisotropic Diffusion:
- **Definition:** Diffusion that differs in different directions.
- **Context:** In this study, diffusion is anisotropic in the nematic phase due to the alignment of molecules.

### 6. Velocity Auto-Correlation Function (VACF):
- **Definition:** Represents how the velocity of a particle at one time is related to its velocity at another time.
- **Interpretation:** If VACF is close to zero, it signals normal diffusion. Positive and negative values indicate superdiffusion and subdiffusion, respectively.
### 7.Nematic Liquid Crystals:
- **Definition:** A type of liquid crystal where molecules align in parallel but are not arranged in well-defined planes.
- **Anchoring:** Determines how molecules near the boundary align relative to the boundary. Types:
  - **Perpendicular:** Molecules align perpendicular to the surface.
  - **Tangential:** Molecules align tangentially to the surface.

  
## 1.2 Data, Equations, and Properties in [Paper](https://www.science.org/doi/10.1126/science.1240591):
[Effect of Collective MolecularReorientations on Brownian Motion ofColloids in Nematic Liquid Crystal](https://www.science.org/doi/epdf/10.1126/science.1240591)

![MSDs and velocity autocorrelation functions of 5-μm silica spheres in IS-8200.](https://github.com/wentaogong111/SoftMatterPhysics_assignments/blob/main/Reorientations%20on%20Brownian%20Motion%20of%20Colloids%20in%20Nematic%20Liquid%20Crystal/Code/342_1351_f2.jpeg)
### 1. Diffusion Coefficient and MSD:
- `⟨Δr^2(τ)⟩ = 6Dτ`

### 2. Anomalous Behavior Equation:
- `⟨Δr^2(τ)⟩ ∝ τ^α`

---


### 3. Measured MSD Values: 
- **Isotropic phase (at 60°C):** Diffusion coefficient 
$$
D = 9.2 \times 10^{-16} m^2/s
$$.
- **Nematic phase (at 50°C):**
  - **Perpendicular anchoring:** $$ D_{||} = 1.9 \times 10^{-16} m^2/s$$ and $$ D_{⊥} = 1.4 \times 10^{-16} m^2/s$$.
  - **Tangential anchoring:** $$ D_{||} = 2.2 \times 10^{-16} m^2/s $$ and $$ D_{⊥} = 1.3 \times 10^{-16} m^2/s $$.

### 4. Equations:
- **velocity autocorrelation functions :**
  - $$ C_{v_{||}}(t) = \langle v_x(t) v_x(0) \rangle$$
  - $$ C_{v_{⊥}}(t) = \langle v_y(t) v_y(0) \rangle$$


### 5. Power Law Representation of MSD:
- Oversimplified model for understanding anomalous diffusion.
- **Equation:** $$MSD \propto t^a $$.
- **Determined values:** For subdiffusive domain:
  -  $a_{||} = 0.35 \pm 0.01 $ and $a_{⊥} = 0.30 \pm 0.01$.
  - For superdiffusion: $a_{||} = 1.32 \pm 0.01$ and $a_{⊥} = 1.20 \pm 0.01$.
  
### 6. Probability Distribution of Particle Displacements:
- Varies with time lags. 
- **Normal Diffusion:** Coincides with a Gaussian fit at long time lags (e.g., 40s).
- **Subdiffusion:** Central portion (small displacements) is Gaussian at intermediate time lags (e.g., 10s), but large displacements are less likely.
- **Superdiffusion:** Large displacements more probable than in normal diffusion at short time lags (e.g., 1s).

## 1.3 Case study

![1. Brownian motion simulation in an](https://github.com/wentaogong111/SoftMatterPhysics_assignments/blob/main/Reorientations%20on%20Brownian%20Motion%20of%20Colloids%20in%20Nematic%20Liquid%20Crystal/Code/brownian_motion.gif)

![Analysis:MSD, velocity autocorrelation functions, Anisotropic Diffusion](https://github.com/wentaogong111/SoftMatterPhysics_assignments/blob/main/Reorientations%20on%20Brownian%20Motion%20of%20Colloids%20in%20Nematic%20Liquid%20Crystal/Code/brownian_motion_plots.png)

### Further study
[Colloidal matter: Packing, geometry, and entropy](https://www.science.org/doi/epdf/10.1126/science.1253751)

[Command of active matter by topological defects and patterns](https://www.science.org/doi/full/10.1126/science.aah6936)
[Directional self-locomotion of active droplets enabled by nematic environment](https://www.nature.com/articles/s41567-020-01055-5)

[Mean first-passage times of non-Markovian random walkers in confinement](https://www.nature.com/articles/nature18272)

[Chiral liquid crystal colloids](https://www.nature.com/articles/nmat5032)

[Control of colloidal placement by modulated molecular orientation in nematic cells](https://www.science.org/doi/full/10.1126/sciadv.1600932)