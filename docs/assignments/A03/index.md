# A3: Parametric and FEA

#### Part 1:
The purpose of this assignment was to design a solid circular bar that is subjected to a direct tensile load between 300 lbf < F < 500 lbf while limiting the maximum axial deflection to 0.009 inches. The circular bar was also required to be constructed from aluminum with a modulus of elasticity between 8.5 x 10^6 psi and 11.5 x 10^6 psi. For my cross-sectional design, I chose a diameter of 0.50 inches for my solid circular bar. First, I calculated the cross-sectional area using the equation A = πd^2/4. Then I used the direct tension elongation equation, δ = AE/FL, and rearranged it to solve for length (L). I used the maximum applied force that I chose and the minimum modulus of elasticity to show the most demanding design condition. The calculations used to determine the bar values are shown below.

<img width="1141" height="900" alt="NBMetadataCache (1)" src="https://github.com/user-attachments/assets/ba2dbb9e-223c-460b-9a06-e724696b301d" />


#### CAD:

The first thing that I did was input my cross-sectional area dimensions into SolidWorks.

<img width="1910" height="1238" alt="image" src="https://github.com/user-attachments/assets/eac1c150-7435-4b2a-a40b-192783b138ec" />

Next, I extruded the length that I found and input it into my SolidWorks design.

<img width="2560" height="1506" alt="image" src="https://github.com/user-attachments/assets/41c8e049-deff-46dd-a313-65d86bb8f3f6" />

After that, I went to the Equations tab and entered all my variables. When I had SolidWorks do the math, I got the same answers.

<img width="1584" height="740" alt="image" src="https://github.com/user-attachments/assets/b3c2ccf3-41ad-4981-a221-750e4c1a5b23" />

This is the material I chose to use in SolidWorks and the material value I used in my hand calculations. I did this to accurately represent what my hand calculations showed.

<img width="1616" height="1358" alt="image" src="https://github.com/user-attachments/assets/283ac8ea-b43d-420d-8bef-160d539dee0b" />

#### FEA Simulation:

For the FEA simulation, I started by fixing one end in place and, at the other end, applied a 500 lb force pulling away from the bar.

<img width="2560" height="1316" alt="image" src="https://github.com/user-attachments/assets/d57b40dd-8267-4339-9701-9d384fb66b43" />

<img width="2548" height="1280" alt="image" src="https://github.com/user-attachments/assets/3ae62e2a-9782-4962-8dc9-7bf1c12a5f7c" />

#### Deflection Curve:

Next, I ran a simulation to find the deflection curve. The result was 0.009005, which matches the maximum deflection given to me and the deflection I solved for in my hand calculations. 

<img width="2554" height="1462" alt="image" src="https://github.com/user-attachments/assets/90d9eaa7-1856-474f-a8df-de1e6bc92b09" />

#### von Mises Stress Curve:

The von Mises stress curve shows that the beam's yield strength was 3.999e03, indicating a safety factor of 1.47. Since the maximum stress is 2738 psi and is lower than the yield strength of 3999 psi, the beam is within the material's allowable strength. 

<img width="2556" height="1494" alt="image" src="https://github.com/user-attachments/assets/0e117f0d-41d3-4615-b926-d886e581f551" />














