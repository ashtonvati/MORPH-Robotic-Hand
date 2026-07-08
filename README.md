MORPH-Robotic-Hand
MORPH (Modular Optimised Robotic Hand)

A 3D-printed, tendon-driven robotic hand with a web-based control interface, developed as my VCE Systems Engineering (Units 3 & 4) major project.

<img width="368.3333333333" height="491" alt="image" src="https://github.com/user-attachments/assets/f6d21a6c-c0ab-4bb6-903f-9598d62e12fb" />

<img width="368.3333333333" height="491" alt="image" src="https://github.com/user-attachments/assets/c92d3e7c-4c75-4d9f-a875-8885336ae235" />

<img width="368.3333333333" height="491" alt="image" src="https://github.com/user-attachments/assets/f4bff2b8-6c40-4644-9e1d-474b7d91e793" />

About the Project

VCE Systems Engineering is a Year 12 subject in Victoria where students complete a year-long engineering project, following the full design process from research and concept development through to manufacturing, testing and evaluation.

For this project, I designed and built MORPH, a five-fingered robotic hand capable of performing gestures and gripping everyday objects through a custom web interface. The hand also features an auto-grip mode that uses servo feedback to detect when an object has been grasped, allowing it to securely hold objects of different sizes.

The project was completed for $223.83, well under the allocated $400 budget.

Tech Used
Hardware

The system is built around an ESP32-S3 Nano, which hosts the web interface and controls all motor movement. A PCA9685 16-channel PWM driver drives the servos, with five 270° servos providing tendon actuation for each finger and four SG90 servos controlling lateral finger movement. Analog feedback from the finger servos is used to implement the auto-grip functionality.

Power is supplied through an Adafruit USB-C PD board, while a custom hand-soldered protoboard connects the electronics into a compact package. The hand itself was designed in Fusion 360 and 3D printed in PLA+ on a Bambu Lab A1, using fishing line as tendons and elastic cord to return the fingers to their resting position.

Software

The firmware was written in Arduino (C/C++), with the ESP32 serving a web-based control interface built using HTML, CSS and JavaScript. Mechanical components were designed in Fusion 360 and all parts were prepared for printing using Bambu Studio.

Challenges

One of the biggest challenges was achieving the correct tolerances for the finger joints. Small changes in clearance had a significant impact on performance, requiring multiple design iterations, prints and assembly tests before the fingers moved smoothly while remaining structurally stable.

Another challenge was packaging the electronics. Since the design intentionally omitted a forearm (to maximise modularity, allowing the hand to be attached to a range of other systems), all ten servos, the ESP32, servo driver and power delivery hardware had to fit within the palm and a compact electronics enclosure on the back of the hand without compromising functionality or appearance.

Engineering Portfolio

The complete portfolio documenting the entire engineering cycle of this project is in this repository
