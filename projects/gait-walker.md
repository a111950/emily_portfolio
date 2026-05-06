---
layout: page
title: Gait Walker Project
parent: Projects
---
## Project Overview
Our team at **EnableTech** was tasked with retrofitting a standard medical Gait Walker with electric motors and custom controls. 
While the current prototype relies on commercial off-the-shelf (COTS) ESP32 and BLDC controller boards, 
we are transitioning to a fully custom integrated electronics suite. This move reduces footprint, minimizes wiring complexity, 
and allows for break and smooth start feature that our client asked for.
<p align="center">
  <img src="https://github.com/user-attachments/assets/2a3a8eab-e0cf-411a-9d37-80bf9c72cc42" width="600" height = "400", alt="Commerical motor dirver board">
  <br>
  <label><em>Figure 1: Client's Gait Walker </em></label>
</p>



<p align="center">
  <img src="https://github.com/user-attachments/assets/ac1e083e-f89f-4664-8f0c-3b41d7083bca" width="600" height = "600" alt="Commerical motor dirver board">
  <br>
  <label><em>Figure 1: Commercial RioRand Motor Driver Board</em></label>
</p>


## Role
As the Lead Electrical Engineer, I am responsible for the end-to-end design of the power electronics system. My primary focus is a high-performance 500W BLDC Motor Controller and a central control board. Key objectives include:

Smooth Motion Control: Implementing precise PWM logic for throttle and braking inputs.

Custom PCB Design: Utilizing the DRV8302 gate driver for robust power delivery and integrated current sensing.

System Integration: Managing high-current 36V rails while ensuring stable 3.3V/5V logic for the ESP32.

This is the schematic that I'm currently designing utilizing DRV 8302
<img width="544" height="381" alt="image" src="https://github.com/user-attachments/assets/e7cdf9b1-6e18-4b95-a6c8-013c2e3444d0" />


