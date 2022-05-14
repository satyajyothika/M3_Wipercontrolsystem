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
