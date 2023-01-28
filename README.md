# Name-Engraving-Robot

This project demonstrates how to use the RoboDK API to control a robot in order to engrave a name on a surface.

![image](https://user-images.githubusercontent.com/111273105/184798821-87040b96-309e-4c74-8be3-d6167b462b31.png)

## Requirements

* RoboDK software (Demo version can be found at https://www.robodk.com/download)
* A robot with 6 degrees of freedom
* A reference target in the RoboDK environment (named "Target 1" in the script)

## How it works

The script starts by importing the necessary libraries (robolink and robodk) and initializing the RoboDK API (RDK). It then retrieves the first robot found in the RoboDK environment and the reference target (named "Target 1").

The robot is then moved to the reference point using the MoveJ method. The script then enters a loop where it calculates the new position of the robot based on the angle of rotation and the radius of the hexagon. The new position is set using the setPos method and the robot is moved to the new target using the MoveL method.

The script ends by triggering a program call (RunInstruction) and moving the robot back to the reference target.

## How to test

1. Run the .rdk file on the RoboDK software
2. Observe the robot engraving a hexagon shape around the reference target
3. The engraving can be adjusted by changing the radius of the hexagon and the angle of rotation in the script
    
Note: The above script is for demonstration purpose only, you need to adjust according to your robot type and the workpiece you want to engrave.



