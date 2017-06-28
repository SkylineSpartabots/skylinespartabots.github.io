---
title: Electronics
---
# Electronics
{:.no_toc}

{::options parse_block_html="true" /}
<div id="toc_nav">
* This line is for the table of contents to be generated
{:toc}
{:.nav}
</div>
{::options parse_block_html="false" /}

<!-- Don't change anything above this point! -->

## Basics
Electronics is a complex system of wires and equipment that allow the robot to function. Electronics' primary role is connecting the brain of the robot to the motors and servos to bridge the gap between software and hardware.

To wire FRC electronics, begin with the roboRIO. The roboRIO is the robot's processor and stores and runs software. Next, connect the roboRIO to the power distribution board (PDM). Next, connect the motor controllers to the power distribution board by using a screwdriver to open the flap. With CANTalons, connect all of the CANTalons together and one to the roboRIO. With Talons or Victors, simply connect the PWM cables straight to the roboRIO. To connect the motor controllers to the motors, crimp the wires and put them into Anderson connectors. Finally, connect the motor controller Anderson connectors to the motor's Anderson connectors.

## Parts

### roboRIO
![Image of a roboRIO](https://user-images.githubusercontent.com/14433542/27520111-b9fd448c-59b7-11e7-9f6f-a7759a431d75.png)

The roboRIO is the robot's main processor, meaning it stores and runs software that controls the robot's hardware.

[User manual for NI-roboRIO](http://www.ni.com/pdf/manuals/374474a.pdf)

If you're interested in the roboRIO's specifications, you can find them [here](http://www.ni.com/pdf/manuals/375275a.pdf).

## Tools

### Wire strippers
To strip a wire close the wire strippers around the wire at its corresponding width and pull.

### Crimpers
Work in progress

## Useful links
[Wiring the 2015 FRC Control System (pdf)](https://docs.google.com/viewer?a=v&pid=sites&srcid=ZGVmYXVsdGRvbWFpbnxzcGFydGFib3Rzd2lraXxneDo1YjNlNTI5M2JhZTZiN2Fk)

[2017 control system hardware overview - WPILib](http://wpilib.screenstepslive.com/s/4485/m/24166/l/144968-2017-frc-control-system-hardware-overview)
