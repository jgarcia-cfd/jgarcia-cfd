## Hi there 👋
# Justin Garcia | Mechanical Engineer
Mechanical Engineering student (B.S. graduating in May 2027) specializing in CFD/FEA workflows, thermal/fluid systems analysis, and turbomachinery design

---
## 🛠️ Tools and Technical Capabilities
* **CFD & Solvers:** ANSYS Fluent, ANSYS CFX ($k-\omega$ SST turbulence modeling), Grid Convergence Index (GCI) study
* **Geometry & Meshing:** Autodesk Inventor, Fluent Meshing (polyhexcore), SpaceClaim, Bladegen, Turbogrid (hexahedral)
* **Numerical Methods:** Python (Numpy, Scipy, Sympy, Matplotlib, Pandas), System Curve Modeling, 1-D Turbomachinery Meanline  Code
---

## **Featured Projects**

### 💨Design and Construction of a Subsonic Wind Tunnel (In-Progress)

**Overview:** Conducted a high-fidelity CFD analysis of subsonic wind tunnel to validate performance & accuracy prior to construction.
* **Workflow:** Inventor geometry $\rightarrow$ ANSYS Fluent CFD simulation $\rightarrow$ Microsoft Excel System Curve generation
* **Physics & Setup:** Transient $k-\omega$ SST turbulence modeling coupled with a 2-D fan zone to model geometry
   * **Boundary Conditions:** Modeled in an airtight room for initial expected deployment of physical tunnel, 2-D fan zone for driving flow, symmetry to model half of the tunnel
   * **Scheme and Solver:** 2nd-Order Upwind & SIMPLE algorithm
   * **GCI:** GCI was performed to validate mesh independence
* **Deliverables:** High-resolution computational domain, velocity contour plot, and system curve

 #### Visual Analysis
 <img width="928" height="357" alt="Mesh" src="https://github.com/user-attachments/assets/cc5bda80-469e-4fe7-afbb-1b1728cd229e" />
 
 * **Figure 1:** Internal volume mesh showing the refined mesh near walls
 
 <img width="928" height="357" alt="Velocity contour plot" src="https://github.com/user-attachments/assets/6820cd57-b9fa-4e74-8464-70eea24006b8" />
 
 * **Figure 2:** Velocity contour plot showing no flow recirculation inside the wind tunnel. Note: Modeled inside an airtight room, which accounts for the negative velocity shown.
 
 <img width="613" height="371" alt="System Curve for Subsonic Wind tunnel" src="https://github.com/user-attachments/assets/5fd57ec5-438e-4bb9-850c-1b59f4108249" />
 
 * **Figure 3:** System curve generated in Microsoft Excel from extracted pressure and velocity from ANSYS Fluent
