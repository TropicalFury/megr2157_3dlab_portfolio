# Lab 5 - Design a Snap Fit

## Prompt
The objective of this lab was to design two parts that mate together using a snap fit. The two parts were to be designed with the use of parameters and constraints in a CAD system of our choice. The design came with a few stipulations and constraints:
- Use a common Young's Modulus and yield strength value of PLA found through research
- Use a Safety Factor of 3.5
- A transverse load of between 0.25 and 5 lbf
- An axial load for the clip of 5 - 10 lbf

The design process also had its own set of required steps for documentation and iteration:
- Initially chose the width and base of the flexure
- Solve the length of the flexure using the beam equation for cantilever beam with a concentrated load at the free end
- Generate a separate FBD of each component
- Determine the bending stress of the flexure component using appropriate force, making sure the stress is less than the strength of material and SF
- Determine the axial stress of the flexure with an appropriate load
- Determine the average shear stress of the flexure protrusion
- Iterate if needed

## Research and Brainstorming
I started my research with finding some common values for PLA filament. From UltiMaker's website I found a Young's Modulus value of 3250 +/- 119 MPa and a yield strength of 52.5 +/- 0.9 MPa. I moved forward to researching snap fit parts so I could come to a general idea of what I wanted to make with the hand calculations using those values I found. 

There were many different designs depending on the required fit of the parts. Some were for latches, some for joints, and others for permanent connections that needed a cheap but effective way to click togehter. I wanted to make something I would actually make use of, and I thought about making a part that would hold my laptop cable in place at my desk. This came from the problem of having to always reach in between my desk and the wall of my room if I needed to plug in my laptop or take the cable with me. With some research and thoughts about the design I decided to use a cylindrical snap joint for my design. One part would have a pair of arms to clamp around the cable and I would make a second part to test the fit and show the viability of the design without having to take my charging cable everywhere. 

## Design
The first step of the design modeling process was to take my values for physical dimension and assign them to parameters for the part in my CAD system of choice, SOLIDWORKS. While some were values were shared across both parts, each one had its own set of parameters and use cases.

**Part 1: Clamp End**

<img width="696" height="456" alt="image" src="https://github.com/user-attachments/assets/76c17c91-ddf2-4985-89e4-2eb0657ce471" />

The first has all the parameters used in the design modeling process, some of them being specific to this part.

<img width="1160" height="744" alt="image" src="https://github.com/user-attachments/assets/48a960d0-423e-41fa-98bc-88b6beb94484" />

By far the most complex geometry of the part, dimensions use either the parameter value exactly or use it in an equation to define a needed size due to the part being developed on one side and then mirrored across a centerline.

<img width="1011" height="721" alt="image" src="https://github.com/user-attachments/assets/227267ad-9927-447b-bc18-ab0aabb464f8" />

The decision to make the first extrusion a midplane was deliberate to save time in finishing the last extrusion of the part.

<img width="866" height="748" alt="image" src="https://github.com/user-attachments/assets/1df89733-1df2-4367-af1b-7649c25654dd" />

The first extrusion for the clamp end part.

<img width="791" height="691" alt="image" src="https://github.com/user-attachments/assets/2898c91a-1acd-49e3-8280-606b19f24e11" />

The base sketch of the ends that keep the ends of the inserted part from moving up or down.

<img width="979" height="769" alt="image" src="https://github.com/user-attachments/assets/cf3aec46-7297-48b9-9661-759bf05b6bb3" />

<img width="704" height="724" alt="image" src="https://github.com/user-attachments/assets/e648abfd-ce4d-498f-b202-dfe44e63f056" />

The extrusion of the top holding end with a slot for the cable to extend out from.

<img width="620" height="699" alt="image" src="https://github.com/user-attachments/assets/7b33e39f-0ac4-4c68-8d51-6ac3cea94223" />

This extrusion was then mirrored onto the bottom of the part about the Top Plane, hence the use of a mid-plane extrusion earlier in the process.

<img width="631" height="742" alt="image" src="https://github.com/user-attachments/assets/25a8ce69-7ff4-4960-9ce6-9815d2612f6a" />

A few finishing touches using fillets to eliminate sharp edges and allow easier insertion of the second part or laptop cable.

<img width="241" height="353" alt="image" src="https://github.com/user-attachments/assets/2bc745b2-682c-4e55-a9a7-d509e6703655" />

The final modeling tree of the first part.

**Part 2: Inserted End**

<img width="698" height="343" alt="image" src="https://github.com/user-attachments/assets/5be70e2c-3795-4780-8323-1ef42a78fbdb" />

Fewer parameters for the second part, but all the ones here were the same from the first part.

<img width="949" height="686" alt="image" src="https://github.com/user-attachments/assets/f0ec1816-c4fc-4dd4-9433-250c2493e943" />

The base sketch for the inserted end.

<img width="990" height="705" alt="image" src="https://github.com/user-attachments/assets/c7b3b5cd-8cd6-4a8d-90b4-d3213d23f60c" />

Details of the extrusion of the inserted end.

<img width="738" height="706" alt="image" src="https://github.com/user-attachments/assets/67c5b1e8-b088-4c97-9868-6b972f940c43" />

The final version of the inserted part after some finishing touches with fillets to eliminate most sharp edges.

<img width="239" height="266" alt="image" src="https://github.com/user-attachments/assets/1e477484-2aa8-4447-afd5-d72bdb10e11e" />

The final modeling tree of the second part.

## Pre-printing Process


## Printing & Testing


## In Review
