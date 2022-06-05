# Quantifying-Safety-of-Learning-based-Self-Driving-Control-Using-Almost-Barrier-Functions

This repository contains the parameters of Kinematic and Dynamic models used in the paper (revised) _Quantifying Safety of Learning-based Self-Driving Control Using Almost-Barrier Functions_.



---


## Vehicle Dynamics Models

Kinematic Model      |  Dynamic Model    
:-------------------------:|:------------------------:
![Kinematic Model](/figures/kinematic_model.png)  |  ![Dynamic Model](/figures/dynamic_model.png) 

The figures above illustrate the kinematic and dynamic vehicle models. The only parameter for the Kinematic model is the wheelbase of the vehicle, which we use $L=2.9$ meters.

For Dynamic model, the parameters are shown in the table below:

| Parameter | Description                                                                 | Value |
|-----------|-----------------------------------------------------------------------------|-------|
| $L$       | Wheelbase (m)                                                               | 4.35  |
| $m$       | Mass (kg)                                                                   | 1600  |
| $I_z$     | Yaw inertia (kg·m^2)                                                        | 7500  |
| $l_f$     | Center of gravity to the front axle (m)                                     | 2.175 |
| $l_r$     | Center of gravity to the rear axle (m)                                      | 2.175 |
| $c_f$     | Coefficient for front tire cornering stiffness linear approximation (N/rad) | 2e4   |
| $c_r$     | Coefficient for rear tire cornering stiffness linear approximation (N/rad)  | 2e4   |

The implementations of the dynamics are based on [[1]](#1), [[2]](#2) and [[3]](#3). We are working to get the full codebase of the barrier function training and verification soon.

<a id="1">[1]</a> 
Snider JM. 
Automatic Steering Methods for Autonomous Automobile Path Tracking.
2009.

<a id="2">[2]</a> 
Sakai A, Ingram D, Dinius J, Chawla K, Raffin A, Paques A. 
PythonRobotics: a Python code collection of robotics algorithms. 
Published online 2018. doi: <https://doi.org/10.48550/arXiv.1808.10703>

<a id="3">[3]</a> 
Dong C. 
PathTrackingBicycle. GitHub repository.
<https://github.com/Derekabc/PathTrackingBicycle>.
2020.