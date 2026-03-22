**Buck Converter Controller Design & Analysis**

This project focuses on the design and performance analysis of a Buck Converter Controller, exploring the differences between Open-loop and Closed-loop control systems. 
It includes the implementation of PI controllers and Feedforward control strategies to optimize transient response and disturbance rejection.

* Project Overview

The primary goal is to design a controller that ensures the system's output reaches the desired target (Reference Tracking) while maintaining stability against external disturbances (Disturbance Rejection).

Key Objectives:
1) Reference Tracking: Ensuring the output voltage/current follows the setpoint accurately.
2) Disturbance Rejection: Minimizing the impact of load variations or input voltage fluctuations.
3) Stability Optimization: Selecting the appropriate bandwidth to balance response speed and noise sensitivity.

* Control Strategies Implemented

  1. Open-Loop Control
  Simple and low-cost implementation by directly setting a constant duty ratio.  
  Limitation: Highly sensitive to parameter changes and external disturbances, leading to potential steady-state error

  2. Closed-Loop (Feedback) Control
  Uses a PI Controller to minimize the error between the reference ($R(s)$) and the feedback output ($Y(s)$)
  Implemented Soft-start up techniques to prevent current spikes and excessive voltage stress during initialization.
  Integrated Integrator Initialization to eliminate overshoot during the transition from open-loop to closed-loop mode.
