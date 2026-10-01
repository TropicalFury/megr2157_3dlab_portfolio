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

What made the measurements come out in two values is the main board has the larger width and length but the supporting structure for the board and pins on the underside had slightly different dimensions and provide a larger thickness, all of which had to be accounted for in the design. Other measurements were taken as well that pertained to the initial thoughts about the design and how it would snap to the artifact. The main measurements and other important ones that came from having to work around the board's elements were entered into SOLIDWORKS as the parameters for the part file depicting the artifact in 3D space.

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
The part was printed on a Prusa Core One FDM printer. The first capture shows the printing progression past the bottom layers and into the infill stage where the gyroid pattern can be seen.

**First Printing Iteration**

<img width="3024" height="2609" alt="IMG_7713" src="https://github.com/user-attachments/assets/1e39f7d7-4f5d-4f3d-a458-84c6a25d5d87" />

The first capture shows the printing progression past the bottom layers and into the infill stage where the gyroid pattern can be seen.

https://github.com/user-attachments/assets/711ea5a5-9e37-4f58-9d4c-9ef3039d8534

The printing in the early stages, again showing the infill and rapid speed of production for a small part like the one designed here.

Unfortunately, the first iteration of the printed part did not meet the desired performance in terms of the snap fit and ability to hold the artifact in place. It could easily shake once inside the prongs and easily slip out, so the part had to go to a second iteration with improvements.

**Second Printing Iteration**

<img width="3024" height="2312" alt="IMG_7721" src="https://github.com/user-attachments/assets/640eee2a-b17b-4885-86a0-959d9a3ac12f" />

The overall design changed very little in terms of part geometry and no change was made in terms of wall thickness, layers, or infill as shown above.

<img width="3024" height="2797" alt="IMG_7724" src="https://github.com/user-attachments/assets/1177b6be-ab6f-4bfd-9617-a8d5f72efc57" />

Towards the end of the printing process only the prongs were left to be completed.

<img width="3024" height="1822" alt="IMG_7726" src="https://github.com/user-attachments/assets/2fd9afa4-50ad-4132-a111-6f84feb7fa3b" />

The completed second iteration as seen on the steel sheet after having just finished printing.

Despite the changes, the second iteration was still to loose in its snap performance to meet the desired results, so further design changes were made and a third iteration was set for printing.

**Third Printing Iteration**

The third print shown in the final stages of completion, rounding off the tops or the prongs.

https://github.com/user-attachments/assets/7fc3fa41-16fc-4dd7-8a56-c1c6960f3ac4

The third print shown in the final stages of completion, rounding off the tops or the prongs.

<img width="4284" height="2985" alt="IMG_7731" src="https://github.com/user-attachments/assets/84c0e590-021d-4523-8c7c-ffdf67ffcf95" />

<img width="4284" height="3201" alt="IMG_7732" src="https://github.com/user-attachments/assets/62d90bd7-e5e6-49ce-b889-36103f460e18" />

2 views of the third iteration after printing completion, one of the long side and the other from an isometric angle.

No further printing was needed because the third iteration met the desired snap performance and thus was the final iteration.

No supports were necessary in the making of the associated parts due to the small size of the snap overhangs, something the Prusa Core One was able to handle without issue.
## In Review & Lessons Learned
Coming full circle, the final design took 3 attempts to get correct. The edits came from making small changes 
