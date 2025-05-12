RCJ2024-Soccer-PCBs
This repository contains all the custom PCB designs created for my RoboCup Junior 2024 soccer robot. The robot features a fully custom electronics stack built from the ground up, focusing on simplicity and reliability.

What is this?
In RCJ 2024, me and 3 other students decided to join the RCJ Soccer Open. I took the task of designing the electrical system. I designed and assembled 2 custom-made dual-layer printed circuit boards for our robot.

PCB 1 (Lower PCB)
This PCB handles line detection (using 16 TCRT5000 IR sensors accompanied by resistor arrays to drive the LEDs and bias the signals) and motor driving (using 4 VNH5019 carrier PCBs from Pololu).
It also has a 40-pin dual-row IDC slot for an interconnect ribbon that links it to the other board.

PCB 2 (Upper PCB)
This PCB handles the robot control system. It has an Arduino Mega2560 Pro board embedded into it, power regulators, decoupling capacitors, and a linear solenoid boost and drive circuit.
It also interfaces with an OpenMV Cam H7+ over UART.
For cross-robot communication, it uses a Bluetooth HC-05 module.
We decided to use an off-the-shelf ESC (BlueRobotics Basic ESC R3) due to manufacturing constraints that prevented us from designing our own.

Further Info
Design Software: Altium Designer 21

Board Stack: Dual-layer

Fabrication: Nori Solutions
