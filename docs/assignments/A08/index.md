# A8 – Gears

### Objective
Design a gearbox which can be assembled and disassembled. The spur gears have a gear ratio of 24:9 and are listed in the resource section. The output gear torque and speed are to be 1.25 in-lbf and 1100 rpm relative. The input (pinion,power-transmission) and output (gear, short shaft) shaft diameters are .125 and .25 inches respectively and each have a length of 1 inch. Use the appropriate equations in the Machinery’s Handbook for empirical units. The critical features of the gearbox include the shafts, and the journal bearings.

### Part 1 - Shaft Design

For this Part of the assignment, I was tasked with designing the input and output shafts for the gearbox with the provided dimensions. 

<img width="1524" height="836" alt="image" src="https://github.com/user-attachments/assets/ed9ee395-5bfd-44b0-9ba8-79113341c757" />

<img width="1528" height="820" alt="image" src="https://github.com/user-attachments/assets/2f59c9dd-7335-4f19-a14f-5f6dbeb4974f" />

### Part 2 - Journal Bearing

For this part, the goal was to find the PV value, compare it to a table to select the proper material, and determine the thickness.

<img width="1528" height="752" alt="image" src="https://github.com/user-attachments/assets/2b02eb85-42a1-49d7-a9b8-d54bbe551e4c" />

### Part 3 - Sketch

Before starting the CAD model, I drew a basic sketch of the gearbox’s top and bottom halves. It gave me an outline for the housing shape and helped me plan where the gears, shafts, bearings, and mounting holes would go. I used the sketch as a guide while creating the 3D parts.

<img width="712" height="392" alt="image" src="https://github.com/user-attachments/assets/2ed40efa-c731-4559-b477-8037f80f6c90" />

### CAD Work - 

I downloaded the gears and bearings I selected from McMaster-Carr and brought their CAD files into my project. This let me use the components’ actual shapes and dimensions as I designed the shafts and gearbox housing around them.

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/b5443f95-d301-4e26-bea8-c84c051112ac" />

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/9c04f43d-9dc7-4578-a74c-03476e3b65c2" />

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/b4e68fe5-9117-4293-b829-4273a3d3ee61" />

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/483c0640-d62e-482f-a4c0-9228947673f7" />


Next, I modeled the input and output shafts. I created a circular sketch using the specified diameter for each shaft and extruded it to the required 1-inch length. I then added a 45-degree chamfer to the end that fits into the gear hub to help guide the shaft during press-fit assembly.

### Output Shaft: 

<img width="450" height="200" alt="image" src="https://github.com/user-attachments/assets/ddbf8377-a90c-4358-ac9f-71f761e66b8a" />

<img width="375" height="200" alt="image" src="https://github.com/user-attachments/assets/879f0cc9-2743-4068-8622-b626f7bfcff6" />

<img width="575" height="250" alt="image" src="https://github.com/user-attachments/assets/24f8fc89-3497-466d-9a7b-b0c8d7b43f85" />


### Input Shafts: 

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/346b71fa-3e90-4475-b9a6-81d8647950d7" />

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/53291660-b778-4519-aeed-456fad734eb7" />

<img width="550" height="300" alt="image" src="https://github.com/user-attachments/assets/4237db1c-6d17-4b04-a6d6-636854eb1271" />

### Gearbox Shell

Now it was finally time for me to create the gearbox. I started by creating the bottom half of the gearbox. I started with a 4" x 3" box and extruded it to allow enough clearance for the gears and shafts to spin and rotate freely. I then used lines to help me find the center of the extrusion and to determine the offset that I needed to put the hole for the shaft. I did this for both the top and bottom gearbox. The last thing that I added was the holes along the edge so that the topa nd bottom can be secured together, preventing them from coming apart.

<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/f93c3712-cd39-443a-a72d-ce9ad86337a6" />

<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/e312e293-db40-4725-b2f5-33b8a52f491c" />

### Final Part

With the top and bottom halves of the gearbox housing completed, I can begin assembling the internal components. I will place each bearing in its housing seat, align the input and output shafts with the bearing bores, and fit the gears onto their respective shafts. I will position the gears so they mesh at the correct center distance and have clearance from the housing walls.

Next, I will mate the shafts and bearings to keep them aligned and set the gear rotation relationship to the specified 24:9 ratio. Because the gears mesh externally, they should rotate in opposite directions. I will then bring the housing halves together and check that their mounting holes line up and the internal parts have room to move.

Finally, I will rotate the input shaft to confirm that it drives the output gear smoothly, without binding or interference. Once the gears mesh and turn freely inside the closed housing, the gearbox assembly will be complete.


<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/38058675-7631-45b6-9258-0b3bd8d21c59" />

<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/350ea6f0-741f-4d7f-a0a8-b2ecbe87e915" />

<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/643128cb-2ace-48de-9a58-8c9b46f84167" />


<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/f2e56a9d-dd97-4808-a0e8-cc307c979806" />

### Lessons Learned

This project helped me understand that CAD modeling involves more than creating parts that look correct. The shafts, bearings, gears, and housing all have to fit together in the right positions. I learned that even a small clearance problem can cause parts to rub or gears to bind, so I need to plan room for the gears to rotate freely to avoid interference as I build the assembly.

I also had to relearn the math used with gears. I reviewed how the 24:9 gear ratio relates the input and output speeds and torque, and how pitch diameters determine the distance between the gear shafts. That math helped me understand why the gears need to be positioned precisely to mesh. I learned that calculating the gear forces also matters when checking whether the shafts and bearings can support the design.

The hardest part of the project was stacking the top and bottom halves of the gearbox after placing the parts inside them. It took several rounds of trial and error to align the shafts, bearings, and gears so the housing halves would fit together and the gears could mesh without hitting the housing.

Overall, I learned to think about how parts work together while modeling them. Careful measurements, clearances, and assembly checks are just as important as making each individual part.


This project took me about 10 Hours to complete from start to finish

### CAD Links

### CAD Part Files

### CAD File
[Download the CAD files for this assignment]((https://drive.google.com/drive/folders/1Bz5pxItmfjdOTA9RV51qsRzwG2u-Q_e4?usp=drive_link))



















