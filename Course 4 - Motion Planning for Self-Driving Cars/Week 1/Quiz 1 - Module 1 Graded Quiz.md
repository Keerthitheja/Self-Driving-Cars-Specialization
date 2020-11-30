# Module 1 Graded Quiz
---
**Question 1.**
Which are examples of common scenarios in the autonomous driving motion planning problem?

- [ ] A. Left and right turns

- [ ] B. Driving up a hill

- [ ] C. Lane changes

- [x] D. A & C
```
Correct
Correct, left turns, right turns, and lane changes are all examples of common
driving scenarios for the autonomous driving motion planning problem.
```

**Question 2.**
What are some examples of dynamic obstacles?

- [ ] A. Trees

- [ ] B. Cyclists

- [ ] C. Cars

- [ ] D. Boulevards

- [x] E. B & C
```
Correct
Correct, cyclists and cars are examples of dynamic obstacles.
```

**Question 3.**
True or false, the autonomous driving mission takes pedestrian behaviour into consideration.

- [ ] True
- [x] False
```
Correct
Correct, mission planning abstracts away dynamic obstacles, such as pedestrians.
```

**Question 4.**
True or false, "Staying Stopped" is a maneuver that is useful for handling traffic light controlled intersections.

- [x] True
- [ ] False
```
Correct
Correct, we require the car to stay stopped at a red light, so it is useful for traffic light controlled intersections.
```

**Question 5.**
Which of these are reasons for decomposing motion planning into a hierarchy of optimization problems?

- [x] A. More computationally efficient
```
Correct
Correct, breaking it into smaller problems helps efficiency.
```
- [x] B. Can tailor each optimization problem to specific level of abstraction
```
Correct
Correct, different levels of abstraction are appropriate for different sub-problems.
```
- [ ] C. Generates higher-quality solutions than solving the problem in its entirety

- [ ] D. None of the above


**Question 6.**
True or false, instantaneous curvature is the inverse of the instantaneous turning radius at a point on a curve.

- [x] True
- [ ] False
```
Correct
Correct, these two values are inversely related.
```

**Question 7.**
Static obstacles constrain...

- [ ] The car's lateral velocity
- [x] The locations the car can occupy
- [ ] The turning radius of the car
- [ ] The car's longitudinal velocity
```
Correct
Correct, for the car's path to remain collision free, the positions along
its path cannot come into contact with the static obstacles surrounding it.
```

**Question 8.**
A leading vehicle in the ego vehicle's lane constrains...

- [ ] The car's lateral velocity
- [ ] The car's maximum jerk
- [ ] The turning radius of the car
- [x] The car's longitudinal velocity
```
Correct
Correct, we must regulate our speed relative to the speed of a leading vehicle
to prevent a collision.
```

**Question 9.**
True or false, the time gap is the amount of time that it would take for the ego vehicle to reach the current position of its leading vehicle.

- [x] True
- [ ] False
```
Correct
Correct, the time gap is defined as the amount of time that it would take for the ego vehicle to reach the current position of its leading vehicle.
```

**Question 10.**
True or false, the friction ellipse is always a tighter constraint than the comfort rectangle.

- [ ] True
- [x] False
```
Correct
Correct, in general, the friction ellipse is a looser constraint than the
comfort rectangle.
```

**Question 11.**
To generate the shortest path to a point, we need to minimize...

- [ ] Curvature
- [ ] Angular velocity
- [x] Arc length
```
Correct
Correct, the length of a path is given by its arc length.
```

**Question 12.**
The integral of difference (IOD) term in a planning objective function can be used to...

- [ ] A. Improve path smoothness
- [ ] B. Track a reference velocity profile
- [ ] C. Track a reference path
- [x] D. B & C
```
Correct
Correct, it is useful for tracking both a reference velocity profile as well
as a reference path.
```

**Question 13.**
True or false, jerk is the derivative of acceleration with respect to time.

- [x] True
- [ ] False
```
Correct
Correct, this is the definition of jerk.
```

**Question 14.**
True or false, maximizing jerk increases the comfort of our planned trajectory.

- [ ] True
- [x] False
```
Correct
Correct, maximizing jerk will make the ride less comfortable for our passengers.
```

**Question 15.**
The _____ at each point in the path constrains the velocity that can be driven at that point, due to the lateral acceleration constraints.

- [x] Curvature
- [ ] Heading
- [ ] Y position
- [ ] X position
```
Correct
Correct, the curvature of the path is what constrains our maximum velocity, due to our lateral acceleration constraints.
```

**Question 16.**
True or false, mission planning focuses on map-level navigation from the ego vehicle's current position to a final destination.

- [x] True
- [ ] False
```
Correct
Correct, mission planning is a higher-level planning sub-problem.
```

**Question 17.**
What are some examples of the inputs a finite state machine might take in the context of behaviour planning for autonomous driving?

- [x] Traffic light transitions
```
Correct
Correct, this is an important regulatory element that needs to be handled.
```
- [ ] The number of passengers in the ego vehicle
- [x] Pedestrian locations
```
Correct
Correct, pedestrians are important agents in the driving task space.
```
- [x] Vehicle positions
```
Correct
Correct, this is critical for determining ego vehicle behaviour.
```

**Question 18.**
True or false, reinforcement learning relies on interacting with an environment during the learning process.

- [x] True
- [ ] False
```
Correct
Correct, learning by interaction is critical for reinforcement learning.
```

**Question 19.**
What is a drawback of using a sampling-based method for path planning?

- [x] A. If run for a minimal number of iterations, it can generate poor quality paths
- [ ] B. It is often slow at exploring the workspace compared to other methods
- [ ] C. Sampling based methods are often computationally intractable
- [ ] D. None of the above
```
Correct
Correct, with two few iterations, even an asymptotically optimal
sampling-based planner can produce low quality paths to the goal region.
```

**Question 20.**
True or false, a conformal lattice planner selects goal points ahead of the car that are laterally offset from the centerline of the road, plans paths to each goal point, then selects the best collision-free path according to some objective function.

- [x] True
- [ ] False
```
Correct
Correct, this process underlies the lattice generation step for a conformal
lattice.
```
