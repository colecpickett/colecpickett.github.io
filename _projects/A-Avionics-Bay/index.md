---
layout: post
title: Avionics Bay for Supersonic Vehicle (Current Development)
description: I am leading the design prototype and final manufacture of the sustainer avionics bay on a two stage carbon fiber super sonic rocket. This is part of my involvement with Aerospace NU
skills: 
  - Dimension Contrained Design
  - Cross-Functional Design
  - Modal Analysis
  - FDM 3D Print Prototyping
  - FEA
main-image: /6B66C58C-4DF4-4DED-8540-22FDCD325043_1_105_c.jpeg
---
---

## The Goal:
Create an avionics bay to fit inside a 95mm diameter within 170mm height. Our avionics team advised on battery choice and required circuitry. The avionics bay requires a flight controller to ignite stage 2, a flight controller for drogue and main parachute deployment, 3 cameras for 3 different views, as well as gps and barometric telemetry.
{% include image-gallery.html images="F108AAC4-DC65-4387-B0AF-A8B8E9948EBC_1_105_c.jpeg" height="300" %}

## Challenges:
Development was time constrained to roughly six weeks (First test flight on November 21st. For this reason it was important I prioritized constraints. I decided to prioritize spacial contraint and manufacturability. This is because these are non-negotiable for a successful fast development project. Other important contraints like aerodynamic performance and weight saving took a back seat to support faster development. 

Next to the 1000oz wet weight of the rocket, the avionics bay weighs relatively little. On top of this the majority of the avionics bay weight is from the batteries and cameras, not the packaging. This means that the 3 oz plastic sled is inconsequential next to the rockets 1000oz total. Aerodynamically, I have made some considerations. The more obtrusive cameras will be placed opposite our launch rails in order to cause the least offset possible in center of pressure, however the small fairing for the obtrusive camera will need to be analyzed for aerodynamic forces.

## Design:
The design of the avionics bay is a triangular sled with two battery holders that can slide into either end. These are then clamped between two balsa end caps for protection.
{% include image-gallery.html images="Screenshot 2026-10-23 122957.png, Screenshot 2026-10-23 123049.png" height="300" %}

Why a triangle?
The triangle makes placement of 3 cameras easy on the 3 faces, as well as three required antenna to be evenly spaced. Furthermore the compartmented design allows easier access/replacement of batteries (stored in the center).
{% include image-gallery.html images="Screenshot 2026-10-23 122929.png, 53F49506-4859-4954-9E32-514358AD8679_4_5005_c.jpeg" height="300" %}

## Analysis:
There are some vibrational concerns in order to prevent damage of the camera footage. For revision 1 I have not had time to analyze the camera mounts, but I do have steps I plan on following for the next iteration. 

The main source of vibration is the rocket motor. This does not have main frequency ranges I can design my camera mounts to avoid, instead it is such a disruptive source I am pushed to design a mount against vibrational magnitude instead. I plan on learning to use Solidwork's modal analysis tool, and measuring the magnitude of vibration experienced at the avionics bay during its first flight. I will then use a pinhole smear model to target a pixel smear below 3 pixels. For the first test flight I opted to design my camera mounts as quite rigid, and will evaluate their performance after the test. 

Another source of concern is aerodynamic forces on the camera facing down. While the third camera is not going to be deployed on our November 21st launch, I have already begun its design. A fairing will be used to protect the camera from aerodynamic forces. This fairing must be able to survive the flight. Using OpenRocket I found the estimated highest dynamic pressure, then converted this dynamic pressure to true pressure by assuming a worst case normal shock scenario. I then applied this pressure as the load in Solidworks FEA. I approximate strength and stiffness values for 3D printed PETG and used the weakened axis (along print lines) for my material.
{% include image-gallery.html images="Screenshot 2026-11-15 210022.png, Screenshot 2026-11-15 203856.png, Screenshot 2026-11-15 202449.png" height="300" %}
After reinforcement the part appears close to failure (under target safety factor of 1.5 in some regions. However if the part is fixed/glued to the side of the airframe it is much stronger. This tells me I need a more robust attachment or I need to epoxy the fairing the the airframe.

## Rapid Prototyping:
I used 3D printing and laser cutting to create a majority of the parts. The carbon fiber coupler and switch band that wrap the avionics bay required 3D printed jigs for hole placement.
{% include image-gallery.html images="B952BFA6-2221-4D18-8155-9E9BE47F1182_1_105_c.jpeg, 0F4361FC-3292-4290-A3F7-2518AF270423_1_105_c.jpeg" height="300" %}

## Cross-Functional Design:
As an avionics packaging project I have worked closely with our avionics division to determine their needs for antennae access, sensor needs, and battery sizing. 
{% include image-gallery.html images="85D1CE9E-64CF-4AEA-9C31-4F58DA261216_1_105_c.jpeg" height="300" %}
