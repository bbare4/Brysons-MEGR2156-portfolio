# A11 – Motor Selection

This project focuses on designing the motorized drive and support structure for a benchtop tensile tester with a 2 kN load capacity. The tester uses two lead screws to move a crosshead and pull a test specimen. By applying tension, the machine can help show how a material responds to load and how much it stretches before it yields or breaks.

Our team will select a motor, design motor mounts, choose or design a coupler, and develop a stable frame and specimen clamps. The design must support the required load with a safety factor of 4, keep the specimen and crosshead aligned, and fit within a practical bench-top size. The lead screw system must also meet the required travel-speed range of 1–50 mm/min and have a minimum lead screw length of 18 inches.

The final work will include CAD models of the engineered parts, supporting sketches and free-body diagrams, design calculations, and a bill of materials with estimated costs. This assignment documents the design process as well as the final design, including decisions, mistakes, and lessons learned.

<img width="352" height="452" alt="image" src="https://github.com/user-attachments/assets/32f8cb7b-e6f8-40a3-a5d7-6e4c7517d258" />

## Motor Selection and Attachments -  (Bryson Bare)

We selected the MOONS’ AM34HD2403-07 hybrid stepper motor because the tester must move slowly while pulling a high load. The stepper motor can provide controlled movement at low speeds, and this model has a listed holding torque of 9.4 N · m. We assumed that one motor would drive each lead screw, so each screw carries half of the tester's 2 kN load. The holding torque helped us identify a candidate, but we use the speed-torque curve to check the torque while the motor is running.

