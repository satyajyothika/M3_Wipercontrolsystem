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
