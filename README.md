# MORPH-Robotic-Hand
### MORPH (Modular Optimised Robotic Hand)
A 3D-printed, tendon-driven robotic hand with a web-based control interface, built as my VCE Systems Engineering Units 3 & 4 major project.

<!-- Add a hero photo of the finished hand here -->
<img width="368.3333333333" height="491" alt="image" src="https://github.com/user-attachments/assets/c92d3e7c-4c75-4d9f-a875-8885336ae235" />

<img width="368.3333333333" height="491" alt="image" src="https://github.com/user-attachments/assets/f4bff2b8-6c40-4644-9e1d-474b7d91e793" />
<img width="368.3333333333" height="491" alt="image" src="https://github.com/user-attachments/assets/f6d21a6c-c0ab-4bb6-903f-9598d62e12fb" />


About the Project

VCE Systems Engineering (Units 3 & 4) is a Year 12 subject in Victoria where students go through the full engineering process, from design brief and research through to design, production, testing and evaluation, to build their own working system as a year-long major project.

MORPH is a 5-fingered robotic hand that's controlled through a web app to perform gestures and grip everyday objects, including an auto-grip function. It was built to a sub-$400 budget, coming in at $223.83.

Tech Used

Hardware


ESP32-S3 Nano as the main microcontroller, running the web server and driving all the servos
Adafruit PCA9685, a 16-channel PWM servo driver
5x 270° servos with analog feedback for tendon contraction in each finger, with the feedback used for the auto-grip function
4x SG90 servos for lateral finger movement
Adafruit USB-C PD board for power delivery
A custom hand-soldered protoboard connecting everything together
3D printed in PLA+ on a Bambu Lab A1, with fishing line acting as tendons and elastic cord providing return tension


Software


Arduino (C/C++) for the ESP32 firmware
HTML, CSS and JavaScript for the web control interface, served directly from the ESP32
Fusion 360 for CAD design
Figma for designing the control interface
Bambu Studio for slicing


Challenges

The first major challenge of this project was getting the tolerances right on the finger joints. If they were too tight the friction stopped the finger moving properly, and if they were too loose the joint became unstable, so I went through several rounds of printing, assembling, testing and reprinting before the fingers moved smoothly. The second major challenge was fitting everything into the hand itself. Since I decided not to include a forearm,, all 10 servos, the microcontroller, the servo driver and the power board had to fit inside the palm and a small electronics bay on the back, without making the hand too bulky or ruining how it looked.

Photos


The complete portfolio, including the design brief, research, calculations, CAD, production process, testing and full evaluation, is included in this repo:
