# A11 – Motor Selection

This project focuses on designing the motorized drive and support structure for a benchtop tensile tester with a 2 kN load capacity. The tester uses two lead screws to move a crosshead and pull a test specimen. By applying tension, the machine can help show how a material responds to load and how much it stretches before it yields or breaks.

Our team will select a motor, design motor mounts, choose or design a coupler, and develop a stable frame and specimen clamps. The design must support the required load with a safety factor of 4, keep the specimen and crosshead aligned, and fit within a practical bench-top size. The lead screw system must also meet the required travel-speed range of 1–50 mm/min and have a minimum lead screw length of 18 inches.

The final work will include CAD models of the engineered parts, supporting sketches and free-body diagrams, design calculations, and a bill of materials with estimated costs. This assignment documents the design process as well as the final design, including decisions, mistakes, and lessons learned.

<img width="352" height="452" alt="image" src="https://github.com/user-attachments/assets/32f8cb7b-e6f8-40a3-a5d7-6e4c7517d258" />

## Motor Selection and Attachments -  (Bryson Bare)

We selected the MOONS’ AM34HD2403-07 hybrid stepper motor because the tester must move slowly while pulling a high load. The stepper motor can provide controlled movement at low speeds, and this model has a listed holding torque of 9.4 N · m. We assumed that one motor would drive each lead screw, so each screw carries half of the tester's 2 kN load. The holding torque helped us identify a candidate, but we use the speed-torque curve to check the torque while the motor is running.

<img width="623" height="709" alt="image" src="https://github.com/user-attachments/assets/85415d0b-f1e4-4ab4-a0e9-1502d2dde7ae" />

<img width="621" height="396" alt="image" src="https://github.com/user-attachments/assets/b79f1e25-2820-4e73-8c9e-4927df5df150" />

# Motor Mount Design (Bryson)

After selecting the motor, we needed to design a motor mount to hold it. We designed a four-bolt motor mount to attach the motor securely to the tester frame. We calculated the force on each bolt from the motor’s reaction torque, checked the plates' bearing stress, and found the minimum thickness needed to meet the allowable stress. Because the minimum thickness was so thin, we selected a 10mm plate for a more practical and rigid mount. I also had to account for the thickness of the top of the frame when choosing the bolt lengths that will hold the mount to the frame. I chose 20 mm because the mount is 10 mm thick and the frame is 10 mm thick.

<img width="941" height="403" alt="image" src="https://github.com/user-attachments/assets/7590605a-62f5-487f-8f1e-e6ce74381ab7" />
<img width="787" height="665" alt="image" src="https://github.com/user-attachments/assets/ad82bf65-e582-445e-b592-6ba1a7fed4a5" />

## Coupling Design (Bryson)

We selected the McMaster-Carr 2764K425 coupler because its 14mm and ½ in bores match the motor shaft and the lead screws nominal diameter. This would connect the motor to the lead screw. The coupler is rated for 89 in*lbf, which is higher than our design torque. Its speed rating also exceeds the leads screws max speed. The flexible discs help accommodate any slight misalignment between the shafts. For a secure fit, the screw end will need to be a smooth section where it enters the coupling. 

<img width="1100" height="499" alt="image" src="https://github.com/user-attachments/assets/41a74f54-44ee-40dc-8d0b-07a55f3b65c4" />
<img width="939" height="635" alt="image" src="https://github.com/user-attachments/assets/415d65ef-04af-48be-a5a3-56c6007566e3" />

### Total time Bryson: 5 Hours

## Analyze and design a Frame - Nolan

For analyzing the frame, I was tasked with running an FEA for the top of the frame and the vertical components of the frame, to ensure the frame will have very low deflections. 

**Top of the frame**

For the top of the frame, I loaded up the CAD assembly for our frame and started a new study. I then measured from the outside edge of the crosshead to the center of the leadscrew hole. 

<img width="942" height="587" alt="image" src="https://github.com/user-attachments/assets/38fdc6f4-c702-4fd5-8341-0b0e1ffdb825" />

I used this measurement to determine where to put the 1kN forces on the top of the frame. I also added this distance to it

<img width="941" height="587" alt="image" src="https://github.com/user-attachments/assets/57b5d94b-4fbd-4536-8404-e9bdf8fc0444" />

I then used this measurement to create a point on the surface of the beam that I could refer to when placing a force down. This did not work, which led me to having to sketch circles around the point. This also did not work, so I had to split the geometry for the face of the beam with the circles I sketched as seen here:

<img width="945" height="592" alt="image" src="https://github.com/user-attachments/assets/4e98fb08-43c6-49c9-9412-803f0b1311e1" />

I then realized that after a 50/50 chance, I did this on the side that was underneath for the assembly, leading me to having to redo this again. After all of this which took around an hour to learn how to put a single force on this one specific location, I had this:

<img width="947" height="590" alt="image" src="https://github.com/user-attachments/assets/00eb92b1-2888-4b7f-b850-260c1320c080" />

### Mesh:

<img width="944" height="591" alt="image" src="https://github.com/user-attachments/assets/cf17c2e3-4a4f-47c8-8fc8-22caf58e8ce8" />


I then realized although not stated in the canvas page, the analysis was supposed to be done for just the beam and not the whole frame and crosshead together. I created these forces and fixtures:

<img width="938" height="588" alt="image" src="https://github.com/user-attachments/assets/0fa2a132-19f0-44a5-b1c9-630071d96306" />

After applying a material and running the study, I was left with these results:

**Von Misses**

<img width="952" height="597" alt="image" src="https://github.com/user-attachments/assets/7554b26f-e009-4e28-8fab-f50d2b73afd6" />

**Deflection**

<img width="949" height="595" alt="image" src="https://github.com/user-attachments/assets/9b69b49b-3d4b-48d1-90db-a786a2961d6d" />


**Safety Factor**

Safety factor was 7.7 everywhere.

This safety factor was well above the project's given 4 value, so I decided it was good to move on to the Side of the frame.


**Vertical Frame**

To check the vertical frame, I ensured that the frame could withstand the 1000N from the leadscrew, as well as the torque from the lead screw (calculated to be 16.6 N*m). Here are my forces and constraints:

<img width="944" height="592" alt="image" src="https://github.com/user-attachments/assets/1ec36f0f-dfeb-475f-97b5-0ca6b5700a2d" />

I then ran the study and got these results:

**Von Misses**

<img width="945" height="590" alt="image" src="https://github.com/user-attachments/assets/720fc892-f76c-4750-ad5f-59518e8fdbfe" />

**Deflection**

<img width="938" height="589" alt="image" src="https://github.com/user-attachments/assets/c7549086-fb79-4b63-97be-8b56e124e7d6" />


**Safety Factor**


I got back a calculated safety factor of 12. This was way above the safety factor of 4, so I decided to deduct that this frame was built strong enough to not need any changes to the overall design. 


### Total time Nolan: 2 hours 

## Design floating Bearing Mount - Brandon Hudson
I first started designing the motor mount with the dimensions Bryson came up with in the math above. Below is the sketch of the motor mount. 

<img width="686" height="509" alt="image" src="https://github.com/user-attachments/assets/90fbd030-a715-4c76-907e-f9a22fdcfefb" />

After doing the sketch I completed the extrude which was a total of 10mm. I then created the 4 holes on the mount and dimensioned them to the correct dimensions given to me by Bryson.  Below is the motor mount after this extrude and the holes inserted. 

<img width="692" height="474" alt="image" src="https://github.com/user-attachments/assets/94934116-6e7d-4d5d-b9ab-e8cea958266c" />

After completing the extrude and holes I finished up the motor mount. Below is the final product of the motor mount. 

<img width="693" height="468" alt="image" src="https://github.com/user-attachments/assets/5d9e6c64-ecf2-43e2-8ca7-0dd67abef95f" />

I then moved onto the assembly by downloading the couplings, motor, and screws needed to fully assemble the motor and frame. I got all the parts needed and began assembling the finished product. Below is the final assembly. 

<img width="688" height="762" alt="image" src="https://github.com/user-attachments/assets/01a0bda6-9626-4dd2-9b8d-274c7790dfcf" />

<img width="690" height="702" alt="image" src="https://github.com/user-attachments/assets/3caf58d1-7ec7-4f3a-9b02-e831138672ac" />

## Bill of materials and labor costs - Brandon Hudson

| Item # | Quantity | Name | Cost/item | Cost | Link |
|:---|:---:|:---|---:|---:|:---|
| AM34HD2403-07 | 2 | Hybrid Stepper Motor | $198.00 | $396.00 | [MOONS' - AM34HD2403-07](https://www.moonsindustries.com/p/am-series-standard-hybrid-stepper-motors/am34hd2403-07-000004611110010745) |
| 2764K425 | 2 | Shaft Coupling | $118.34 | $236.68 | [McMaster-Carr](https://www.mcmaster.com/2764K425/) |
| 91274A141 | 1 pack (50) | Socket Head Screw | $10.63 / 50 | $10.63 | [McMaster-Carr](https://www.mcmaster.com/91274A141/) |
| 98940A305 | 2 | Lead Screw | $28.64 | $54.56 | [McMaster-Carr](https://www.mcmaster.com/98940A305/) |
| 97790A110 | 2 | Flange Nut | $178.60 | $357.20 | [McMaster-Carr](https://www.mcmaster.com/97790A110/) |
| 92316A540 | 4 | Socket Head Screw | $10.02 / 50 | $10.02 | [McMaster-Carr](https://www.mcmaster.com/92316A540/) |
| 47065T882 | 1 | Frame | $125.63 | $125.63 | [McMaster-Carr](https://www.mcmaster.com/47065T882-47065T752/) |
| **Total Cost** | | | | **$1,190.72** | |

## Lessons Learned – Engineering Design

Throughout this project, I improved my CAD modeling and mechanical assembly skills by designing a motor mount and developing a complete assembly that included motors, couplings, bolts, and mounting components. A major part of the project involved creating and modifying CAD geometry to ensure that all components fit together accurately. I gained experience working with individual part models, positioning components, and using assembly constraints to establish the correct relationships between parts.

One of the more challenging aspects was designing portions of the supporting frame to ensure the motor would fit correctly. I had to determine the necessary dimensions, create mounting features, position holes, and modify the frame geometry to accommodate the motor mounts and other components. This required repeatedly checking component clearances, alignment, and positioning to ensure the assembly functioned as an integrated mechanical design.

This project taught me the importance of developing accurate and organized CAD models while considering how individual components interact within a larger assembly. I also gained a better understanding of how to approach custom part design, troubleshoot assembly interference, and make dimensional modifications without compromising the overall design. Overall, the project strengthened my ability to translate mechanical design requirements into detailed 3D CAD models and complete assemblies.

### Total time Brandon: 8 hours

## Cad Files

The CAD files for A11 are available in the Google Drive folder below:

[Open the A11 CAD Folder](https://drive.google.com/drive/folders/16NzgxDtks0Jcl7XMD67j7Hv-oHWpTYXf)





