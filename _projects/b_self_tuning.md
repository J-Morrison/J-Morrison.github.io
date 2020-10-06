---
title: "Adaptive Air-Fuel Ratio Control"
subtitle: "April 2019"
excerpt: "This was the final project for a graduate level course on self tuning control."
header:
  image: /assets/images/engine_.png
  teaser: /assets/images/engine.png
---
*Completed April 2019*

This project is based on a paper called "Adaptive Air-Fuel Ratio Regulation for Port-Injected Spark-Ignited Engines Based on a Generalized Predictive Control Method" by L. Meng et al, which can be found in its entirety [here](https://www.mdpi.com/1996-1073/12/1/173).

For this project it is assumed that the only system variable defined in the paper that can be manipulated is the fuel injection mass flow rate and that the engine system can be described by a given CARIMA model. The control objective for the system is then to maintain the engine fuel/air equivalent ratio at 1 during simulations of 1000 samples. 

In order to meet the control objective an adaptive generalized predictive controller is designed and adjusted to handle four sets of increasingly difficult engine simulation settings. Further, this adaptive controller is designed to use the Exponential Forgetting and Resetting Algorithm (EFRA) for parameter estimation. In each case, a simulation is carried out and the results are analysed. For the first case, constant parameters are simply assumed, providing a nominal parameter set. In the next case, some parameters are tweaked to test the robustness of the controller. In the third case, it is then assumed that the fraction of fuel entering the engine that becomes liquid wall film is time varying and can be described by a sine wave. Further, the mass flow rate of air into the engine cylinder is also assumed to vary over the 1000 simulation samples. Finally, the fourth case uses the same simulation settings as the third case, while also featuring variations in system delay. Here, the amount of delay in the system changes every 200 samples or so.

In the end the designed adaptive generalized predictive controller proved capable of handling the different sets of simulation settings quite well. This leads to the positive conclusion that adaptive generalized predictive control with EFRA parameter estimation represents a solid control option for time varying single-input single-output systems, even when aspects of the system, such as the delay, are both unknown and variable.

I completed this project for a graduate level course on self tuning control. The full pdf document for the project can be accessed by clicking below.

[View Document](/projects/JacobMorrison_AdaptiveAirToFuelRatioControl.pdf){: .btn .btn--primary}