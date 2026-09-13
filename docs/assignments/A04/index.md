# A4 – Motor Mount

## Description

Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) HERE which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations) Follow Appendix B for the initial approach to set up the design analysis.

<img width="566" height="219" alt="image" src="https://github.com/user-attachments/assets/0a8541c0-3e57-4025-8334-be97937f6ac9" />

Appendix A: 

<img width="1384" height="517" alt="image" src="https://github.com/user-attachments/assets/b521b1bf-1e16-48b8-8470-7c60e1349097" />

Appendix B: 

<img width="367" height="650" alt="image" src="https://github.com/user-attachments/assets/7b5d0b09-9b5e-4349-9e27-30eb6c51e8ee" />

## Feature 1:

The first step in designing Feature 1 was to determine the minimum height needed to safely support the applied load without exceeding material stress or the maximum allowable deflection. I began by creating a FBD to isolate Feature 1 and determine the forces acting on it so I could calculate the moment. The applied load was 300 N, and I selected a width of 40 mm for Feature 1. The mount material is ABS, with an elastic modulus of approximately 2,000 N/mm^2. A safety factor of 3 was required for the stress calculation, and the maximum allowable deflection was 0.30mm. I then calculated the moment, which gave me a value of 5400 N*mm. The main unknown was the height. I then created known and unknown columns to organize the known information before calculating the unknowns, so I could clearly identify the dimension that needed to be solved.

<img width="2752" height="1832" alt="IMG_0075" src="https://github.com/user-attachments/assets/f8a14d0d-9a4f-4042-9321-b514bee42fcf" />

With all the known and unknown values, I used the bending stress and deflection equations to solve for the required feature height. I started by solving both equations symbolically so I could easily plug in the numbers. Once I set up the height equations, I substituted my known values and solved for height. After finding both stress and deflection, I compared them and selected the larger value to ensure the feature met both the stress and deflection requirements.

<img width="2752" height="1848" alt="IMG_0076" src="https://github.com/user-attachments/assets/d42ef238-1865-451b-bb1e-dee0a5c45f9d" />

## Feature 2

For feature 2, I first created a free-body diagram and listed all my known and unknown values. Before solving for the required height, I needed to determine the feature's overall length and maximum bending moment. Using the 80 mm plate length and the 13 mm height from feature 1, I found the overall length to be L2 = 93 mm. I then used the applied force of 300 N and the distance from the fixed end to calculate the maximum bending moment, M = 33,300 N/mm. 

<img width="2752" height="1662" alt="IMG_0077" src="https://github.com/user-attachments/assets/91a6d94e-8814-412b-9711-dc3a39a72ebd" />

After finding these values, I used the bending stress and deflection equations to solve for the required height, h2. The next thing that I did was compare the two calculated heights and use the larger values so feature 2 meets both the stress and deflection requirements.

<img width="2752" height="1832" alt="IMG_0078" src="https://github.com/user-attachments/assets/4030bfb5-1c58-4841-a804-8877aa60ea6f" />

## Motor Mount Sketch

<img width="2752" height="1356" alt="IMG_0079" src="https://github.com/user-attachments/assets/791ce275-1d6a-45c5-8173-714c3e4856cc" />

## CAD Modeling of the Motor Mount














