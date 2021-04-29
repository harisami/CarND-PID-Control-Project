# CarND-Controls-PID
Self-Driving Car Engineer Nanodegree Program

---

## Goal

In this project you'll revisit the lake race track from the Behavioral Cloning Project. This time, however, you'll implement a PID controller in C++ to maneuver the vehicle around the track!

The simulator will provide you the cross track error (CTE) and the velocity (mph) in order to compute the appropriate steering angle.

One more thing. The speed limit has been increased from 30 mph to 100 mph. Get ready to channel your inner Vin Diesel and try to drive SAFELY as fast as possible! NOTE: you don't have to meet a minimum speed to pass.

## Reflection

Keeping `Kp` (proportional component) zero caused the car to go very close to the edges and ultimately off the road.

`Ki` (integral component) became smoother when I brought it down close to zero, from 0.004 to 0.001, but at the expense of more swinging at the begining of each ride.

`Kd` (differential component) being zero resulted in a lot of swinging left and right.