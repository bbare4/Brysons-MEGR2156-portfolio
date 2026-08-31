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






 







