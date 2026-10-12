## Hi there 👋
# Justin Garcia
**Undergraduate Mechanical Engineering Student** | Abilene Christian University (B.S. Expected May 2027)
*Focusing on Thermal/Fluid Systems, Turbomachinery Meanline Analysis, and Computational Fluid Dynamics (CFD)*

---

## 🎯 Profile & Research Interests
I am an undergraduate engineering student passionate about aerothermodynamics and turbomachinery systems (specifically axial/radial compressors and high-pressure turbopumps). Driven by a desire to pursue SME-level expertise in turbomachinery and CFD, I actively design and build complex computational workflows, fluid systems, and educational frameworks alongside my formal coursework.

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

### 1. Subsonic 2-Spool Turbofan: Modular 1D Cycle & 3D CFD Workflow Framework (In Progress)
**Role:** System Architect, Project Lead, & Technical Authority (Self-Directed Initiative)

- **Overview:** Conceiving, architecting, and directing a student-led initiative to build a repeatable, high-fidelity CFD workflow manual and parameterized benchmark suite for gas turbine components within the ANSYS software ecosystem. Designing the end-to-end multi-pipeline system architecture (CFX rotating turbomachinery, Fluent static ducts, and Fluent/Chemkin combustion) and leading a 4-person team executing parallel component demonstrations across representative Fan, Compressor, Turbine, Duct, and Combustor modules. Serving as the lead technical authority with final sign-off authority on all mesh quality gates, solver convergence parameters, and project deliverables.
- **Scope & System Architecture:**
  * **System Architecture & 1D Cycle:** Authoring the master Python + `CoolProp` thermodynamic cycle script (piece-wise calorically perfect gas model) to establish engine station boundary conditions ($P_0, T_0, \dot{m}$ at Mach 0.85 / 30,000 ft) and designing standardized Workbench master templates (`.wbpz`) for automated performance mapping and parameter sweeps.
  * **Module A Pipeline (Rotating Machinery):** Establishing the **Vista AFD → BladeGen → TurboGrid → ANSYS CFX** standard ($y^+ \le 1$, $k-\omega\text{ SST}$, mixing planes) executed across representative Fan, Core Compressor, and Turbine stages.
  * **Module B Pipeline (Static Ducts):** Establishing the **Inventor → SpaceClaim → Fluent Meshing → ANSYS Fluent** standard ($y^+ \le 1$, $k-\omega\text{ SST}$) executed for intake diffuser and exhaust nozzle geometries.
  * **Module C Pipeline (Combustion):** Co-leading the 3D combustor sector setup in ANSYS Fluent integrated with imported Chemkin finite-rate kinetics (Realizable $k-\epsilon$, $y^+ \approx 30\text{--}100$) utilizing Volumetric Reactions to evaluate flame anchoring, primary recirculation zones, and exit thermal profiles.
- **Target Deliverables:** Authoring and editing the comprehensive student-facing ANSYS Turbomachinery & Combustion Workflow Manual, enforcing quality control across component convergence logs, generating automated component performance maps ($\pi_{tt}, \eta_{is}$ vs. $\dot{m}_{corr}$), and conducting side-by-side verification of 1D design targets against 3D CFD diagnostics.

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
