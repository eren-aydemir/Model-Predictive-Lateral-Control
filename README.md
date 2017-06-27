### Model-Predictive-Steering-Control

This project aims to find an optimal tracking path for a vehicle to follow given waypoints. The solution uses IPOPT and CPPAD to overcome this optimization problem. The optimization considers kinematic models of a vehicle and cost functions for given boundiries and coinstraints and produces safe to drive actuation inputs as steering and throttle-braking. 

# Kinematic Vehicle Model


# Timestep Length and Elapsed Duration (N & dt)

N and dt together arrange that the optimizer considers how many data points in how much time. Choosing N around 10 or more and arraging dt that satisfies N*dt = 1 generally gives sufficient results. Tried combination of N & dt are 10/0.1, 25/0.04 and many others.

# Latency Issue

Latency is a real-world problem that may encounter due imperfect steering system and nonlinear effects like bushes and tires. In this project Udacity Simulator has been used to simulate latency between simulation and data acquision. 100ms latency has been used which is also good example for passenger and heavy commercial vehicles.  
