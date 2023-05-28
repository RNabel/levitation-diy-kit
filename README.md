# Magnetic levitation kit instructions

## Introduction
This page outlines how to assemble the [Alibaba](https://www.aliexpress.com/item/4000905874457.html) [magnetic](https://www.aliexpress.com/item/1005004188246953.html) levitation / Levitron DIY kit [0], because it comes without instructions. This is a basic soldering project that takes an afternoon to complete even when you have little soldering experience.

The best existing instructions are this [image](https://github.com/RNabel/levitation-diy-kit/assets/10717566/fa132d55-bff8-4aa4-b29e-f1e5fbe1550c) that is included in some listings, and this [fast-forwarded 720p video](https://www.youtube.com/watch?v=-8alDzQ5_Jw) (with much confusion in the comments).

# Rough instructions

Disclaimer: I'm not an electronics expert, so some of this may be wrong.

## Installing the lower section
For reference: 2 pictures of the lower half with a few components installed, [image 1](https://github.com/RNabel/levitation-diy-kit/assets/10717566/a0a678fb-8a05-4e8f-b52a-f18396bb1cf2),
[image 2](https://github.com/RNabel/levitation-diy-kit/assets/10717566/2410a874-ffe3-49e0-9bd6-eacd2e06b96f).

If you're new to soldering: Place some of the components on the top of the board, secure them with Blutack or similar to keep the components in place when turning the board upside down and then solder the pins, then cut the excess pins and repeat. I'd recommend using something to hold your board while soldering (e.g. a "helping hand", or something like [this](https://www.aliexpress.com/item/1005005476494763.html)).

1. **Resistors**. They go in these markings <img src="https://github.com/RNabel/levitation-diy-kit/assets/10717566/26a5b00e-0767-467c-8529-23a43faf0b54" alt="Screenshot 2023-05-28 175307" width="40">. This part is simple: you just need to identify the resistors by their color coding or the labelling in the kit. All resistors came correctly labelled for me, but if you want to double-check there's a wikiHow on [how to identify them](https://www.wikihow.com/Identify-Resistors).

2. **Transistors**: There are 2 types, B772 and B882 both look like black boxes with 3 pins coming out. These go in the boxes labelled B772/B882 respectively, with the side with the text facing up, away from the board. I bent the pins directly against the housing, which resulted in them roughly fitting into the boxes.

3. **Components with different-length pins**: Some components that have different pins lengths - the shorter pin is the negative side. The board markings for these are round and have a shaded area next to one of the holes, which indicates the negative side, *shorter* pin side:
![Screenshot 2023-05-28 182223](https://github.com/RNabel/levitation-diy-kit/assets/10717566/ced7103f-fd6b-41db-8009-b9a81b467158)
The black, cylindrical 220 uF capacitors also have a line on the body next to the negative side.

4. **104/105 capacitors**: These can go into the board either way around. Also note that the components look the same but the board markings are very different, not sure why.

5. **IC chips**: i.e. the chips with many pins, have a nook at one end of the housing that should match the nook marked on the board (the nook on the housing and board will be on top of each other when installed)

6. **Potentiometers**: i.e. the blue boxes labelled "Baoter 3296", are installed text up, with pins bent at the housing. The screws on the potentiometers control the magnetic field on top of the device, so will be used to calibrate the magnetic field later.


## Installing the upper section

1. **Electromagnets**: The inner ring of eletromagnets (the copper-coloured coils) have two wires coming off it: the one coming from the middle of the top of the spool go to the board connectors labelled `1` (i.e. A1/B1/etc)
2. **Hall sensors**: ([wiki](https://en.wikipedia.org/wiki/Hall_effect_sensor)) the three components between the electromagnets, marked H1/H2/H3. These are super important:

    1. Install H1/H2 such that the housing is about 1CM above the board, roughly half way of the height of the copper coloured coils.
    2. The H3 hall sensor needs to be bent by 90 degrees, so that the the text side of the housing faces straight up, away from the board. I bent the pins directly at the housing, but there's enough space to bend the pins slightly away from the housing. The H3 housing should be at the same height as the H1/H2 hall sensors.
    3. **NOTE**: The hall sensors detect the magnetic field of the floating magnet, so if they're not straight, the floating magnet may not float well or at all.

## This thing gets pretty hot
... especially the black transistors: don't keep this plugged in without some supervision. I'm planning on sticking some small heatsinks on the transistors.

## Calibrating
2 parts are responsible for calibration: a) the small blue boxes on the bottom board, b) (I think) the pin pairs under the top board that are angled away from the board.

There seem to be two ways to calibrate the board:
1. The "let's do this live" method of: basically switch it on and calibrate the magnetic field until the magnet is stable
    
    - install the black connectors to the angled out pin pairs on the top board (as in the pictures of the finished board above)
    - connect the two boards
    - plug into power
    - then carefully take the big round magnet and float it over the top board until the blue light engages
    - you will (probably) feel the magnet being pulled in one direction
    - use the screws in the blue boxes to adjust the magnetic field. Each box has a little arrow next to it that indicates which direction the screw moves the magnetic field. There are matching markings on the top board.
    - Repeat until the magnet is stable. This is what the video linked at the top does.

2. (didn't try this) Similar to above, but, roughly, using Ammeters connected to the angled-away pins on the top board, move the floating magnet 1.5CM above the center of the top board and turn the screws until the Ammeters read 0. This is discussed in the instruction-image linked at the top.


# Pictures of the finished project
Top board, upper side:
![image](https://github.com/RNabel/levitation-diy-kit/assets/10717566/d0540d28-861f-4c54-a096-cb8135e70de0)

Top board, focus on the hall sensors (middle three components):
![image](https://github.com/RNabel/levitation-diy-kit/assets/10717566/8381b3ac-ea73-4030-b1b1-b0d5c2f44d2a)

Top board, underside:
![image](https://github.com/RNabel/levitation-diy-kit/assets/10717566/6cda768f-6579-4e19-908e-fe391cc31155)

Lower board, upper side:
![image](https://github.com/RNabel/levitation-diy-kit/assets/10717566/75b982e5-8503-4928-8f26-c7cad7756f05)

Lower board, underside:
![image](https://github.com/RNabel/levitation-diy-kit/assets/10717566/9014f36b-83d9-4bf5-83c4-abf70257c6fd)

[0] These are not affiliate links; there are a lot of these listings.
