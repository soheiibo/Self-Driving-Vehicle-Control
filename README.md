# Self-Driving-Vehicle-Control

This respository explains the approach implemented for the final project of the course, Introduction to Self-Driving Cars from the Self-Driving Cars Coursera Specialization.

The aim of this project was to implement a controller in Python to drive a car around a track in the Carla Simulator. To control successfully the vehicle, both longitudinal and lateral controllers were implemented, in order to obtain the throttle, brake and steering control signals.

![ezgif-6-0823856c2c7b](https://user-images.githubusercontent.com/64086951/88726973-8fd0a700-d126-11ea-8b7a-4fc4fc05554f.gif)


## Project notes:
The waypoints include positions as well as the speed the vehicle should attain. As a result, the waypoints become the reference signal for our controller and navigating to all the waypoints effectively completes the full track.

Since the controller reference contains both position and speed, we need to implement both Longitudinal and Lateral Control.

The output of the controller will be the vehicle throttle, brake and steering angle commands.

The throttle and brake come from the Longitudinal speed control and the steering comes from our Lateral Control.

If you want to make your own controller design, I highly recommend that you should  open 
# controller2d.py.

## The Race Tack including waypoints:
![590](https://user-images.githubusercontent.com/64086951/88724909-27cc9180-d123-11ea-9ba4-1e8712c74add.jpg)

## Some concepts including formulas and expected output of the controller :

![510](https://user-images.githubusercontent.com/64086951/88725848-a413a480-d124-11ea-988a-71a70f8c0d44.jpg)
![55582651-b9431380-5728-11e9-9a26-46e08467ffd3](https://user-images.githubusercontent.com/64086951/88726005-e0df9b80-d124-11ea-9cca-fca55f7fec85.jpg)

# Results

## Longitudinal control
To evaluate the performance of the longitudinal controller the next image is provided. In the graph, the speed profile proposed to drive the car around the track is in orange, and the real vehicle speed obtained by using the PID controller is in blue.

![Figure_2](https://user-images.githubusercontent.com/64086951/88726231-43389c00-d125-11ea-8dce-c35b3a48fe8e.png)

## Lateral control
Similar to the longitudinal controller, a image is provided to shown the performance of the lateral controller. In the graph, the trajectory proposed to drive the car around the car is shown in blue, and the trayectory followed by the vehicle by using the Pure pursuit Controller is in orange.

![Figure_1](https://user-images.githubusercontent.com/64086951/88726320-66634b80-d125-11ea-9d9b-441f700459c0.png)

Other types of controllers such as the Stanley or even the Model Predictive Control could be implemented to try to enhance the system performance.
