## Hi there 👋
# Justin Garcia
**Undergraduate Mechanical Engineering Student** | Abilene Christian University (B.S. Expected May 2027)
*Focusing on Thermal/Fluid Systems, Turbomachinery Meanline Analysis, and Computational Fluid Dynamics (CFD)*

---

## 🎯 Profile & Research Interests
I am an undergraduate engineering student passionate about aerothermodynamics and turbomachinery systems (specifically axial/radial compressors and high-pressure turbopumps). Driven by a desire to pursue SME-level expertise in CFD, I actively design and build complex computational workflows, fluid systems, and educational frameworks alongside my formal coursework.

**Current Endeavors:**
- **Undergraduate Thesis:** Designing and building a low-cost subsonic wind tunnel for ACU's emerging aerospace concentration.
- **Self-Directed Propulsion Initiative:** Initiated and leading a multi-student team project to build a comprehensive 1D thermodynamic-to-3D CFD educational workflow manual and demonstration suite for a 2-spool turbofan engine across all major components.
- **Academic Dissemination:** Preparing abstracts for submission to AIAA and ASEE calls for papers.

---

## 🛠️ Skills & Technical Tools (In Active Development)

- **CFD & Reaction Solvers:** ANSYS Fluent, ANSYS CFX ($k-\omega$ SST & Realizable $k-\epsilon$), Chemkin Kinetics Integration, Grid Convergence Index (GCI) verification
- **Turbomachinery & Geometry:** ANSYS Vista AFD, BladeGen, TurboGrid (Hexahedral meshing $y^+ \approx 1$), SpaceClaim, Autodesk Inventor
- **Numerical Methods & Cycle Analysis:** Python (`NumPy`, `SciPy`, `CoolProp`, `Matplotlib`, `Pandas`), 1D Meanline Code Development, Thermodynamic Cycle Modeling

---

## 🚀 Featured Projects

### 1. 2-Spool Turbofan Engine: Modular 1D Cycle & 3D CFD Workflow Framework (In Progress)
**Role:** Project Architect, Team Lead, & Compressor Specialist (Self-Directed Initiative)

* **Overview:** Conceived and organized an unprompted, student-led project to create a repeatable, high-fidelity CFD workflow manual and parameterized benchmark suite for gas turbine components within the ANSYS software ecosystem. Recruited and delegated components across a team of peers to expand the scope from a single compressor stage into a full-engine demonstration suite (Fan, LPC, HPC, LPT, HPT, Diffuser, Combustor, Nozzle).
* **Scope & Methodology:**
  * **1D Thermodynamics:** Developed a Python + `CoolProp` script (piece-wise calorically perfect gas model) to establish the single source of truth for engine station pressures ($P_0$), temperatures ($T_0$), and mass flow rates ($\dot{m}$) at Mach 0.85 / 30,000 ft cruise.
  * **Meanline & Geometry:** Derived non-dimensional stage loading ($\psi$), flow coefficient ($\phi$), reaction ($R$), and meanline velocity triangles to initialize 3D blade profiles via Vista AFD and BladeGen.
  * **Rotating Machinery Pipeline:** Designed the **Vista AFD $\rightarrow$ BladeGen $\rightarrow$ TurboGrid $\rightarrow$ ANSYS CFX** pipeline using structured hexahedral meshes ($y^+ \approx 1$) and $k-\omega$ SST closure to model representative single stages with steady-state Stage/Mixing Plane interfaces.
  * **Combustion & Ducts:** Integrated 3D combustor sector models in ANSYS Fluent with imported Chemkin finite-rate kinetics to map thermal fields, Pattern Factor ($PF$), and $NO_x/CO$ emissions.
* **Key Deliverables:** Step-by-step tutorial manual, parameterized Workbench templates (`.wbpz`), automated performance map generation (${\pi}_{tt}$ and $\eta_{is}$ vs. $\dot{m}_{corr}$), and cross-verification of 1D design targets against 3D CFD diagnostics.

---

### 2. Design, Analysis, and Construction of a Subsonic Wind Tunnel (In Progress)
**Role:** Lead Researcher (Undergraduate Thesis)

* **Overview:** Conducted high-fidelity CFD simulations to evaluate flow quality, wall interference, and pressure losses for a newly commissioned open-circuit subsonic wind tunnel designed for ACU's aerospace track.
* **Numerical Methods & Setup:**
  * **Domain & Physics:** Modeled the complete internal domain within an enclosed room environment; applied 2D fan zone representations and 3D symmetry planes to optimize computational resources.
  * **Solver Configuration:** Steady/transient incompressible solver, 2nd-Order Upwind discretization with SIMPLE pressure-velocity coupling, $k-\omega$ SST turbulence closure.
  * **Verification:** Conducted a Grid Convergence Index (GCI) study based on Roache's methodology to verify spatial mesh independence.
* **Key Deliverables:** Verified core flow acceleration with zero internal separation, extracted pressure drop data to generate system curves in Excel/Python for physical fan selection, and compiled construction specs.

#### Visual Analysis

<img width="928" alt="Wind Tunnel Mesh" src="https://github.com/user-attachments/assets/cc5bda80-469e-4fe7-afbb-1b1728cd229e" />

* **Figure 1:** Computational domain featuring boundary layer refinement along wall bounds.

<img width="928" height="357" alt="Velocity contour plot" src="https://github.com/user-attachments/assets/6820cd57-b9fa-4e74-8464-70eea24006b8" />

* **Figure 2:** Mid-plane velocity contours showing uniform core flow acceleration in the test section.

<img width="613" alt="System Curve" src="https://github.com/user-attachments/assets/5fd57ec5-438e-4bb9-850c-1b59f4108249" />

* **Figure 3:** System loss curve generated from extracted CFD static and total pressure differentials.
