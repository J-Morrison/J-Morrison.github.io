---
title: "Solar Control Based On Load Prediction"
excerpt: "This project was my master's thesis. It incorporates both controls and machine learning."
header:
  image: /assets/images/system_pic2.png
  teaser: /assets/images/system_pic2.png
---
*Completed August 2020*

In this project an Iterative Learning (IL) approach to disturbance prediction that uses intelligent iteration grouping is proposed for Economic Model Predictive Control (EMPC), and applied it to an Integrated Solar Thermal System (ISTS) in order to improve controller performance. An ISTS consists of a Solar Thermal Collector (STC) which collects energy from the sun, a Thermal Storage Tank (TST) which stores this energy for later use, and an auxiliary Heat Pump (HP) which acts as the actuator for the system, providing additional energy as required. The disturbance in the system is then the user hot water demand. In order to optimize the control performance of an ISTS with EMPC, it is important to be able to accurately predict this hot water demand before it happens. To solve this problem, a novel IL-based approach to disturbance prediction for EMPC is presented. 

This approach involves separating long-term disturbance data, which in this case is user hot water demand, into a number of 24 hour iterations. These iterations are then further divided into groups using unsupervised learning based on the individual iteration profiles. Following the grouping of iterations, each iteration is given features such as the day of the week it occurs on, and a supervised learning classifier is trained to map from features to groups in order to predict the group of future iterations. Finally, IL is applied to learn patterns within each group iteratively and predict the actual hot water demand trajectory for future iterations. 

A simulation of an ISTS using real world hot water demand data then demonstrates the effectiveness of the proposed approach to disturbance prediction, achieving higher performance EMPC than can be attained with existing disturbance prediction methods. Specifically, the EMPC implementation using the IL-based disturbance prediction algorithm is shown to prevent constraint violations within the ISTS more effectively than all other EMPC implementations while decreasing the average daily system cost by over 6%.

I completed this project for my master's thesis. The full published thesis document can be found through the University of British Columbia Library by clicking below.

[View Thesis](https://open.library.ubc.ca/cIRcle/collections/ubctheses/24/items/1.0394371){: .btn .btn--primary}

*Note: The thesis is currently embargoed until the publication of a journal paper I wrote based on similar results. If you would like to view the full thesis document please contact me and I would be happy to share the pdf file with you.*