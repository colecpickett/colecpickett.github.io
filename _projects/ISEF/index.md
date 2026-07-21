---
layout: post
title: Ionic Thruster Design and Optimization (ISEF submission)
description:  I worked in partnership to test multiple variables in optimization of ionic thrust utilizing standard atmosphere. We successfully were able to optimize anode-cathode distance and test multiple different shapes to create a theoretically optimized thruster design. 
skills: 
  - Fusion 360
  - SLA/FDM prototyping
  - Custom Test Fixture Design
  - Soldering
  - Circuit Design
  - Data Analysis
  - Electroplating

main-image: /ISEF_Title.png
---
---

## The Problem:
Ion thrusters typically operate in the vacuum of space, where the absence of atmospheric resistance allows even small thrust forces to accelerate a craft over time. Producing measurable, controllable ion thrust *within* Earth's atmosphere presented a different challenge: identifying the anode-cathode configuration and voltage that would generate usable thrust using the atmosphere itself as propellent.

## The Product:
The result is a functioning ion thruster prototype paired with a custom-built thrust measurement fixture, designed to quantify thrust output at varying voltages and electrode distances. The system uses a DC power supply stepped up to an estimated 40,000V to ionize air between a copper anode and cathode, generating measurable thrust via ion drift.

## Design:
I designed and fabricated both the thruster and its test fixture, using Fusion 360 to model a rig capable of isolating and measuring small thrust forces via a cantilevered tensiometer. The thruster itself was manufactured from copper sheet and tubing, soldered throughout to ensure continuous electrical continuity under high voltage.

{% include image-gallery.html images="thruster-cad.png, rig-photo.png" height="400" %}

## Analysis:
To identify the optimal thruster configuration, I ran data analysis across a range of anode-cathode distances and voltages, measuring resulting thrust with the custom tensiometer fixture. This process identified the optimal electrode spacing for maximum thrust within atmospheric conditions, validated through repeated testing at varying voltage levels.

{% include image-gallery.html images="testing-setup.png" height="400" %}

## Results:
Qualitative streamer testing showed firmer, more consistent airflow compared to earlier design iterations, confirming the improved electrode geometry translated to real performance gains. The completed prototype and testing methodology earned 1st place in Electrical Engineering at the Oregon State Science Fair.

{% include image-gallery.html images="final-prototype.png" height="400" %}

## Future Work:
Building on this first-generation design, I identified two areas for continued development:

**Future Testing:**
- Testing alternative anode and cathode geometries to further optimize thrust output
- Analyzing the effect of manipulating chamber air pressure on thrust performance

**Future Design:**
- Using CFD to design an optimized inlet and nozzle geometry
- Developing a lighter, more aerodynamic cathode by electroplating carbon-coated SLA prints

{% include image-gallery.html images="future-design-cad.png, future-cathode.jpg, electroplate-design.png" height="300" %}

