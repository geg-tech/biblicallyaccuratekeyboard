# The Biblically Accurate Macropad

This is a custom, 3d-printed macropad made to resemble a biblically accurate angel, powered by a Raspberry Pi Pico RP2040. <br/>

My intial goal for this project was to just simply make something cool for the summer and to keep me occupied, but soon grew into a very complex CAD and art project that I had loads fun working on (and also served as great Fusion 360 practice for school). <br/>

I learned lots of useful techniques in Fusion 360, such as the Surface modeling tools, Create Form, and the 3D Sketch feature, which I will use extensively in my other work like future hardware projects, school work, and for my team in VEX Robotics. I also plan to show off this project to my high school's IRL Hack Club to encourage more students to join Hack Club :3 <br/>

The macropad is powered with a RP2040 running QMK, which is soldered into a PCB in the center dodecahedron, and has external rings of key switches surrounding the center, all wired to the center PCB. <br/>

To fit the biblically accurate angel theming, the macropad has a common motif of eyes, which is often seen in interpretations and drawings of biblically accurate angels. The case is also made out of gold PLA filament, with the center, keycaps, and some decorations painted white to fit the color scheme often associated with angels. <br/>

## CAD
<img width="700" alt="image" src="https://github.com/user-attachments/assets/0de3e70f-f1d7-4ddf-9ae9-d1b76fbdbad3" />
<img width="596" alt="image" src="https://github.com/user-attachments/assets/7e9120c1-b31b-475a-9a18-8fdf20a21f9e" /> <br/>

## PCB + Wiring Diagram
### Schematic
<img width="500" alt="schematic" src="https://github.com/user-attachments/assets/1bce7456-8bae-4900-b491-a54f3b4d6997" /> <br/>

### Center PCB (dont mind the raspberry pi being a neon green)
<img width="330" alt="image" src="https://github.com/user-attachments/assets/329870d0-676f-4dce-892c-88122e587eff" /> 
<img width="330" alt="image" src="https://github.com/user-attachments/assets/9d29fcaf-92b4-4c62-9225-2a479278c12b" />
<img width="330" alt="image" src="https://github.com/user-attachments/assets/07908aa8-9610-4414-a34f-51c2247d29db" /> <br/>

### Switch PCBs
<img width="330" alt="image" src="https://github.com/user-attachments/assets/db938bbd-287b-4969-8169-cb4e5bc37124" />
<img width="330" alt="image" src="https://github.com/user-attachments/assets/8459273b-3e27-4104-b182-b5a7244f61bb" />
<img width="330" alt="image" src="https://github.com/user-attachments/assets/bf4dd4e9-b2a3-428f-bba7-e98d4ee9c291" /> <br/>

### Wiring Diagram
<img width="600" alt="image" src="https://github.com/user-attachments/assets/791c785f-159f-4cee-aa85-9e1cd2803449" /> <br/>

## BOM
| Item  |  Purpose | Price | Source |
| ------------- | ------------- | ------------- | ------------- |
| SUNLU Gold PLA Filament | Filament for the case | $19.99 | Amazon |
| Switch PCBs  | Houses the switches in the rings | $5.20 | JLCPCB |
| Center PCB  | Holds the RP2040 and connects to the PC | $2.00 | JLCPCB |
| Yellow 26 AWG Wire | Holds the switches and wires to the center | $3.57 | Aliexpress |
| Outemu Blue Switches | Switches to detect user input/presses | $0.99 | Aliexpress |
| RP2040 Microcontroller | Communicates to the computer, detect switch presses | $2.56 | Aliexpress |
| 3D Printer | Manufactures the keyboard case | Owned |  |
| Soldering Iron | Assembles the PCBs, can weld case to seal cracks | Owned |  |
| Keycaps | Makes switches more comfortable to use | Owned (printing |  |
| Cable | Allows connection between RP2040 and PC | Owned |  |
| Super Glue | Secures parts of the case to each other | Owned |  |
| M3 Screws (6mm, 10mm) | Allows for PCBs to be attached to the case | Owned |  |
| ------------- | ------------- | ------------- | ------------- |
|  |  |  | **Subtotal: $34.31**  |
| Amazon: $28.28 | JLCPCB: $18.81 | Aliexpress: $11.74 |  **Total (tax + shipping): $58.83** |

## additional notes and whatnot
* The case is costs around **466.37** grams of filament, and my current spool of black PLA is running really low (<100 grams left)
* The case will be assembled inside-out (starting from the center, threading the wires through the appropriate connectors before permanently attaching PCBs/ring sections
* JLCPCB is used instead of PCBWay due to the $20 coupon announcement to save costs by Hack Club HQ
* The macropad will be programmed via QMK or KMK and after the macropad is built

**special thanks**
* *Adedayo Adeleke* on Slack for giving me some microcontroller recommendations early on
* *Atrocious* on Slack for giving me a rundown on how to add 3D models to the PCB previewer in KiCad
* My friends and the many people who liked my work and encouraged me to continue working on the absolute clusterfuck of Fusion
* Special thanks to Hack Club and the people behind Highway for making this possible :D

**Inspirations** <br/>
* The indie game *ULTRAKILL*, specifically the angelic enemies named *Virtues* and the upcoming FRAUD update
* The Roblox game *Block Tales*, specifically the final boss of Demo 4, *The Ancients*

<img width="300" alt="angel" src="https://github.com/user-attachments/assets/2648a13b-9429-4980-a22e-8d41d4260295" /> <br/>
The angel is also called bobby :)))) <br/>







