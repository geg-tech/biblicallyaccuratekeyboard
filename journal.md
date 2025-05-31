---
title: "The Biblically Accurate Keyboard"
author: "egg_splats"
description: "Making a biblically accurate angel go click and clack"
created_at: "2025-05-17"
---

# welcome to da journal :)
(fyi dates are in mm/dd/yy cuz 🦅🇺🇸)

## 5/17/25
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
<img width="300" alt="sticky note sketch" src="https://github.com/user-attachments/assets/46cad23b-449f-4359-9bf7-2a51c7a1b3b9" />  
time spent: ~0.5 hours

## 5/18/25
second entry ahhh

This morning I hopped on and decided to start on how i wanted the PCBs to look like. I made a preliminary model of what the keyboard should look like, as well as some research on
possible microcontrollers.
* currently im thinking of using a rp2040-ZERO microcontroller due to the small size and large amounts of pins (20 switches from what i counted), possibly could also use a larger microcontroller like an esp32 from what i read (credit to Adedayo Adeleke on slack for telling me about the rp2040-zero)  
* the microcontroller could be located in the center of the angel, with the outer pcbs containing the switches being wired through the supports using copper contacts and soldered on wires  
* could also use flex pcbs or ribbon cables to manage the wiring more efficiently, though im completely new to them  
<img width="450" alt="preliminary 3d model" src="https://github.com/user-attachments/assets/0f148203-d7e6-4ea2-91c6-18fe6a05b707" />  
<img width="300" alt="possible wiring" src="https://github.com/user-attachments/assets/59eb3f14-7ae9-4e62-b8c8-4e959fd868d7" />  

>sometimes its not about the ergonomics, batman...
time spent: ~2 hours

## 5/23/25
5 days later from the second entry but we ball (too busy being sleepy and playing balatro)

I didn't get much done today since I was on call with friends for most of my time after school, but I managed to create a type of "testing platform" for the wiring for my keyboard.
Currently, I'm using a Raspberry Pi Pico WH and push buttons from my old Sprig to simulate the keyboard, but couldn't get it to work (probably due to me uploading the firmware wrong
and/or apple not accepting it as a keyboard, xd)

I also want to remake the preliminary model of the keyboard, since it doesn't look much like the biblically accurate angels depicted before (the rings being too large, the center being too small, etc.)  
<img width="500" alt="quick lil prototype" src="https://github.com/user-attachments/assets/c3731413-0c31-4b87-a3b6-5969899324e4" />  
time spent: ~2 hours (building prototype and bumping my head into the firmware-shaped wall)

## 5/24/25
IT WORKS!!!!!!!!!!!!!! (and by it the prototype)

I tried finagling with raspberry pi pico code found on adafruit and the hackpad website, but eventually got it working with the QMK Keyboard Configurator using the adafruit/pico-pad configuration.  
I plan to change up to code the keyboard by myself for an easier time tweaking the keyboard, but this currently shows that my wiring idea for the core microcontroller and outer PCBs works.  
<img width="500" alt="the prototype works (in wiring)" src="https://github.com/user-attachments/assets/c85f3855-ccf2-48d3-95b9-c5ecbdd6d3c2" />  
Next should hopefully be another remodel of the current design, followed by PCB design and the first iteration of the keyboard!  
time spent: ~1 hour

## 5/29/25
got a lil carried away with the prototype and made it into a tiny breadboard micropad 🐈‍⬛ (even made tiny little keycaps for the buttons)  
thankfully school is out in florida so its time to LOCK IN  
  
ideas and changes:
* The rings/center should be made of two shells that come together for ease of assembly/printing; the rings are to be made into halves, and then possibly made into quarters to fit on my A1 Mini  
* Ring sections could be connected via gluing, assisted with pins or notches for alignment  
* The outer ring is an octogon and houses ~22 switches, while the inner ring is a hexagon and houses ~12 switches (may vary since i also plan on making custom keycaps for the space/enter/shift/esc keys with the same angelic theme)  
The model is currently using a placeholder board from KiCad, but the size of the board shouldn't really change when I remake it (good)<br/>

<img width="625" alt="fresh and brand spankin new design woo" src="https://github.com/user-attachments/assets/f4f3b7cb-ad6b-4a02-8638-0452353e4167" /><br/>
also gave the fella some eyes :)))))<br/>
time spent: ~3 hours modeling and figuring out how to make a dodecahedron

## 5/30/25
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




