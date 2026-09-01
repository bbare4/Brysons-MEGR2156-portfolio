# Project Overview
For this assignment, I developed and analyzed a truss system using certain parameters. The work below documents the geometry, support reactions, member force analysis, minimum member cross-sectional area, estimated truss weight, and pin shear sizing. I've organized the page so that each step and calculation shows the development of my design.

The truss used in my calculations has a pin support at A and a roller support at B. The top member is 1.20 m long, and joints C and D are located 0.30 m below the top member and 0.40 m in horizontal spacing from the reference lines. There are 25 kN loads that are acting upwards at point C and a 25kN load that is acting downward at D.

<img width="440" height="257" alt="image" src="https://github.com/user-attachments/assets/1078a484-4112-489c-a2a1-791b0f1df26f" />

# Establishing the Truss Geometry 
I began by sketching the truss and labeling the  joints A ,B ,C, and D. The members used in the analysis are AB, BC, CD, DA, and AC. I then added the known dimensions: 0.4 m between BC, CD, and AD. I also added the vertical distance of 0.3 m. Next, I picked a load between 20 and 30 kN. I chose 25 because it was in the middle, and I felt it was a good load to choose. Since A is a pin support, I included reaction forces Ax and Ay. Since B is a roller support, it has only one reaction force: By.

# Solving for External Reactions
Before I could analyze the individual members, I had to solve for the external reactions for the entire truss. I took moments around A because B has only 1 unknown and A has 2 unknowns. When I took moments around A, I ended up with -8.333 kN for By. Then I used the By value to solve for my Ay using the sum of forces in the y direction. That gave me Ay equal to 8.333 kN. With no horizontal load on the truss,the horizontal forces equal out to zero, so Ax is equal to 0.

The negative result for By means the actual reaction acts in the opposite direction from the originally assumed direction.

<img width="580" height="493" alt="image" src="https://github.com/user-attachments/assets/ec03934a-966f-452c-b80b-060b168fc71e" />

# Method of Joints
After finding my reaction support forces, I used the method of joints to solve for my internal forces. At each of the points, I used the sum of forces in the Y direction and the X direction to solve for the axial member forces.

### Joint B
I started at B because the support reaction was unknown and it had only 2 unknown member forces. The 0.30m by 0.40m geometry gives BC = 0.50m, and my trigonometric work records the angle as 53 ° 13 '.  Using this, I calculated the sum of forces in the Y, giving BC = 13.89 kN, and the sum of forces in the X, giving AB = -11.11 kN. When it comes to internal forces, the sign of the forces either tells you that it's in tension ( positive ) or compression ( negative ).

<img width="580" height="493" alt="image" src="https://github.com/user-attachments/assets/277baa16-0a37-4551-b08c-b28473d1b7d6" />

### Joint C
For joint C, I started by solving for the length of AC, which was 0.8544 m. I then used this length to find my direction ratios for my sum of forces:e cosθ = 0.9363 and sinθ = 0.3511. Using these components, I used my sum-of-forces equation to get AC = -47.47 kN and CD = 33.333 kN. The negative AC result just means that the member is in compression based on the assumed force direction when making the FDB.  This force becomes the largest member force in my work, so it will control member sizing later in the design.

<img width="580" height="493" alt="image" src="https://github.com/user-attachments/assets/16f0b702-2176-4ac8-bfc7-7ac7fde59a32" />

### Joint D
For Joint D, I just used my sum of forces to find the last member for DA, which equaled 41.67 kN. I now have all the member force information I need to begin stress-based sizing.

<img width="580" height="493" alt="image" src="https://github.com/user-attachments/assets/16148330-46c5-499c-96d7-5b68d6a27458" />

# Selecting the Critical Member
As I mentioned earlier, the controlling member in my analysis is AC at 47.47 kN in compression. The known parameter values we received are a safety factor of 3.5, a yield strength of 345 MPa, and a density of 7850 kg/m³. Below I will list all of the knowns and unknowns:

<img width="580" height="493" alt="image" src="https://github.com/user-attachments/assets/48d78381-a292-4498-9d3b-86567a1c96e0" />

# Minimum Member Cross-sectional Area
When it came to solving for my cross-sectional area, I used the normal stress relationship σ = F/A and the defined allowable stress factor using the safety factor that was given , σallow = σy/N. I then rearranged the equations to give me Amin ≥ NFmax / σy.

<img width="580" height="493" alt="image" src="https://github.com/user-attachments/assets/675c19dd-f760-4b73-9dc5-6b0562d34a4c" />

I then used these formulas to solve for my Amin = 4.816×10^−4 m² or 481.6 mm²

<img width="700" height="493" alt="image" src="https://github.com/user-attachments/assets/55626b0d-7ac8-4a17-ba39-a04ff6069599" />

# Estimating Truss Member Weight
I added all of the member lengths shown in my worksheet: AB = 1.20m, BC = 0.50m, CD = 0.40m, DA = 0.50m, and AC = 0.8544m. The total length after adding all of these up was 3.2544m. I then used V = AL to find the volume, and m = pV to find the mass of the truss. I also used W = mg if I needed the weight force. My values for these records were V = 0.001664 m³, m = 13.06 kg, and a final member weight of 128.1 N or 28.8 ibf.

<img width="640" height="558" alt="image" src="https://github.com/user-attachments/assets/53f852cc-67be-4236-b0ae-c87395e13f29" />

# Pin Shear Analysis
The pins are sized using shear stress rather than normal stress. For my calculations, I used the largest support reaction rather than the largest internal member force. The recorded values are 8.33 kN = 1.873 kip, shear strength 170 ksi, safety factor N = 4, density 0.278 lb/in^3, and one shear plane. Below is me solving for this symbolically:

<img width="793" height="382" alt="image" src="https://github.com/user-attachments/assets/b803d62e-59cd-4c5f-a8a0-1bd6baa15a58" />

Below is me solving for this numerically: 

<img width="537" height="600" alt="image" src="https://github.com/user-attachments/assets/bd1afd77-d81c-4820-82ac-992f818e919c" />

# CAD Model of Truss System
After completing my analysis and determining the dimensions of the truss members and pins, I began creating the 3D truss model in SolidWorks. To start my CAD model, I used the line tool to create the outline for my truss body. After that, I extruded the lines to create the 3D version of my 2D model.

<img width="2036" height="1026" alt="image" src="https://github.com/user-attachments/assets/d4c4effc-a238-408f-80ca-6c0c23f4491f" />

Next, I spent a few minutes coming up with different ways to design where the pins would go and how to connect the trusses. Below are some of the early designs I came up with while modeling the pin joints for these trusses. The design that I ended up using for my trusses is the circular one that you can see in the top left. I felt like that best represented the joints while keeping the pin distance within the parameters.

<img width="1376" height="1032" alt="NBMetadataCache" src="https://github.com/user-attachments/assets/0aa881c6-5cc7-4818-89ce-37b729a32480" />

After deciding to add the circular joint, I spent some time in SolidWorks installing it on the truss system, as you can see below.

<img width="2102" height="1270" alt="image" src="https://github.com/user-attachments/assets/848e8ee4-f050-4599-abed-5f71921e81aa" />

After creating the truss joints, I knew it was time to start working on the pins that would hold it all together. I started with a circle with a diameter of 0.0635m. Then I extruded the circle 0.022 m, the same depth as the trusses, to give a smooth finish when the pin is inserted. Below is the finished pin with the measurements.

<img width="1448" height="1092" alt="image" src="https://github.com/user-attachments/assets/652cb7a6-a318-4580-8fa7-18b468e0d160" />

Now it was time for me to install the pins into the joints to secure the trusses together. I had to add each pin into an assembly with the main truss. Once the pin was in the assembly, I used a feature called Mate in SolidWorks that allowed me to easily install the pins into the holes. As you can see below: 

<img width="2550" height="1416" alt="image" src="https://github.com/user-attachments/assets/84f5aa2b-1ed2-4a08-ae26-844b7d454345" />

Now all I have left to do is have SolidWorks calculate the truss weight and compare it to my own. When selecting materials for my truss, A500 structural steel wasn't an option, but ASTM A36 steel was, and it's extremely similar to A500. For my pins, I had to use AISI type A2 tool steel, which has very similar numbers to the steel I used in my problems.

<img width="1630" height="1306" alt="image" src="https://github.com/user-attachments/assets/91ac18f9-86cb-4131-8233-02f6489578eb" />

After SolidWorks measured the weight of the truss, it said it weighs 12.83 kg, which is very close to the value I solved for in my hand calculations (13.06 kg). Below are the hand calculations for when I solved for truss weight :

<img width="734" height="496" alt="image" src="https://github.com/user-attachments/assets/ba001666-7baa-4915-9f3d-db8301f6c7b4" />

After doing some basic math, I learned that the percent error between the hand-calculated weight and the SolidWorks weight was only 1.76%.

<img width="646" height="384" alt="image" src="https://github.com/user-attachments/assets/2d326d48-1dc1-49f0-b711-980f1956ccc4" />

Here is the final truss, all put together: 

<img width="2560" height="1416" alt="image" src="https://github.com/user-attachments/assets/b8fdaa5f-42fc-46eb-a912-af6c6905b7b8" />

The downloadable links for the CAD model will be submitted inside a PDF into Canvas and will be on this Google Drive: 

[Download CAD Files from Google Drive](https://drive.google.com/drive/folders/1akkGbr3GPoff2P-tgb-UEINVovxZqkha?usp=drive_link)

# Engineering Lessons Learned: 

One main engineering lesson that I really learned while doing this project over the last 4 days is time management. After doing the math portion of this assignment, I underestimated the 3d modeling section and focused on other assignments, pushing this to the last minute. If I had started this much earlier, I wouldn't have felt so rushed and anxious to finish the night before. One of the major problems I faced was putting the pins into the joints, which sounds easy, but for some reason it gave me trouble. Both situations made me rush and finish everything the night before, but it was a good lesson for future assignments.

This assignment took me about 11 hours to finish.





























 







