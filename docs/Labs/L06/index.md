# Lab 6 - Design Fits for an Artifact

## Prompt

This lab was about designing a snap fit for a certain artifact that we were given to mate our part to. This part was to be designed parametrically and with constraints in CAD. The design process came with a few instructions listed as follows:
- Take needed measurements of the artifact
- Create hand sketches of the part for physical reference and to be included in the portfolio
- Create the feature in a CAD system of our choice
- Test the design after printing and if it did not fit properly, remake the part
- Detail the decision making process and how the fits and allowances of the interactive parts were engineered

## Research & Brainstorming
**Artifact Information**

The artifact to design a snap fit part for was the Raspberry Pi Pico. It is a starter board for beginners learning about electronics and coding. A rather small part with a lot of elements on the top side of the board, any snap fit design would need to have adequate clearance for those elements. Initial thoughts were to clamp the Pico from the short ends around the USB input plug and screw holes. This would allow for a lot of flexure in the cross-members of the part rather than the prongs that snap fit. The aim with that was to make said prongs last longer and not the be failure point of the part which would result in the artifact coming loose. After consideration of possible interference with a cable connected, the decision was changed the clamp the artifact on the long sides close to the corners, using the force of the snap and friction to hold the artifact in place.

**Artifact Measurements**
The design choice to hold the part from (blank location) on the artifact necessitated recording of the following main measurements:
- Width: .827in/.804in
- Length: 2.008in/2.020in
- Thickness: .042in/.144in

What made the measurements come out in two values is main board has the larger width and length but the supporting structure for the pins on the underside of the board has slightly different dimensions and provide a larger thickness, all of which had to be accounted for in the design. Other measurements were taken as well that pertained to the initial thoughts about the design and how it would snap to the artifact. 

<img width="650" height="321" alt="Screenshot 2026-09-28 235154" src="https://github.com/user-attachments/assets/b082f14a-042d-4aa8-a798-bc59a76c73f8" />

## Design
The CAD system chosen for this project was SOLIDWORKS. 

## Pre-printing Process
The file was imported into PrusaSlicer for slicing and pre-print processing. 

**Print Settings**
- Material: PETG (Blue)
- Wall Thickness: 0.86mm
- Layer Thickness: 0.2mm
- Layers: 5 for top and bottom of part
- Build Volume: 
- Slicer Settings: 
- Infill Percentage: 30%
- Infill Type: Gyroid

## Printing
The part was printed on a Prusa Core One FDM printer.

<img width="3024" height="2609" alt="IMG_7713" src="https://github.com/user-attachments/assets/1e39f7d7-4f5d-4f3d-a458-84c6a25d5d87" />

The first capture shows the printing progression past the bottom layers and into the infill stage where the gyroid pattern can be seen.

https://github.com/user-attachments/assets/711ea5a5-9e37-4f58-9d4c-9ef3039d8534

The printing in the early stages, again showing the infill and rapid speed of production for a small part like the one designed here.

Unfortunately, the first iteration of the printed part did not meet the desired performance in terms of the snap fit and ability to hold the artifact in place. It could easily shake once inside the prongs and easily slip out, so the part had to go to a second iteration with improvements.


No supports were necessary in the making of the associated part due to the small size of the snap overhangs, something the Prusa Core One was able to handle.
## In Review & Lessons Learned

