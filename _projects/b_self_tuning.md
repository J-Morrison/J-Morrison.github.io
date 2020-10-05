---
title: "Adaptive Air-Fuel Ratio Control"
subtitle: "April 2019"
excerpt: "This was the final project for a graduate level course on self tuning control."
header:
  image: /assets/images/engine.png
  teaser: /assets/images/engine.png
---
*Completed April 2019*

This project is based on a paper called "Adaptive Air-Fuel Ratio Regulation for Port-Injected Spark-Ignited Engines Based on a Generalized Predictive Control Method" by L. Meng et al, which can be found in its entirety [here](https://www.mdpi.com/1996-1073/12/1/173).

For this project it is assumed that the only system variable defined in the paper that can be manipulated is the fuel injection mass flow rate and that the engine system can be described by a given CARIMA model. The control objective for the system is then to maintain the engine fuel/air equivalent ratio at 1 during simulations of 1000 samples. 

In order to meet the control objective an adaptive generalized preidictive controller is designed and adjusted to handle four sets of increasingly difficult engine simulation settings. In each case a simulation is carried out and the results are analysed. For the first case constant parameters are simply assumed, providung a nominal parameter set. In the next case, some parameters are tweaked to test the robustness of the controller. In the third case it is then assumed that the fraction of the flowing fuel that ends up as liqud wall film is time varying and can be described by a sin wave. Further, the mass flow rate of air into the engine cylinder is also assumed to vary over the 1000 simulation samples. Finally, the fourth case uses the same simulation settings as the third case while also featuring variations in system delay, with the amount of delay in the system changing every 200 samples or so.

I completed this project for a graduate level course on self tuning control. The full pdf document for the project can be accessed by clicking below.

[View Document](/projects/JacobMorrison_AdaptiveAirToFuelRatioControl.pdf){: .btn .btn--primary}