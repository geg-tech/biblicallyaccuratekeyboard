---
title: "The Biblically Accurate Macropad"
author: "egg_splats"
description: "Making a biblically accurate angel go click and clack"
created_at: "2025-05-17"
---

# welcome to da journal :)
(fyi dates are in mm/dd/yy cuz 🦅🇺🇸) <br/>
technically its more like a macropad but shhhhhhhhh 🤫 it doesn't have the same ring to it man

## 5/17/25 - The Start of Highway
>be me  
>wake up  
>highway announcement  
>wtf  
  
First entry into the journal! Today I brainstormed a bunch of ideas on what to do for highway, such as:  
* combat robot that flips onto opponents with a vertical spinner (slam jam)  
* horse racing robots with mash-able "cheer" buttons that have a very small chance to boost the robot forward  
* irl V1 wings from ultrakill  
  
Ultimately, I decided to choose something that is somewhat within my comfort zone of circuit boards and 3d modeling (though I hope to do the other ones someday),
that being a keyboard in the shape of a biblically accurate angel. I chose this idea due to the existing tutorial on hackpad which should be a great 
stepping stone into this project, while also being unique and funnier from the usual, flat micropads (though I'm unsure if this idea would count as a custom or starter project 🗿).
  
I have some ideas on what the keyboard should look like, with the shape of the board most likely looking like the usual orb angel with the revolving rings of eyes.  
<img width="500" alt="angel go clack" src="https://github.com/user-attachments/assets/115d9f0f-bb39-4dbc-8a9d-8685635a11cc" />
<img width="300" alt="sticky note sketch" src="https://github.com/user-attachments/assets/46cad23b-449f-4359-9bf7-2a51c7a1b3b9" /> <br/>

time spent: ~1 hours

## 5/18/25 - Preliminary Designing
second entry ahhh

This morning I hopped on and decided to start on how i wanted the PCBs to look like. I made a preliminary model of what the keyboard should look like, as well as some research on
possible microcontrollers.
* currently im thinking of using a rp2040-ZERO microcontroller due to the small size and large amounts of pins (20 switches from what i counted), possibly could also use a larger microcontroller like an esp32 from what i read (credit to Adedayo Adeleke on slack for telling me about the rp2040-zero)  
* the microcontroller could be located in the center of the angel, with the outer pcbs containing the switches being wired through the supports using copper contacts and soldered on wires  
* could also use flex pcbs or ribbon cables to manage the wiring more efficiently, though im completely new to them  
<img width="450" alt="preliminary 3d model" src="https://github.com/user-attachments/assets/0f148203-d7e6-4ea2-91c6-18fe6a05b707" />  
<img width="300" alt="possible wiring" src="https://github.com/user-attachments/assets/59eb3f14-7ae9-4e62-b8c8-4e959fd868d7" />  

>sometimes its not about the ergonomics, batman... <br/>

time spent: ~3 hours modeling and sketching

## 5/23/25 - Prototyping Electronics
5 days later from the second entry but we ball (too busy being sleepy and playing balatro)

I didn't get much done today since I was on call with friends for most of my time after school, but I managed to create a type of "testing platform" for the wiring for my keyboard.
Currently, I'm using a Raspberry Pi Pico WH and push buttons from my old Sprig to simulate the keyboard, but couldn't get it to work (probably due to me uploading the firmware wrong
and/or apple not accepting it as a keyboard, xd)

I also want to remake the preliminary model of the keyboard, since it doesn't look much like the biblically accurate angels depicted before (the rings being too large, the center being too small, etc.)  
<img width="500" alt="quick lil prototype" src="https://github.com/user-attachments/assets/c3731413-0c31-4b87-a3b6-5969899324e4" /> <br/>

time spent: ~3 hours (building prototype and bumping my head into the firmware-shaped wall)

## 5/24/25 - it worked :D
IT WORKS!!!!!!!!!!!!!! (and by it the prototype)

I tried finagling with raspberry pi pico code found on adafruit and the hackpad website, but eventually got it working with the QMK Keyboard Configurator using the adafruit/pico-pad configuration.  
I plan to change up to code the keyboard by myself for an easier time tweaking the keyboard, but this currently shows that my wiring idea for the core microcontroller and outer PCBs works.  
<img width="500" alt="the prototype works (in wiring)" src="https://github.com/user-attachments/assets/c85f3855-ccf2-48d3-95b9-c5ecbdd6d3c2" />  
Next should hopefully be another remodel of the current design, followed by PCB design and the first iteration of the keyboard! <br/>

time spent: ~2 hours

## 5/29/25 - Remodel #1
got a lil carried away with the prototype and made it into a tiny breadboard micropad 🐈‍⬛ (even made tiny little keycaps for the buttons)  
thankfully school is out in florida so its time to LOCK IN  
  
ideas and changes:
* The rings/center should be made of two shells that come together for ease of assembly/printing; the rings are to be made into halves, and then possibly made into quarters to fit on my A1 Mini  
* Ring sections could be connected via gluing, assisted with pins or notches for alignment  
* The outer ring is an octogon and houses ~22 switches, while the inner ring is a hexagon and houses ~12 switches (may vary since i also plan on making custom keycaps for the space/enter/shift/esc keys with the same angelic theme)  
The model is currently using a placeholder board from KiCad, but the size of the board shouldn't really change when I remake it (good)<br/>

<img width="625" alt="fresh and brand spankin new design woo" src="https://github.com/user-attachments/assets/f4f3b7cb-ad6b-4a02-8638-0452353e4167" /><br/>
also gave the fella some eyes :)))))<br/>

time spent: ~4 hours modeling and figuring out how to make a dodecahedron

## 5/30/25 - PCB Designed
Redesigned the PCBs for the switches today, that's it really  
More specifically...  
* I added another GND hole to allow the boards to be "chained" to each other through wires going through GND (should dramatically reduce the amount of wires needed for GND)
* ^ i also tested this with the same raspberry pi from the prototype with a chain of breadboard power rails  
* Centered the switches on the board  
* Added a M3 screw hole to the board for easy attachment to the case (I could also hot glue the pcbs to the case if one screw is inadequate but the spacing should be just right for the boards)  
* Added eyes to the back silkscreen because :eye:  
<img width="300" alt="board" src="https://github.com/user-attachments/assets/4dafe2d0-d5f6-4fc0-b169-f8b6a4873054" />  
<img width="300" alt="board2" src="https://github.com/user-attachments/assets/c564524e-37f0-42d8-b2b4-92018d14c87d" />  
<img width="300" alt="board3" src="https://github.com/user-attachments/assets/fd07ff2b-1eae-4b39-9539-5955a8f63dfc" /> <br/>

time spent: ~2 hours redesigning and routing

## 6/5/25 - Started CAD on the case
damn its already june 😔 <br/>
  
Today (after a long break of block tales with friends) I started modeling the 3d printed parts of the keyboard. <br/>
I made the sections of the rings and found out that it would most likely be easier to print each side of the rings individually, instead of trying to meddle with supports and oddly placed holes if I printed the rings in entire sections. <br/>
I also added small slots on the sides of the sections to aid in alignment and gluing, since it would most likely be very difficult to glue and keep together an entire polygon of 3d printed parts lmao <br/>
<img width="600" alt="fusion design of one of the 6 inner sections" src="https://github.com/user-attachments/assets/5a5c5829-cb2e-4c0f-8b0a-acae6cbfe306" /> <br/>
Once I had the sections made, I printed out two pieces to test the tolerances. The parts fit together nicely, but they left a large (and honestly pretty ugly) gap between the two sections. <br/>
I did some research on how to fix this, and found out that I can seal up the gap and join the parts using spare filament and a soldering iron. After some time messing around, I managed to seal the gap in a way that looked good enough <br/>
<img width="400" alt="fusion design of one of the 6 inner sections" src="https://github.com/user-attachments/assets/9b303264-8b6a-4c00-b85a-8c27bb588949" /> <br/>
btw ignore the crack i was testing how strong the bond was (it was strong) <br/>

time spent: ~1 hour printing, ~3 hours modeling and learning how to weld plastic

## 6/6/25 - Modeled Connectors
oh hey double sixes <br/>
  
Today I modeled the connector pieces that would hold the rings together, as well as the corresponding sections of the rings that attach to the connectors <br/>
Initially, I made the connector similar to those made by organic generative design programs like the one in Fusion 360. I spent a good while wrangling 3d sketches in Fusion, and after modeling and printing it, the design *literally exploded* the moment I applied shear to it lmfao
> (generative design not as in text prompting an AI model but the ones you would see making those weird bony-shaped parts that are supposedly super tough in aerospace applications and stuff) <br/>

<img width="200" alt="GONE. REDUCED TO DUST. 💔" src="https://github.com/user-attachments/assets/dd454841-2f31-40ae-8405-837378ebfff6" /> <br/>
I chose the bony shape of the connector initially since it looked cool due to the organic shape, as well as having holes for wires to feed through for the inner ring of switches, but quickly learned that wasn't an option. In return, I remade the connector in a much more boring fashion (literally just a cylinder with a rectangular hole) 😔 <br/>
<img width="322" alt="boring" src="https://github.com/user-attachments/assets/2c098253-e4e9-4d29-9222-d939c9cfa761" />
<img width="322" alt="fancy" src="https://github.com/user-attachments/assets/32fa6125-e28b-4e3d-8941-975b8ea11947" /> <br/>

time spent: ~1 hour designing, ~1 hour printing

## 6/8/25 - Created the BOM
This morning I decided to get a headstart on making my bill of materials (totally not procrastinating on designing the core 🦨) <br/>
<img width="600" alt="image" src="https://github.com/user-attachments/assets/238f3873-f71b-4dc7-b2cb-614c0ca02c01" /> <br/>
I considered making another custom PCB to house the microcontroller and the wires, but then realized that it would be be infinitely times cheaper to mount everything to a perfboard inside the core since it most likely won't be visible in the final product (I forgot who mentioned using a perfboard on the Slack but credit to you, I remember their message being something like using a protoboard for a radio of some kind) <br/>
  
I also believe that using a perfboard will allow for greater flexibility in my design, especially if I want to add extra features like LEDs, but may also have the drawback of being annoying to design around/assemble compared to a custom PCB. <br/>
Currently, almost all the prices are not accounting for tax + shipping, but should be a good start (expect the BOM to be nearly finished near the end of the day, its morning as of writing lol) <br/>

***uh oh future update from the afternoon***
Turns out adding another PCB to the PCBWay order doesn't cost nearly as much as I expected! (5 dollars more and an extra dollar to shipping if included with the switch PCBs) <br/>
While a perfboard *would* still be cheaper by a margin of a few dollars, I had no luck finding the exact hole dimensions for the perfboard I found on Aliexpress, which would make designing the core of the keyboard MUCH harder than it needs to be (not to mention the time needed to learn to assemble a perfboard and the general build quality) <br/>

so yeah pcbs are back on the menu <br/> 
i also picked up some m3 screws and a bottle of super glue on my way to the hardware store today so there's that too :3 <br/>

time spent: ~2 hours of researching/filling out BOM

## 6/9/25 - Designed the core PCB and (parts of the) case
teehee funny 69 date <br/>

Today I designed and finished the PCB that will hold the RP2040 and wires from the switches. <br/>
The center of the PCB holds the RP2040 microcontroller, which is connected to multiple holes that will receive input from the switches on their own PCBs. The holes also contain GND to string throughout the switch PCBs. While choosing the footprints, I realized that I had an odd number of pins heading out (split between 12 and 11 pins on each side), so I also added a hole for 3.3V in case if I ever want to add something extra like an LED as a power light or aesthetics. <br/>
<img width="300" alt="uhh" src="https://github.com/user-attachments/assets/74958dd2-64ca-4f29-983a-4c67b27c1fc6" /> <br/>
The board also looked pretty *empty* and *sad* so I threw in some inside jokes from my friend group, as well as my school's Hack Club logo (made by yours truly :3). On the back I also made a picture of the core of the macropad, using Fusion 360 to create the dodecahedron and Figma to create a solid outline and the custom text for the macropad.<br/>
<img width="300" alt="image" src="https://github.com/user-attachments/assets/32c51e87-1be6-4f77-b3b5-21a02acb605a" />
<img width="300" alt="image" src="https://github.com/user-attachments/assets/25c78ffc-654e-43fb-9d30-471b52df332a" /> <br/>
i also affectionately named the macropad bobby <br/>

After designing the core PCB, I got to work making the case for the center of the macropad. I remade the dodecahedron so I could separate it into halves, making sure the thickness did not extend perpendicular to the faces so the halves could be interlocked with each other. After that, I added a 0.6 in. wide hole to fit the connectors from the rings. <br/>
<img width="300" alt="image" src="https://github.com/user-attachments/assets/c40b4865-0ef0-4a87-a685-2e67689e16c0" /> <br/>
Once I got the PCB imported into the Fusion file, I quickly made the screw holes and supports to hold the PCB, as well as a cable hole to connect the PCB and microcontroller to the computer. <br/>
<img width="200" alt="image" src="https://github.com/user-attachments/assets/ec1c41fc-c6c8-4525-add1-4f327ee3d87d" />
<img width="200" alt="image" src="https://github.com/user-attachments/assets/412b66d9-c0e0-43a8-97bb-03b158edf111" /> <br/>
Hopefully tomorrow I can start finishing up the CAD for the center and start working on the aesthetics side of the CAD, such as designing custom keycaps, eye plates that will slot into the sides of the dodecahedron, and polishing up the CAD models. <br/>
time spent: ~4 hours in PCB design and drawing art, ~2 hours modeling

## 6/11/25 - Core CAD model finished and completed BOM
I just finished the CAD model for the center, nothing else really <br/>
heres a picture i guess <br/>
<img width="200" alt="image" src="https://github.com/user-attachments/assets/ff6b0d59-f422-4003-9d4c-1001702b9de5" /> <br/>

I also spent some time going over and reviewing my bill of materials, taking out parts that I didn't need (M3 screws and super glue) and rechecking parts. For example, the PLA filament in my BOM recently went on sale for ~$2 less, which I should take advantage of. I also swapped over from PCBWay to JLCPCB, due to the recent announcement of a 20 dollar coupon for PCBs and my PCBs costing just under $20. <br/>
<img width="700" alt="image" src="https://github.com/user-attachments/assets/2cc4c571-31f3-435b-b5f0-47ca5c14b0e4" /> <br/>
time spent: 30 minutes finishing CAD, 1 hour finishing bill of materials

## 6/12/25 - Modeled custom keycaps
Today I made custom keycaps for the macropad. <br/>
I knew that the microcontroller I was going to order (and the current setup of the switches) weren't going to support all 30 switches in the prototype CAD model, which meant that I had to merge some keys to fit the amount of GPIO pins. Because of this fact, I ended up making 3 different variants of the keycaps, each using up one, two, and three spaces for switches. <br/>

I designed the switches around the models found in hineybush's Github repo (found here https://github.com/hineybush/CherryMX), using the measurements for the keycap stems and adjusting them for my printer's own tolerances and for the general size of the keycaps (18mm x 18mm x 10mm). Other than that, the models for the keycaps are original. I also added designs on top of the keycaps, based around the eyes found on the rings of depictions of biblically accurate angels. <br/>
Overall, I'm satisfied on how they keycaps turned out, but I may also redesign the 2-wide keycap since it the eyes are all skewed compared to the other keycaps. <br/>
<img width="150" alt="1-wide keycap" src="https://github.com/user-attachments/assets/f676b726-3165-4915-8490-10facace62f8" />
<img width="200" alt="2-wide keycap" src="https://github.com/user-attachments/assets/62a4b28e-9a35-413f-a388-053b03c7e943" />
<img width="300" alt="3-wide keycap" src="https://github.com/user-attachments/assets/247904a7-57ef-4fcf-ad7e-ee249dbf8056" />
<img width="500" alt="3d prints" src="https://github.com/user-attachments/assets/ec165efe-9f8f-43bd-bed5-c4a0e09973fc" /> <br/>
Hopefully next should be designing eyes that can be attached to the sides of the center, and then final revisions for submission 🐈‍⬛ <br/>
time spent: ~2 hours designing keycaps

## 6/13/25 - more decorations!!!!! (and failing)
Today I remodeled the 2-wide keycap to have one eye, as well as attempting to create eyes that will be attached to the sides of the center. <br/>
Although the keycap went well (perhaps my favorite keycap out of the three), I struggled to make the eye for the center. At first I went with using the *"Create Form"* tool in Fusion, making a sketch and creating a pipe with it, but soon ran into issues trying to make it "smooth" into the surface. <br/>
<img width="800" alt="image" src="https://github.com/user-attachments/assets/6cb78eb9-8a90-42c1-9e4e-3109fe3ac135" /> <br/>
After that didn't work, I tried using the Fillet tool to make it smooth into the surface, but spent an eternity bashing my head against fillet size errors. In the end, I ended up giving up for the day since it was already pretty late into the night (and the fact that Fusion's rendering was tweaking out). <br/>
but anyways cool keycap :D <br/>
<img width="300" alt="image" src="https://github.com/user-attachments/assets/a373aea7-c70d-469c-b1f3-874778e317e3" /> <br/>
I also realized that the inside parts of the eyes were *really* thin (about 1 pla layer), so I also ended up thickening the keycaps there. <br/>
time spent: ~3 hours modeling

## 6/14/25 - that eye that i hate (finished it)
I finished that damn eye <br/>
I ended up making the eyelids by using a regular extrude command, combined with large fillets to create that smooth shape that makes it look like it is part of the surface. After that, I used a revolve tool to create the eye, as well as the iris. All of the parts in the eye are different parts, with the eyelids and iris planned to be colored gold in contrast to the white of the center/eye. <br/>

I also revamped the ring sections that feature the holes that connect to the center of the macropad, removing the screw holes (idk why i put them there) and adding a cover plate to the outer ring variant. <br/>
<img width="528" alt="new eye rah i hated this part" src="https://github.com/user-attachments/assets/0289ab59-f4ea-49ed-a4cd-628e9badd017" />
<img width="678" alt="ooh cool new sections" src="https://github.com/user-attachments/assets/c978a868-03c6-4940-8eba-62b5835d47a1" /> <br/>

also here's the full peeper with all the modeled cad and stuff added on (too lazy to add keycaps rn so tomorrow) <br/>
<img width="561" alt="image" src="https://github.com/user-attachments/assets/55b573fb-a678-4697-9ea1-8f24cb35da15" /> <br/>
time spent: 2 hours modeling and creating the full CAD

## 6/16/24 - OUGH ITS DONE (the cad)
This morning I colored and added the keycaps to the model I made on the 14th











