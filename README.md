# ECE 528/L - Robotics and Embedded Systems with Lab
**CSU Northridge**

**Department of Electrical and Computer Engineering**

## Motor Control Lab
The Motor Control lab interfaces with the following:

* User LEDs of the TI MSP432 LaunchPad
* Pololu Gearmotor with Encoder - [Product Link](https://www.pololu.com/product/3675)
* Left Bumper Switches for TI-RSLK MAX - [Product Link](https://www.pololu.com/product/3673)
* Right Bumper Switches for TI-RSLK MAX - [Product Link](https://www.pololu.com/product/3674)
* HS-485HB Servo-Stock Rotation - [Product Link](https://www.servocity.com/hs-485hb-servo/)

## Overview
This lab introduces us to different modules within the MSP432 LauchPad. Specifically we worked with SysTick and Timer_A. We utilized the Timer_A module to output PWM signals for our Motor Driver. 
## Componets Used:
* MSP432 LauchPard
* Bumper Switches
* HS-485HB Servo
* Oscilloscope
* Oscilloscope probes
## Analysis and Results:
The first think that we did for this lab was to connect the HS-485HB to the board. After making the proper connections we uncommented certain portions of the code to run, once this was done we used an oscilloscope, with a pin connected to P5.6, for our case we only had one servo so we were not able to capture screenshots for both pins. We used the oscilloscope to check when the servo was at 0 degrees, this was indicated by a red light. And when the servo was at 180 degrees, indicated by a blue light. Once these images were taken we also need to make sure the pulse widths were correct, they were. These images can be found in the [image](/images/) files. Once this was completed we moved onto the Tasks, the first three tasks required us to Implement the Bumper_Switches_Init function as well as the Bumper_Switches_Handler function, once we completed these we tested the bumper switches, the required screenshots are also located in the [image](/images/) files. Moving on from these tasks we implemented the Timer_A0_PWM_Init function, for this function we used the SMCLK clock source, divided it by 8 and were in the up/down mode. Once this was done we implented the functions that controlled the direction of the motors. Finally we were able to test it to make sure it worked, as well as implement a function to handle collisions. This function would cause the robot to stop for two seconds once it collided with an object, then the robot would move backwards and turn right. From this lab we learned how to implement PWM, using Timer_A modules, to move a robot. 
## Known Issues or Limitaitons
During this Lab we did not find any issues or limitations.

## Author Contribution
Both of us collaborated on the main procedure for this lab.
* Michael Sanchez
    * Worked on Tasks 4, 5 and part of 7


## References

* MSP432P4xx SimpleLink™ Microcontrollers
Technical Reference Manual