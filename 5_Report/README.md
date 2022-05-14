# M3_Wipercontrolsystem


![wipers](https://user-images.githubusercontent.com/101032635/168334457-63cd8b6b-3ca7-49b7-8513-8ad859a6b231.jpg)

## Abstract

A windscreen wiper or windshield wiper or wiper blade is a device used to remove rain, snow, ice, washer fluid, water from a vehicle's front window. Almost all motor vehicles, including cars, trucks, buses and train locomotives are equipped with one or more such wipers, which are usually a legal requirement. The wiper blades are made of rubber and must apply enough pressure to the windshield in order to remove all moisture without any streaks. The blade is swung back and forth over the glass, pushing water, other precipitation, or any other impediments to visibility, from its surface.

Most windscreen wipers operate together with a windscreen washer; a pump that supplies a mixture of water, alcohol, and detergent (a blend called windscreen washer fluid) from a tank to the windscreen. The fluid is dispensed through small nozzles mounted on the hood. Conventional nozzles are usually used, but some designs use a fluidic oscillator to disperse the fluid more effectively.

Some vehicles are now available with automatic or driver-programmable windscreen wipers that detect the presence and amount of rain using a rain sensor. The sensor automatically adjusts the speed and frequency of the blades according to the amount of rain detected. These controls usually have a manual override.

In this project, we use the STM32 an ARM based Microcontroller to illustrate an automobile wiper control system. Most automobile wipers are controlled by a DC motor, however because the STM32 lacks a motor, we are exploring using LEDs in this application. The STM32 has four LEDs and a Push Button. The colours of these LEDs are orange, green, red, and blue. If you push and hold the user button for two seconds, the Red Led is on indicating that the ignition key is positioned at the ACC. Furthermore, the LEDs are flickering with a frequency of 1HZ when the push button is pressed indicating that the wipers are turned on. If we again press the push button the LED’s flicker with increased frequency of 4HZ,and if we press third time the LED’s will flicker with a increased frequency of 8HZ and if we press fourth time the LED’s will stop after coming to starting position. And if we push and hold the user button for two seconds the red LED turns off indicating that the the ignition key is positioned at the Lock.

## Requirements

## Introduction

A windscreen wiper or windshield wiper or wiper blade is a device used to remove rain, snow, ice, washer fluid, water from a vehicle's front window. Almost all motor vehicles, including cars, trucks, buses and train locomotives are equipped with one or more such wipers, which are usually a legal requirement.  The wiper blades are made of rubber and must apply enough pressure to the windshield in order to remove all moisture without any streaks. The blade is swung back and forth over the glass, pushing water, other precipitation, or any other impediments to visibility, from its surface. 

## SWOT Analysis

### Strengths:

*	Visual clarity.

* The wiper does not stop in the middle of the window,Even if stooped in the middle, the wiper returns to its default position.

* The wiper speed can be adjusted.

### Weaknesses:

* Rubber Blades need to be replaced after a while, which raises the expense. 

### Opportunities:

* Rain detection and automatic operation can be added as extra features.

### Threats:

* windshield wiper blades are made of rubber that's meant to handle water and sometimes ice. Faced with anything solid, these rubber blades can rip easily causing your wipers not to work.

## 5W's and 1H

### Who:

  It is extremely important for drivers of any type of vehicle that require clear road visibility in the event of dust, snow, or rain.
  
### What:

It is the Wiper Control system, which is installed in all automobiles to safeguard the safety of passengers and drivers during inclement weather.

### When:

When the weather is terrible, such as snow, dust, or rain.

### Where:

It can be found in the windscreen of an automobile.
### Why:

Keeping the windscreen clean so that you may see well at all times.
### How:

It is implemented using the STM32 microcontroller.

## High Level Requirements

<html>
<body>
<!--StartFragment-->

ID | Description | Status 
-- | -- | --
HLR-1 | Operation in ACC Mode | Implemented
HLR-2 | Activation of the Wiper System | Implemented
HLR-3 | Control the wiper speed | Implemented  
HLR-4 | Deactivation of the Wiper System | Implemented
HLR-5 | Operation in lock Mode | Implemented

<!--EndFragment-->
</body>
</html>

## Low Level Requirements

<html>
<body>
<!--StartFragment-->

ID | Description | Status 
-- | -- | --
LLR-1 | Push button pressed once for 2 sec-ON RED LED | Implemented
LLR-2 | Button pressed once-Blue, Green, Orange blink with 1HZ | Implemented
LLR-3 | Button pressed second time-Blue, Green, Orange blink with 4HZ | Implemented
LLR-4 | Button pressed third time-Blue, Green, Orange blink with 8HZ | Implemented
LLR-5 | Button pressed fourth time-LED’s will stop blinking after coming to Blue LED | Implemented
LLR-6 | Push button pressed again for 2 sec- OFF RED LED | Implemented


<!--EndFragment-->
</body>
</html>

## Behavioural Diagrames

## Block Diagram

![BLOCK_page-0001](https://user-images.githubusercontent.com/101032635/168335094-88e1cccf-b6aa-45ad-95a4-43fda8f9c7ee.jpg)


## High Level Flow Chart

![FC-HL_page-0001 (1)](https://user-images.githubusercontent.com/101032635/168335080-c59a9e02-2e44-4d73-859b-d7d8a11d70fe.jpg)


## Low Level Flow Chart

![FC_page-0001](https://user-images.githubusercontent.com/101032635/168335055-37d063a7-a7dc-4f88-b706-8a6985733441.jpg)


## Schematic Diagram

![STM32](https://user-images.githubusercontent.com/101032635/168335136-7e06fb74-f574-408a-8b4b-9901acee8e7b.jpeg)

## TestCases

## High Level Test Plan

<html>
<body>
<!--StartFragment-->

ID | Description | Expected Output | Actual Output | Status 
-- | -- | -- | -- | --
HL-1 | Operation in ACC Mode | Engine Started | Engine Started | Success
HL-2 | Activation of the Wiper System | Wipers ON | Wipers ON | Success
HL-3 | Control the wiper speed | The wiper's speed can be adjusted. | The wiper's speed can be adjusted. | Success  
HL-4 | Deactivation of the Wiper System | Wipers OFF | Wipers OFF | Success
HL-5 | Operation in lock Mode | Engine Stops | Engine Stops | Success

<!--EndFragment-->
</body>
</html>


## Low Level Test Plan

<html>
<body>
<!--StartFragment-->

ID | Description | Expected Output | Actual Output | Status 
-- | -- | -- | -- | --
LL-1 | Push button pressed once for 2 sec | RED LED ON | RED LED ON | Success
LL-2 | Button pressed once | Blue, Green, Orange blink with 1HZ | Blue, Green, Orange blink with 1HZ | Success
LL-3 | Button pressed second time | Blue, Green, Orange blink with 4HZ | Blue, Green, Orange blink with 4HZ | Success
LL-4 | Button pressed third time | Blue, Green, Orange blink with 8HZ | Blue, Green, Orange blink with 8HZ | Success
LL-5 | Button pressed fourth time | LED’s will stop blinking after coming to Blue LED | LED’s will stop blinking after coming to Blue LED | Success
LL-6 | Push button pressed again for 2 sec | RED LED OFF | RED LED OFF | Success


<!--EndFragment-->
</body>
</html>

