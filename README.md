# Mobility

The mobility system of the rover is comprised of a wheel sub-assembly, rocker-bogie suspension and a differential joint connecting the suspension to the chassis. 

## Rocker Bogie Suspension
This suspension was chosen to ensure the chassis remains parallel to the ground at all times. Furthermore, the system is designed such that the rover can traverse objects up to 30cm in height, without compromising the stability of the system. All components in the suspension are manufactured using Aluminium 6065, which was chosen for its light weight, tensile strength and manufacturability. 

## Wheels and Motors
The wheels on New Opportunity are made from durable, puncture-resistant rubber and are inflatable. This allows us to adjust the pressure within the wheels based on the terrain. 170KV brushless DC motors by Alien Power Systems were chosen since they provide high torque at a low RPM, have sufficient documentation and are reliable. The motors are controlled via Flipsky VESCs using PPM signals from the on-board ATmega328P-based microcontroller. 

## Suspension-Chassis Joint
The self-levelling mechanism is guided by the rotating differential bar attached to the chassis and rocker. 

## Control Scheme
The rover is steered using a 6-wheeled differential drive mechanism. The six wheels on the rover rotate at different velocities to achieve a desired rotation/movement. The control input comes from a joystick/autonomous command, which provides coordinates to the microcontroller, which in turn runs the motors at calculated velocities. The control scheme also uses a PID controller with a negative feedback loop to account for differences in velocities which may occur due to terrain/obstacles.
