---
layout: post
title: SwimEx Depth Select (Professional Product Design)
description: I worked on a team of two engineers to design and launch SwimEx's latest product line.
    The DepthSelect allows athletes and patients to use an underwater treadmill at any depth from 2' to 6'.
skills: 
  - FEA
  - Isotropic Approximation of Orthotropic Material
  - Dynamic Seal Design
  - Cross-Functional Design
  - Design for Composite Manufacture
  - FDM 3D Print Prototyping
  - Material Compatibility Research
  - Design for Serviceability/Repairability
main-image: /DepthSelect_Default.png
---
---

## The Problem:
Underwater treadmills use buoyancy to support joints and water viscosity to add resistance, making them effective tools for progressive recovery. Matching resistance to the specific needs of each athlete or patient requires precise depth control; this need drove the design of the DepthSelect.

## The Product:
The DepthSelect is an isolated unit installable in any large SwimEx pool. It allows one user to control their own depth while other users remain at full depth for separate activities in the same pool, improving the pool's cost-to-performance ratio by letting a single installation serve multiple training and recovery needs at once, rather than requiring separate dedicated units.

The current prototype drains its 7'6" x 4' x 5'6" chamber at a rate of 700L/min.

## Design:
Over six months as a design engineering intern at SwimEx, I played a key role in design decisions for the DepthSelect chamber and was one of two engineers responsible for early CAD development.

## Analysis:
I evaluated the strength of an acrylic wall, a steel supported acrylic wall, and a composite wall with acrylic windows using Fusion FEA. Comparing the performance of these solutions to price quotes our team decided to move forward with the fiberglass composite wall.

I did not have access to a purpose-built orthotropic FEA software, so I used an approximated isotropic Young's modulus to estimate our material properties, then modeled the layers of the composite schedule. To verify this I applied the method to a simple cantilever beam, then had a physical beam manufactured. Testing the physical beams deflection (our critical metric) against the FEA exposed a discrepancy and allowed me to tune my FEA to better match reality. To further validate the FEA I consulted a composite engineer from our fiberglass supplier. He helped us develop our final composite stack, and my tuned FEA was approximate to his hand calculations. 

This FEA served as a conservative estimate and set the maximum size of the chamber.

{% include image-gallery.html images="test-fea.PNG, IMG_1393.jpeg, wall-fea.PNG" height="300" %}

## Rapid Prototyping:
One of the most demanding parts of the design was the mechanical seal. Because fiberglass composites retain some flexibility, FEA predicted wall flex during draining and filling meaning the connection to the outer pool wall couldn't be a rigid bond. I developed a seal design that both acted as a simple support against the hydrostatic pressure, and allowed the wall to slide in the case of chamber flex.

I designed a full-scale cross section of the seal at the point where the wall meets the floor, then 3D printed it to test the seal design directly. This prototype validated the seal's performance, identified the most effective adhesive, and surfaced key design changes before we moved to a full-scale build. The 3D printed prototype validated the reliability of the seal with a two month static set. The full scale prototype functioned, the seal did not leak after several fill cycles and retained its capability for a one week static set.

## Full-Scale Prototype:
After months of FEA, regulatory research, design work, rapid prototyping, and market research, we began construction of a full-scale prototype using designs I developed and drawings I authored. I worked with our manufacturing manager for successful DFM, then supported manufacture. I am pictured below alongside SwimEx's Head Engineer in what became the first functional DepthSelect chamber.

{% include image-gallery.html images="IMG_1976.jpeg, 20260625_115324.jpg, Installed.jpeg" height="300" %}

## Cross-Functional Design:
Delivering a project of this scale required close coordination across teams. I worked directly with the SwimEx sales team, exchanging renders and design input to ensure the product met client ergonomic and aesthetic expectations. I sat in on client meetings and helped present the concept in its early stages to build market support, and regularly briefed SwimEx's finance and administrative teams on design progress, incorporating their input on timeline and budget.
