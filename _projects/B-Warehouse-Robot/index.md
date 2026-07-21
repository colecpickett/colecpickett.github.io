---
layout: post
title: Warehouse Storage Automation Robot (Prototype)
description: As part of a four-person team, I helped design, build, and program an autonomous 
    mobile robot capable of navigating a warehouse-style environment and transporting boxes 
    between shelves using a scissor-lift mechanism.
skills:
  - Fusion 360
  - Rack-and-pinion mechanism design
  - Scissor lift design
  - Arduino / C++
  - FDM 3D printing
  - Sensor integration (ultrasonic + IR)
  - Decision matrix analysis
  - Iterative design process
    
main-image: /warehouse-hero.jpg
---
---

## The Problem:
Warehouses lose significant time and money to inefficiencies in manual box handling, and warehouse work carries real safety risk — industry data shows tens of thousands of forklift and material-handling injuries occur annually. Our team, as part of Northeastern's Cornerstone of Engineering course, set out to design an autonomous mobile robot (AMR) that could transport boxes between shelves, reducing both inefficiency and the need for workers in repetitive, injury-prone roles.

## Research & Concept Selection:
We researched existing AMR systems, including GreyOrange's warehouse robots, to inform our design direction. Using a Duncker diagram and weighted decision matrices, our team evaluated multiple line-following path layouts and lift mechanism options before committing to a design — ultimately selecting a straight two-shelf path for reliability and a micro-servo-driven rack-and-pinion lift for precision and part availability over motor or alternative servo options.

## Design:
I contributed to the mechanical design of the robot's chassis, scissor-lift arms, and shelf system in Fusion 360. The lift went through three major iterations — from an initial proof-of-concept slider-and-rack mechanism, to a wider "double-wide base" supporting two parallel lifts, to a final version with added fillets for structural stability and refined tolerances on friction-prone surfaces. The drivetrain used four DC motors mounted to 3D-printed drive trays, paired with a sensor suite of one ultrasonic distance sensor and IR contrast sensors for line-following.

{% include image-gallery.html images="Warehouse_Default.png, scissor-lift-cad.png" height="300" %}

## Prototyping & Iteration:
We built and tested multiple physical prototypes throughout the semester. Early testing surfaced friction issues in the lift's top rail, prompting us to add clearance and tolerances in later prints. Final assembly and testing revealed a robot sag caused by added tolerances — with no effect on performance — along with several field fixes, including a quick-turnaround servo brace we designed and printed after the original servo mounts failed shortly before the deadline.

{% include image-gallery.html images="amr-cad.png, mechanical-drawing.png" height="300" %}

## Results:
The final robot successfully executed its full task cycle: following a line between shelves, detecting ports with its ultrasonic sensor, and lifting and placing boxes using the scissor mechanism. Millis-timer-based code allowed the robot to read sensor input and act in real time, and the 3D-printed chassis held up reliably through testing and the final demonstration.

{% include image-gallery.html images="final-1.png, final-2.jpg" height="400" %}

## Reflection:
Simplifying our warehouse layout and code logic paid off — the robot ran with fewer bugs than earlier, more complex iterations. Looking back, the team identified a rear-facing distance sensor and improved hook/servo design as the most valuable next steps for a future version, along with a larger, more complex warehouse layout to test scalability.
