# CNC Plotter

A computer-controlled device used for drawing or plotting complex designs or patterns on various surfaces such as paper, fabric, and other materials.

### Team Members:
- Aakriti
- Sanju Kumar

### Supervisor:
**Dr. Saurabh Kumar Pandey**  
Professor, EE Dept.  
IIT Patna

**Date:** October 4, 2023

---

## Abstract

With the advancement of technology, the demand for Computer Numerical Control (CNC) plotter machines in Educational Institutions and Laboratories is rapidly rising. CNC (Computer Numerical Control) drawing machines are computer-controlled devices that use automated software to control the movement of a pen or other drawing tool. We have used a pen instead of mechanical tools like drilling, grinding, machining, etc. These machines are used to create precise and intricate designs on various surfaces such as paper, fabric, and other materials. CNC drawing machines have revolutionized the way we create art, design, and engineering products.

---

## Acknowledgements

We would like to express our sincere gratitude to our supervisor, Dr. Saurabh Kumar Pandey, for accepting our project proposal and guiding us throughout the project. Your valuable feedback, constructive criticism, and encouragement were instrumental in shaping this project and bringing it to fruition.

We would also like to extend our heartfelt thanks to our friends for their invaluable support in recording the demonstration videos and making this project a fun and memorable experience. Their enthusiasm, creative ideas, and technical expertise made this project all the more enjoyable and rewarding.

Finally, we would like to thank Tinkerer’s Lab for providing us with the resources, facilities, and opportunities to pursue this project. This project would not have been possible without their support and encouragement.

---

## Contents

1. [Hardware Assembling](#hardware-assembling)
   - [Hardware](#hardware)
   - [The Circuit](#the-circuit)
2. [Methodology](#methodology)
   - [Main Parts of CNC Plotter](#main-parts-of-cnc-plotter)
   - [Block Diagram of Process](#block-diagram-of-process)
3. [Software](#software)
   - [Uploading the Code](#uploading-the-code)
   - [Making Our Own G Code File](#making-our-own-g-code-file)
   - [Sending G Code to CNC Machine](#sending-g-code-to-cnc-machine)
4. [Conclusion](#conclusion)
   - [Applications](#applications)
   - [Advantages](#advantages)
   - [Disadvantages](#disadvantages)
   - [Conclusion](#conclusion-1)

---

## Hardware Assembling

### 1.1 Hardware

The following hardware components were used to construct the CNC machine:

- 2 x NEMA 17 Steppers 1.8 Degree Step 12V Torque more than 4kg/cm
- 2 x 8mm, 10mm Stainless Steel Smooth Rods
- 2 x LM8UU 8mm, LM10UU 10mm Linear Bearings or SC8UU 8mm, LM10UU 10mm Linear Bearings
- 4 x SK8 8mm, SK10 10mm Rod End Support
- 4 x LM10UU 10mm Linear Bearings or SC10UU 10mm Linear Bearings
- 2 x 20-Tooth GT2 Pulleys
- 12 x F623ZZ Bearings
- 1 x Micro Servo SG90
- 1 x Arduino UNO
- 1 x CNC Shield V3
- 2 x Pololu Step Sticks A4988 Stepper Driver
- 1 x GT2 Belt (3 meters long)
- 1 x Hard Wood Ply 50cmx60cmx1.5cm
- Multiple screws with nuts
- 1 x Wire 5m
- 1 x SMPS 12V 5A
- 1 x Soldering Wire
- 1 x Solder
- 1 x Jig Saw
- 1 x Jig Saw Blade for wood cutting
- 1 x USB Wire
- 1 x PEN

### 1.2 The Circuit

After assembling the hardware, we built the circuit and tested the stepper motors (X and Y axis). The breadboard circuit schematic is shown below. In the next step, we tested the X and Y axes. If the steppers didn’t work properly, we found the correct working combination by changing the cables between them and the L293D IC.


![1](https://github.com/user-attachments/assets/c108eda5-5445-442e-a926-fe80dcebb33d)


---

## Methodology

### 2.1 Main Parts of CNC Plotter

The Mini CNC Plotter Machine works by converting G-code designs into movements via an Arduino, stepper drivers, a CNC shield, and stepper motors that rotate a lead screw. We focused on maintaining the lowest cost for our project and designed a simple construction. The setup of the machine is flexible, making it easy to transport and quick to maintain.


![2](https://github.com/user-attachments/assets/7e6f2e13-9d38-4f05-86fe-19fa532af26c)


### 2.2 Block Diagram of Process

In this project, an Arduino microcontroller is used, which can be easily interfaced with a PC. The G-Code from the computer is fed to the control unit (Arduino), which controls the stepper motors and the servo motor.


![3](https://github.com/user-attachments/assets/9bccb9ad-9ca8-46d5-b487-dfc71bdf2e7c)



---

## Software

### 3.1 Uploading the Code

We used the Grbl library, which accepts standards-compliant G-Code to draw various shapes such as arcs, circles, and helical motions. It also includes full acceleration management with look-ahead to deliver smooth acceleration and jerk-free cornering. The program is uploaded to the Arduino using the Arduino IDE.

### 3.2 Making Our Own G Code File

To create G-code files compatible with this CNC machine, we used the Inkscape software. Inkscape is used by design professionals and hobbyists worldwide for creating a wide variety of graphics such as illustrations, icons, logos, diagrams, maps, and web graphics. It uses the W3C open standard SVG (Scalable Vector Graphics) as its native format and is free and open-source software.

The image we wanted to draw was uploaded to the Inkscape software and then exported as a G-code file, which was used to send commands to the CNC machine.

### 3.3 Sending G Code to CNC Machine

The Universal Gcode Sender (UGS) is a software application used to control CNC machines through G-code commands. First, it is connected to the Arduino, and then the G-code file is uploaded. In the next step, the UGS ‘run’ command is executed, which sends each G-code line one by one.

---

## Conclusion

### 4.1 Applications

CNC drawing machines have a wide range of applications, including:

- **Art and Design**: Used to create complex and intricate designs on various surfaces such as paper, canvas, and wood. Artists use CNC drawing machines to create large-scale murals or detailed sketches.
- **Architecture and Engineering**: Used to create precise blueprints and schematics for architectural and engineering projects, saving time and reducing errors in the design process.
- **Sign Making**: Used to create custom signs with high precision and consistency, particularly useful for businesses that require large volumes of signs, such as retail stores and restaurants.
- **Textile Industry**: Used to create complex patterns and designs on fabrics, such as embroidery or applique, useful for creating custom clothing or other textile products.

### 4.2 Advantages

CNC drawing machines offer several advantages over traditional manual drawing methods, including:

- **Precision and Accuracy**: Ability to create precise and accurate designs with consistency.
- **Speed**: Ability to complete complex designs quickly and efficiently.
- **Versatility**: Ability to work on a variety of surfaces and materials.
- **Reduced Errors**: Less likely to make mistakes or errors compared to traditional manual drawing methods.

### 4.3 Disadvantages

CNC drawing machines also have some disadvantages, including:

- **High Cost**: Expensive to purchase and maintain.
- **Complexity**: Requires specialized training and knowledge to operate effectively.
- **Limited Creativity**: Limited by the designs that are programmed into them, which can restrict creativity.

### 4.4 Conclusion

CNC drawing machines have revolutionized the way we create art, design, and engineering products. They offer several advantages over traditional manual drawing methods, including precision, speed, versatility, and reduced errors. However, they also have some disadvantages, including high cost and complexity. Despite these limitations, CNC drawing machines are a valuable tool for creating precise and intricate designs on various surfaces and materials.
```
