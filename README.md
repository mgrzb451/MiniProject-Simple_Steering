# Simceneter 3D - Simple Steering Mechanism Analysis
Exploring the Flexible Body Motion Simulation further. Designed a very simplified steering mechanism and the results I got left me with more questions than I had at the outset 😅

<img width="1465" height="815" alt="image" src="https://github.com/mgrzb451/MiniProject-Simple_Steering/blob/main/assets/3D_model.jpg" />

# Analysis
<img width="1504" height="816" alt="image" src="https://github.com/mgrzb451/MiniProject-Simple_Steering/blob/main/assets/flex_stress.gif" />

## Flexible Body Simulation Result
Estimated mass of `250 kg` is spread out evenly over 4 wheels of the Gokart. The coefficient of static friction between dry rubber and concrete is `1`.
We want to estimate the Normal Stress induced in the Steering Rod. The Flexible Body Analysis yields a value of just over `1 MPa`.

## Manual Analysis and Questions
When we perform a very crude manual analysis the results we get are completely different than what Simcenter produces...

Both manual calculation starting from the applied force and even calculations **based on Simcenter's own Torque result** are vastly different from the stress result in the Flexible Simulation 🤨
<img width="1744" height="862" alt="image" src="https://github.com/mgrzb451/MiniProject-Simple_Steering/blob/main/assets/hand_calc.jpg" />
<img width="856" height="372" alt="image" src="https://github.com/mgrzb451/MiniProject-Simple_Steering/blob/main/assets/Torquestrut.jpg" />

# Conclusions
1. Sadly I just don't understand how the software translates the forces in the structure to FEM results in the Flexible Body Motion Simulation.
The Force and Torque results produced by the Dynamic Simulation on Rigid Bodies seem correct and conform to manual calculations but the Flexible Body results are completely different than expected 😫
- Perhaps I had made too many simplifications in my analysis setup? 🤔

2. Despite the doubts that emerged I learned a lot of new things! 😄
  - Ackerman angle
  - steering system types and design basics
  - Ball joints types, manufacturing process and how much more prevalent IRL they are than I realized!



