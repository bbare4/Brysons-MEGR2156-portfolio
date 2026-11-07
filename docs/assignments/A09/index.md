# Assignment 9
<h3 align="center">A9 – Pulley Design</h3>

The purpose of this assignment is to design a pulley system that transfers power between two parallel shafts. The system must use two 3-inch pulleys spaced 4–6 inches apart, operate at 1,000–2,000 rpm, and have a stationary belt tension of 4–6 lbf with a minimum safety factor of 3. The project includes selecting a polyurethane belt, sizing the shafts, choosing journal bearings, and designing a supporting frame. Calculations, sketches, and lessons learned will document the design process.

For my design, I selected steel pulleys with a specified yield strength of 100,000 psi. Both pulleys have a diameter of 3 inches and are positioned 5 inches apart, measured from center to center. I chose an operating speed of 1,000 rpm, a stationary belt tension of 5 lbf, and a design safety factor of 3. These choices meet the assignment’s requirements and provide the starting values for designing the system.

<h3 align="center">Belt Design</h3>

The calculations below resulted in a minimum belt diameter of approximately 9/32 inch. Since this size was not available among the belt options, I selected a 5/16-inch polyurethane belt. This larger diameter exceeds the calculated minimum and provides additional cross-sectional area, reducing tensile stress under the same load and providing an extra margin above the required safety factor of 3.

<img width="772" height="990" alt="image" src="https://github.com/user-attachments/assets/2a8c6020-a32a-41be-9a01-a8d56b5cc85a" />

<h3 align="center">Shaft Design</h3>

The goal of the shaft design is to determine the minimum diameter needed to transmit torque through the pulley system without exceeding the material’s allowable shear stress. The shafts are made from 1060 hardened steel, and my calculations use the applied torque, material strength, and a safety factor of 3. These calculations resulted in a minimum shaft diameter of 0.128 inch. A shaft size at or above this value will be selected to satisfy the calculated torsional strength requirement.

<img width="770" height="727" alt="image" src="https://github.com/user-attachments/assets/c4343721-4f83-4cea-8257-fcf8adc73a3f" />

<h3 align="center">Journal Design</h3>

The next step was to select the journal bearings and a suitable bearing material. I calculated the bearing pressure, shaft surface velocity, and resulting PV value, then compared these values with the material limits in the reference chart. Based on my calculations, I selected dry graphite because its allowable pressure, velocity, and PV limits accommodate the calculated operating conditions of my pulley system.

<img width="761" height="849" alt="image" src="https://github.com/user-attachments/assets/1c1e9c2c-ece3-4284-ac4a-340fbf043ce4" />

<img width="1243" height="840" alt="image" src="https://github.com/user-attachments/assets/21447826-3fc5-4ab8-92fb-f22c71465247" />

<h3 align="center">Frame Design</h3>

For my frame design, I chose a simple rectangular frame to provide mounting locations for the shaft bearings and maintain the required 5-inch spacing between the pulley centers.

<img width="1017" height="986" alt="image" src="https://github.com/user-attachments/assets/69b385a5-579b-4a0d-a9ec-38585708df07" />

I selected aluminum alloy for the pulley frame based on the Ashby plot. I chose aluminum because it balances strength and low weight, making it suitable for supporting the pulley system without adding unnecessary mass.

<img width="480" height="609" alt="image" src="https://github.com/user-attachments/assets/0041b624-b4bf-4ab2-9901-0d919efd28f3" />

<h3 align="center">Lesson Learned</h3>

In this assignment, I learned how pulleys use belt tension and friction to transfer power and how material choices affect how well the system works. Unsuitable materials can cause parts to bend, wear out, or fail. I also learned that understanding the system’s purpose, speed, and load helps guide the selection of materials and sizes so it works as intended. Our calculations assumed the belt would not slip, but a real design would require checking this because slipping can reduce power transfer and wear out the belt.

This assignment took me 2.5 hours to complete.




















