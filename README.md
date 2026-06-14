# Autonomous Rover V2
This is a WIP version 2 of my [autonomous face tracking rover](https://github.com/theejebu/Autonomous-Face-Tracking-Rover). This is not a tutorial, but documentation on how I made it. 

### Components
- 4 mecanum wheels
- 4 DC motors
- A chassis for the components to lie on
- 18650 battery (mine was rechargeable)
- ESP32-S3-CAM
- HC-SR04 distance sensor
- Some extra jumper wires
- Some LEDs

### Introduction
To build this project I wanted to challenge myself and learn different skills, like soldering, 3D designing and PCB design. Compared to my first version of this robot, which could only track and move to faces, I wanted this to be able to detect people, other objects and also have the ability to scan for them. My previous design also didn't have a distance check which is what I wanted to implement using a distance sensor. Additionally, instead of Haar Cascade to detect faces, I would use YOLO on my PC to detect various objects and send the data to my ESP32 over Wi-Fi.

### Construction 
To make the autonomous rover, I first dissasembled a mecanum based RC car, which provided the wheels I wanted. (Image below)

<img width="199.7" height="226.8" alt="IMG-20260524-WA0038" src="https://github.com/user-attachments/assets/72ca8c73-fbd1-47df-a8f6-2572b97ce71f" />

The wheels did not fit onto my DC motors so I had to model an adapter. 

It was in this part of my project where I decided I make my own custom PCB with additional features. This would mean I would have to learn how to make a PCB, and also 3D print a chassis to hold the new components. I will still use the motor driver and keep the other features of my idea as part of the PCB.

### PCB Design
I had a few ideas for the PCB. 
It would:
- Have a distance sensor
- Have female header pins for me the plug the ESP32 into
- Have male pins for the ESP32 to connect to the driver module
- And have 3 LEDs

The 3 LEDs would be diagnostics:
- Nothing detected - Red one lights up
- Something detected and action in progress - Yellow one lights up
- Something detected and action completed - Green one lights up
