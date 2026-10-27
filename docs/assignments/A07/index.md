# A7 – [FEA on Bracket Design]

This assignment builds upon the previous bracket design developed in Assignments #5 and #6. Although this assignment continues the original model, several modifications improve the component's overall stability and structural performance. These changes create a more stable geometry and allow better control and distribution of the applied load. The objective remains to design a bracket that is strong, stiff, and lightweight, using Finite Element Analysis (FEA) to ensure stress, displacement, and safety factor results differ by no more than 7% at each mesh-refinement stage.

All three designs use SOLIDWORKS 6061-T6, a 600 lbf downward load on the lower cylinder, and fixed underside retaining-lip faces. We tested three mesh sizes for each design. The plots below show the finest-mesh result for each design; the tables retain the mesh comparison needed to judge convergence.

# Design 1
For design 1, I kept the original bracket geometry; I made no geometry changes. The sharp stem-to-crossbar at the top of the part was a stress hot spot. I used the finest available mesh: 0.10 in. Below is the information, picture, and calculations for each of the FEA finest meshes. 

<img width="2466" height="768" alt="image" src="https://github.com/user-attachments/assets/2d200395-2626-426d-b48a-4330ae091234" />

<img width="1604" height="540" alt="image" src="https://github.com/user-attachments/assets/fdc000d2-2223-4159-b145-189be1db911b" />

# Design 2

For design 2, I added a 0.15 fillet where the stem meets the crossbar to help smooth out the stress hotspot that I found when I ran the FEA for design 1. During design 2, I tested 3 different mesh sizes, and the photos below only show the finest mesh (0.075 in). Its stress changed by 7.08% from the previous mesh, just over the 7% limit, so I stopped here and used the finest-mesh result for design 2.

<img width="2458" height="750" alt="image" src="https://github.com/user-attachments/assets/b7c0e306-002c-4b7f-9af6-b969a1c548db" />

<img width="1604" height="534" alt="image" src="https://github.com/user-attachments/assets/97ec606e-5540-48a3-bb01-0fd51386858a" />

# Design 3
For design 3, I kept the root fillet that I created in the previous design, but this time I increased the stem depth from 0.659 to 1.00 to help reduce the bending that has been happening in the last 2 designs. The final stress change was 2.89%, which is well within the 7% limit, so I was happy with these results.

<img width="2470" height="754" alt="image" src="https://github.com/user-attachments/assets/eebc72c6-202b-49fb-b5a8-a9c82d699159" />

<img width="1608" height="544" alt="image" src="https://github.com/user-attachments/assets/ac945b84-e157-4270-8df1-06e0e921c03d" />

# Final Mesh Comparison

<img width="2134" height="332" alt="image" src="https://github.com/user-attachments/assets/5d28003f-cc73-46e9-a675-b4fdfc272e36" />

<img width="1180" height="266" alt="image" src="https://github.com/user-attachments/assets/ccd912d3-f521-4641-8891-090596ff348a" />

From Design 1 to Design 3, the finest mesh deflection dropped from 1.251 mm to 0.3884 mm; stress coverage was 2.89% between the last two meshes. Its safety factor was 3.67 versus the target safety factor of 4, and its mass was 24.1% above the baseline. Only design 3 passes the 7% stress convergence limit after 3 mesh attempts.

# Learned 
During this assignment, I learned how changing mesh size affects FEA results. Running each design with progressively finer meshes helped me check whether stress, deflection, and safety factor were converging before I started changing the geometry. Another thing I learned when adjusting the geometry is that sometimes what you think will decrease stress and deflection doesn't help as much as you expect, and then I had to come up with new ideas. I also learned how to use Excel to organize all the calculations and my FEA results. While it took some time and some help from AI to set it up, it made it easy to track mesh sizes and element counts and compare my 3 designs.

# Time

Overall, this assignment took me around 6-7 hours to complete from start to finish. I spent most of that time making changes to my design; I tried to keep it as original as possible without making a whole new product. That probably made the assignment take longer.

[Click here to Download Design 1 (.SLDPRT)](../../../A07-Design1.SLDPRT)

[Click here to Download Design 2 (.SLDPRT)](../../../A07-Design2.SLDPRT)

[Click here to Download Design 3 (.SLDPRT)](../../../A07-Design3.SLDPRT)








