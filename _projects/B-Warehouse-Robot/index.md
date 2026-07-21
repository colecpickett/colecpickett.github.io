---
layout: post
title: Warehouse Storage Automation Robot (Prototype)
description: I designed, fabricated, and coded an autonomous robot prototype to automate package moves and organization within a controlled factory system.
skills: 
  - FDM 3D Printing
  - Fusion 360
  - Arduino
  - C++
  - Tolerance Analysis
  - Breadboard prototype PCB design

main-image: /Warehouse_Default.png
---
---

## The Problem:
Manual package handling and sorting within a factory system is slow and labor-intensive. An autonomous robot capable of navigating a fixed path and moving packages between designated ports offers a way to automate this process without requiring a fully custom industrial solution.

## The Product:
The result is an autonomous robot prototype built to move packages between fixed ports within a controlled factory layout. The robot uses line-following navigation to travel its route, an ultrasonic sensor to detect ports, and a scissor-lift mechanism to pick up and carry packages along the way.

## Design:
I designed the robot's chassis and scissor-lift mechanism in Fusion 360 and Solidworks, then manufactured the parts using FDM 3D printing. The system was powered and controlled by an Arduino, programmed in C++ to handle both navigation and lift actuation.

{% include image-gallery.html images="robot-cad.jpeg, robot-build.jpeg" height="400" %}

## Autonomy & Sensing:
To navigate independently, the robot combines a line-following program with an ultrasonic sensor for port detection — allowing it to travel a fixed route and stop precisely at each package port without manual intervention.

{% include image-gallery.html images="robot-final.jpeg" height="400" %}

## Results:
The completed robot successfully used its line-following program to navigate between package ports, picked up and carried packages using the scissor-lift, and reliably detected each port using the ultrasonic sensor — validating the full pick-up, transport, and drop-off cycle end to end.
