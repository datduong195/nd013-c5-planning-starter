# Motion Planning and Decision Making for Autonomous Vehicles

In this project, you will implement two of the main components of a traditional hierarchical planner: The Behavior Planner and the Motion Planner. 

Both will work in unison to be able to:
* Avoid static objects (cars, bicycles and trucks) parked on the side of the road (but still invading the lane). The vehicle must avoid crashing with these vehicles by executing either a “nudge” or a “lane change” maneuver.
* Handle any type of intersection (3-way,  4-way intersections and roundabouts) by STOPPING in all of them (by default)
* Track the centerline on the traveling lane.

To accomplish this, you will implement:

* Behavioral planning logic using Finite State Machines - FSM
* Static objects Collision checking.
* Path and Trajectory generation using Cubic Spirals
* Best trajectory selection though a cost function evaluation. This cost function will mainly perform a collision check and a proximity check to bring cost higher as we get closer or collide with objects but maintaining a bias to stay closer to the lane center line.

## Results in Carla Simulation:
### Obstacle detection and avoidance path planning 
<img width="960" alt="obstacle_detected_left" src="https://user-images.githubusercontent.com/36104217/180063108-33529c9c-af6f-4f04-ae0d-5243a5fc068e.png">
<img width="960" alt="obstacle_detected_minimal_right_turn_1" src="https://user-images.githubusercontent.com/36104217/180063114-73ce269d-a48e-4bbf-b13b-88fb2903f789.png">
<img width="848" alt="obstacle_detected_minimal_right_turn_2" src="https://user-images.githubusercontent.com/36104217/180063120-b91db3cb-146d-4e13-aa0c-c2243e11e62c.png">
<img width="958" alt="obstacle_detected_right" src="https://user-images.githubusercontent.com/36104217/180063124-d0455e79-0568-48f7-94bf-08a7279583b7.png">

### Deceleration to stop at intersection
<img width="960" alt="deceleration_at_intersection" src="https://user-images.githubusercontent.com/36104217/180063872-ed6c7725-3eca-4d37-bcda-27868fda2edd.png">

### Full stop at intersection
<img width="960" alt="full_stop_at_intersection" src="https://user-images.githubusercontent.com/36104217/180063161-3d6df3dd-5a66-46e8-8b06-1d52daa7af43.png">
