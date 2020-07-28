# Self-Driving-Vehicle-Control

This respository explains the approach implemented for the final project of the course, Introduction to Self-Driving Cars from the Self-Driving Cars Coursera Specialization.

The aim of this project was to implement a controller in Python to drive a car around a track in the Carla Simulator. To control successfully the vehicle, both longitudinal and lateral controllers were implemented, in order to obtain the throttle, brake and steering control signals.

## Project notes:
The waypoints include positions as well as the speed the vehicle should attain. As a result, the waypoints become the reference signal for our controller and navigating to all the waypoints effectively completes the full track.

Since the controller reference contains both position and speed, we need to implement both Longitudinal and Lateral Control.

The output of the controller will be the vehicle throttle, brake and steering angle commands.

The throttle and brake come from the Longitudinal speed control and the steering comes from our Lateral Control.

If you want to make your own controller design, I highly recommend that you should consider the following points:

If you open the simulator directory and navigate to the Course1FinalProject folder, you will see a file named controller2d.py
## The Race Tack including waypoints:
![590](https://user-images.githubusercontent.com/64086951/88724909-27cc9180-d123-11ea-9ba4-1e8712c74add.jpg)
