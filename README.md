# Fractal 5 Pro

The Fractal 5 Pro is an open source intuitive benchtop multidirectional 5-axis 3D printer.

A user-friendly 5-Axis slicer application was developed to go along with this printer. **You can download it for free here**. 💻

<p align="center">
  <img src="./CAD/images/Fractal_5_Pro_ISO.PNG" width="500">
</p>

# Project Motivation
This project was motivated by the **Fractal Robotics** vision: **To accelerate the development of mechanical solutions.** In support of this vision, this printer aims to address the gap between the limitations of 3-axis FDM and the inaccessibility of current 5-axis FDM 3D printers.

**📋Limitations of 3-Axis 3D Printers**
  - Part strength is limited due to the direction of printing
    - Parts often fail when forces are applied parallel to the direction of layer lines
    - Stacking layers in only one direction limits design freedom
  - Overhangs require support structures
    - The process of removing supports often damages or destroys a part
    - Support structures waste material

**🔒Inaccessibility of Existing 5-Axis 3D Printers**
  - No commercially available intuitive slicer applications
    - Non-planar slicing requires significant training on advanced CAM softwares
  - Commercially available 5-Axis 3D printers are huge and expensive

---

# 🔎Product-Market Fit
Dozens of potential customers were interviewed to determine 3D printing needs, budgets, and expectations across different industries. This process helped inform and focus design decisions.

**🔑Key Customer Needs Translated to Design Decisions**

Our response to the customer interviews was to design an accessible product that addressed the shortfalls of 3-axis FDM while still being easy to use.

  - Control over orthotropic strength, less waste material, reduced post-processing risk ➡️ 5-Axis
  - Ease of maintenance, clean setup ➡️ FDM, removable build surface, full-size front and side doors
  - Reduced training time ➡️ Intuitive multidirectional slicer software, backwards compatibility with 3-Axis 3D printing
  - Printing complex parts ➡️ Compatible with any 3D geometry
  - High reliability ➡️ CoreXY gantry, auto bed leveling, rigid 30x30mm aluminum frame extrusions
  - Expansive material compatibility ➡️ Direct Drive Extruder, heated build plate, fully enclosed
  - Large print volume ➡️ 300mm Diameter x 250mm build height

---

# FAQ's

**What does this printer do that others can't?**
- It provides all of the following in one product: high reliability, stronger parts, more design freedom, less waste material, large build volume, intuitive user experience, and ease of maintenance at a relatively affordable price.

**Why FDM? Why not SLA or SLS?**
- FDM printers are low maintenance, have an easy & clean setup, and are compatible with a large selection of affordable materials. Further, since FDM is the printing method that is most effected by orthotropy, it stands to benefit the most from 5-axis technology.

**Why Direct Drive instead of Remote Drive?**
- The customers interviewed tend to favor printers that are compatible with a wide selection of feedstock materials, including softer filaments. TPU needs direct drive to print effectively since it's so soft. Using remote drive to extrude soft filaments would be like pushing on the end of a string to get the far end to move, which doesn't work very well.

**How is the print bed heated if it can spin infinitely? Wouldn't the wires get twisted up?**
- We use a high current slip-ring to transfer power to the rotating shaft.

**What is multidirectional 5-axis 3D printing?**
- ...

**Why choose multidirectional slicing instead of non-planar printing?**
- Non-planar slicing requires significant training in advanced CAM softwares while multidirectional printing provides almost all the benefits of 5-axis 3D printing in a more accessable and familiar platform. Further, multidirectional 5-Axis does not require the printhead to be long and thin to achieve tight angles, so the printhead can achieve much higher print speeds with far less vibration than existing 5-axis 3D printers.

---

# 📝Future Work
- Redesign print bed gimbal for higher rigidity
  - Use 1/4" thick aluminum sheets instead of 1/8"
  - Rearrange A-Axis bearing assembly to minimize unsupported shaft length
  - Incorporate larger corner gussets
- Change A-axis pulley drive to a high ratio gear drive
- Convert cable-chain wire harness system to CAN-bus
- Integrate accelerometer into printhead for input shaping (resonance cancellation)
- Instead of using the inductive probe for centering the print bed, use a sensor that has better defined sensing radii in the X and Y directions
  - The same centering routine can be used, but a different sensor solution is needed
