# Autonomous Rover V2
This is a WIP version 2 of my [autonomous face tracking rover](https://github.com/theejebu/Autonomous-Face-Tracking-Rover). This is not a tutorial, but documentation on how I made it. 

### Components
- 4 mecanum wheels
- 4 DC motors
- A chassis for the components to lie on
- 18650 battery (mine was rechargeable)
- ESP32-S3-CAM
- Some extra jumper wires

### Construction
To make the autonomous rover, I first dissasembled a mecanum based RC car, which provided many of the key components provided above. (Image below)

<img width="1997" height="2268" alt="IMG-20260524-WA0038" src="https://github.com/user-attachments/assets/72ca8c73-fbd1-47df-a8f6-2572b97ce71f" />

Next I wanted to learn how to crimp dupont headers onto the wires on the battery connector, this was vital to be able to attach it to the motor driver. 
My crimping was not very successful so to keep the electrical connection secure, I reinforced it with electrical tape. (Image below)

<img width="2040" height="1530" alt="image" src="https://github.com/user-attachments/assets/a7a093be-4156-4b49-994f-0cd9463b8b0f" />

It was in this part of my project where I decided I did not want to use the motor driver, but instead make my own custom PCB with additional features. This would mean I would have to ditch part of my construction and start almost fresh. 
