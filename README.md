# Fractal 5 Pro

The Fractal 5 Pro is an intuitive benchtop multidirectional 5-axis 3D printer designed for professional use.

This machine was designed in support of the Fractal Robotics vision: **To accelerate the development of mechanical solutions.** This printer aims to address the gap between the limitations of 3-axis FDM 3D printing and the accessibility of current 5-axis FDM 3D printing solutions.

<p align="center">
  <img src="./CAD/images/Fractal_5_Pro_ISO.PNG" width="500">
</p>

---

**🔎Market Gap:**

**-📋Limitations of 3-Axis 3D Printers**
    - Part strength is limited due to the direction of printing
      - Parts tend to fail when forces are applied along the direction of layer lines
      - Only being able to stack layers along one direction limits design freedom
    - Overhangs require support structures
      - The process of removing supports often damages or destroys a part
      - Support structures waste material

**-🔒Inaccessibility of Existing 5-Axis 3D Printers**
    - No intuitive software available for non-planar printing
    - Commercially available printers are huge and expensive

---

**⚙️Design Features**
- CoreXY Gantry (high reliability)
- Direct Drive Extruder  
- Fully Enclosed
- Rigid 30x30mm aluminum frame extrusions
- Triple Lead-Screw Z Axis  
- Dual Rotary Axis Printing Bed  
  - 300mm Diameter x 250mm Build Height  
  - Heated build plate up to 100°C  
  - Infinite spin rotation about A-Axis  
  - 0°–90° tilt rotation about B-Axis  
  - Removable textured spring-steel build surface
- Compatible with Klipper Firmware
- Backwards compatible with 3-Axis 3D printing

---

**📝Future Work**
- Redesign print bed gimbal for higher rigidity
  - Use 1/4" thick aluminum sheets instead of 1/8"
  - Rearrange A-Axis bearing assembly to minimize unsupported shaft length
  - Incorporate larger corner gussets
- Change A-axis pulley drive to a high ratio gear drive
- Convert cable-chain wire harness system to CAN-bus
- Integrate accelerometer into printhead for input shaping (resonance cancellation)
- Instead of using the inductive probe for centering the print bed, use a sensor that has better defined sensing radii in the X and Y directions
  - The same centering routine can be used, but a different sensor solution is needed
