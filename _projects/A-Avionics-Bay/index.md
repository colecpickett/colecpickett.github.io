 ---
layout: post
title: Avionics Bay for Supersonic Vehicle (Current Development)
description: I am leading the design prototype and final manufacture of the sustainer avionics bay on a two stage carbon fiber super sonic rocket. This is part of my involvement with Aerospace NU
skills: 
  - Dimension Contrained Design
  - Cross-Functional Design
  - Modal Analysis
  - FDM 3D Print Prototyping
main-image: /Current_State.png
---
---

## The Goal:
Create an avionics bay to fit inside a 95mm diameter within 160mm height. The avionics bay had run time contraints set by our launch site as well. Our avionics team advised on battery choice, and required circuitry. The avionics bay requires a flight controller to ignite stage 2, 3 cameras for 3 different views, as well as gps and barometric telemetry.

## Challenges:
The avionics bay needs to be developed quickly to enable a launch in November. For this reason it was important I prioritized my contraints. I decided to prioritize spacial contraints and manufacturability. This is because these are non-negotiable for a succesfful fast development project. Other important contraints like aerodynamic performance and weight saving took a back seat to support faster development. 

Next to the 1000oz wet weight of the rocket, the avionics bay weighs relatively little. On top of this the majority of the avionics bay weight is from the batteries and cameras, not the packaging. This means that the maximum 3 oz plastic sled is inconsequential next to the rockets 1000oz total. Aerodynamically, I have made some considerations. The more obtrusive cameras will be placed opposite our launch rails in order to cause the least offset possible in center of pressure, however the small faring for the obtrusive camera will be minor due to our large stabilizers, and once at high speeds the hole for the side view camera will have minimal impact due to boundary layer conditions.

## Design:
The design of the avionics bay is a triangular sled with two battery holders that can slide into either end. These are then clamped between two fiberglass end caps for protection.
{% include image-gallery.html images="Screenshot 2026-10-23 122957.png, Screenshot 2026-10-23 123049.png" height="300" %}

Why a triangle?
The triangle was inspired by the constraint of 3 cameras. With one camera per section and room in the middle for battery storage, the avionics bay could be kept within the 160mm height constraint. Furthermore the compartmented design allows easier access/replacement of batteries
{% include image-gallery.html images="Screenshot 2026-10-23 122929.png" height="300" %}

## Analysis:
Since the airframe is carbon fiber, the avionics bay is not needed aas a structural element. However, there are some vibrational concerns in order to prevent damage of the camera footage. For revision 1 I have not had time to analyze the camera mounts, but I do have steps I plan on following for the next iteration. 

The main source of vibration is the rocket motor. This does not have main frequency ranges I can design my camera mounts to avoid, instead it is such a disruptive source I am pushed to design a mount against vibrational magnitude instead. I plan on learning to use Solidworks modal analysis tool, and measuring the magnitude of vibration experienced at the avionics bay during its first flight. This will allow me to design the next revision to withstand that magnitude within a certain maximum rotation value. I will set that maximum rotation value by my target of less than 2 pixels of smear. I can convert pixel smear to rotation at the sensor using a pinhole smear model. 

## Rapid Prototyping:
The design for revision 1 is almost complete, and the first prototype will be 3D printed from ABS plastic using water soluable PLA supports this coming week. 

## Cross-Functional Design:
As an avionics packaging project I have worked closely with our avionics division to determine their needs for antennae access, technology needs, and battery sizing. 
