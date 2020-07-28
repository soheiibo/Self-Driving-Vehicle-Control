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

## Some concepts including formulas and expected output of the controller :

![510](https://user-images.githubusercontent.com/64086951/88725848-a413a480-d124-11ea-988a-71a70f8c0d44.jpg)
![55582651-b9431380-5728-11e9-9a26-46e08467ffd3](https://user-images.githubusercontent.com/64086951/88726005-e0df9b80-d124-11ea-9cca-fca55f7fec85.jpg)

# Results
## Longitudinal control
To evaluate the performance of the longitudinal controller the next image is provided. In the graph, the speed profile proposed to drive the car around the track is in orange, and the real vehicle speed obtained by using the PID controller is in blue.
![forward_speed](https://user-images.githubusercontent.com/64086951/88726117-08366880-d125-11ea-95ef-ccf11e29e062.png)
