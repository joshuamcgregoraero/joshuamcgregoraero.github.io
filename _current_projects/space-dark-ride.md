---
title: Gravity Themed KUKA Arm Dark Ride
date: 2026-05-07
excerpt: A Full Boar Dark Ride Simulation
tags: [Autonomy, Robotics, Controls, Theme Park, Ride]
status: In Progress
---

## Overview
This ride will be a complete overview of a ride experience from start to finish. I intend to model the entire ride sequence and controls in TwinCAT and Ignition Maker.
Once that is completed, I will make POV and off-ride videos in Maya from accurately modeled SolidWorks models.
I will attempt to conduct force simulations on the ride vehicle and the riders to compare them with the ASTM F24 standards.

## Key Contributions
- Themed entertainment industry level controls
- Maya animation
- Force Simulation
- PLC Setup

## Tools
TwinCAT PLC, Maya, SolidWorks, Ignition Maker, ANSYS


## 06/10/2026 Update Post #1
I have already learned so much about these processes from just this first month of development. It has been a bit of a struggle and learning curve getting used to three new programs all at once, as well as making a layout for this attraction.
Not coming from an Electrical, Software, or Computer Engineering background, I have had to put in a lot of extra work, but I am very happy with this work and field. Along with learning TwinCAT, IgnitionMaker, and Maya, I have had to learn a 
whole handful of new regulation texts and guidelines. To be honest, given my naivety, I thought that attractions only followed ASTM F24, but I completely forgot that the control software and formatting have regulations.
I still haven't figured out how to commit changes to GitHub from TwinCAT, but trust me, it's looking pretty good so far. I have implemented three different actual PLCs, along with one simulation PLC to mock the attraction. I chose to split
the PLCs to emulate real-world conditions. Having the three PLC tasks run through a single PLC would mean that the safety systems and show logic share a single cycle speed, and the show logic does not need to run at the same speed as the safety logic.
If the show logic were to fail, it would also cause the safety system to fail, which is unnecessary and can increase downtime. Given how TwinCAT works, to my current knowledge, if all of the systems were to run through a singular PLC, then if there were to be a fault near the top of the program when the code is running towards the middle, it will not be caught until the program gets back to it at the next cycle. For safety systems where life is at risk for either serious injury or death, that is not acceptable.
I changed the theme to be gravity-focused, specifically in a lab setting. I want the ride narrated or guided by two scientists whose characters I have not quite figured out yet. I would like it to be a bit more on the light-hearted side and have the characters be similar to Phil and Lem from "Better Off Ted", or like Honeydew and Beaker.
The ride will start with guests boarding a seemingly hovering ride vehicle powered by their newest invention, which is some form of electricity or field-sensitive gravity fluid. The ride is then narrated by the scientists as they guide you through their lab facility, growing increasingly destructive as you go, culminating in the lab operator speeding up the guests' tour so they "smash" through a wall to reach the gravity-well test room. In this room, there will be windows that reveal the two scientists as animatronics who then open the floor beneath the riders, where they test the strength of the fluid. As it begins, the fluid holds, but a power outage or spike can cause it to go out of control, and the ride drops using a drop track. The operators then sound panicked as the ride vehicles shoot backward into a hallway where massive Pepper's ghosts create an out-of-control field effect around the riders as they traverse through the destroyed lab. All the experiments they saw earlier are now destroyed or scattered as the riders experience the more intense parts of the attraction. The ride then culminates in the guests disembarking at a different part of the lab, as the scientists are very apologetic. 
I want to incorporate an inversion in some way, but figuring out a comfortable way to do so has so far proven difficult.
Until next update,
Joshua
