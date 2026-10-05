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

The artifact to design a snap fit part for was the Raspberry Pi Pico 2 W. It is a starter board for beginners learning about electronics and coding. A rather small part with a lot of elements on the top side of the board, any snap fit design would need to have adequate clearance for those elements. Initial thoughts were to clamp the Pico from the short ends around the USB input plug and screw holes. This would allow for a lot of flexure in the cross-members of the part rather than the prongs that snap fit. The aim with that was to make said prongs last longer and not the be failure point of the part which would result in the artifact coming loose. After consideration of possible interference with a cable connected, the decision was changed the clamp the artifact on the long sides close to the corners, using the force of the snap and friction to hold the artifact in place.

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
Coming full circle, the final design took 3 attempts to get correct. The edits came from making small changes to the part's geometry in a couple of places starting with the distance between prongs when looking at the part from the short ends.

**Distance Between Prongs**

<img width="3024" height="1917" alt="IMG_7736" src="https://github.com/user-attachments/assets/501a6e4e-4ea8-477d-8ecc-6c8b3b981020" />

The above picture shows the profile of the part around where it snaps to the artifact. The gap between prongs here with the first iteration was .835in.

<img width="3024" height="1955" alt="IMG_7744" src="https://github.com/user-attachments/assets/dfbfe3fe-5f03-4f5d-b4d5-2442727da93b" />

The second iteration saw that same gap tightened to .833in with the actual print, a decrease of 2 thou compared to a decrease of (blank) thou in the CAD model.

<img width="3024" height="2040" alt="IMG_7751" src="https://github.com/user-attachments/assets/21817125-94cc-4d95-ad99-eebc3d94fcc5" />

The gap between prongs on the final iteration came out to .829in upon printing, finally providing the necessary force to keep the part engaged on the artifact. While the part would stay engaged, prolonged use of the part being snapped onto the artifact could potentially open up the gap between prongs over time. This dimension could be tightened further to make the clamping force stay strong for longer, or more prongs could be added to provide more resistance.

**Prong Design**

The second area of the part that saw an iterative change were the prongs that snap onto the artifact. 

<img width="3024" height="2567" alt="IMG_7737" src="https://github.com/user-attachments/assets/f093fc06-1e18-41d7-a9c5-e9ecfac77455" />

The first design only had one set of what will be referred to as "claws" that snap around the main board of the part. These restricted motion when snapping onto and removal from the artifact, but allowed for movement once snapped on. The artifact could move closer to the support structure of the part, an undesired outcome that necessitated a fix.

<img width="3024" height="2148" alt="IMG_7741" src="https://github.com/user-attachments/assets/b5de43c8-3e19-4ae9-9003-d0f8cde8caa4" />

The second iteration had to claws on each prong that prevented the movement previously mentioned. No other changes were made to the prongs themselves besides this, but another potential problem was seen with how far the part support structure was to the elements on top of the artifact that stick out particularly far. Another change was made to attempt to rectify this.

<img width="3023" height="2657" alt="IMG_7750" src="https://github.com/user-attachments/assets/574c360f-bf5c-4f53-80d1-fc4343513b18" />

<img width="3024" height="2270" alt="IMG_7754" src="https://github.com/user-attachments/assets/aa7cf591-f7b5-441c-9245-cd81f872e8e4" />

The claws and profile of the prongs stayed the same for the final iteration except that they were made taller overall. The comparison between the second and third showing this change can be seen in the second image just above. This demonstrated a marked improvement in eliminating interference with the tallest elements on the artifact. The micro-USB input was easily cleared along with most other elements, but the debug plug-in still made contact with the middle cross-member of the supporting base. A further attempt was not made to eliminate this interference due to running into the time constraint, but this would be an emphasis for further change in a new iteration.

**Fit on Artifact**
The main goals of the design from the start were to keep part clamped with minimal material use, quick manufacture time, and retain the ability to use all elements on the artifact when the part is applied to it.

<img width="3024" height="2326" alt="IMG_7757" src="https://github.com/user-attachments/assets/7ce738cf-eabe-4e3e-a36d-3ef15d9779ca" />

The final fit of the part on the artifact showing how the first goal of the project was met.

<img width="3024" height="1993" alt="IMG_7756" src="https://github.com/user-attachments/assets/0319cb15-3288-467d-92e5-4366bbe35394" />

The openings in the support structure of the part allow for access to all elements on the artifact that can be physically interacted with.

Breaking down the overall time spent on the project, it took around 4 hours to design and print the project through three iterations and then around 6 hours to fill out the page in this portfolio and inspect the part in its final iteration, rounding out to an estimated 10 hours to complete total. The main point of improvement that can be made moving forward is to start the projects earlier so as to not run into time constraints and build up large amounts of external pressure.
