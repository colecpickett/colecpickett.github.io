---
layout: post
title: SwimEx Depth Select (Professional Product Design)
description: I worked on a team of two engineers to design and launch SwimEx's latest product line.
    The DepthSelect allows athletes and patients to use an underwater treadmill at any depth from 2' to 6'.
skills: 
  - FEA
  - Isotropic approximation of orthotropic material
  - Dynamic seal design
  - Cross-functional design
  - Design for composite manufacture
  - FDM 3D print prototyping
  - Material compatibility research
  - Design for serviceability/repairability
main-image: /DepthSelect_Default.png
---
---

## The Problem:
Underwater treadmills use buoyancy to support joints and water viscosity to add resistance, making them effective tools for progressive recovery. Matching resistance to the specific needs of each athlete or patient requires precise depth control — this need drove the design of the DepthSelect.

## The Product:
The DepthSelect is an isolated unit installable in any large SwimEx pool. It allows one user to control their own depth while other users remain at full depth for separate activities in the same pool — improving the pool's cost-to-performance ratio by letting a single installation serve multiple training and recovery needs at once, rather than requiring separate dedicated units.

The current prototype drains its 8'x4'x5'6" chamber at a rate of 400L/min, roughly 1 foot of depth change every 30 seconds.

## Design:
Over six months as a design engineering intern at SwimEx, I played a key role in design decisions for the DepthSelect chamber and was one of two engineers responsible for early CAD development.

## Analysis:
After evaluating an acrylic wall, we chose a composite wall to match the design language of the rest of the pool — introducing a new validation challenge. To address this, I developed an isotropic approximation of the orthotropic composite stack for use in Fusion 360 FEA. I validated this approximation against a physical test piece, and the FEA results proved accurate to within 15% of measured deflection.

{% include image-gallery.html images="IMG_1393.jpeg" height="400" %}

## Rapid Prototyping:
One of the most demanding parts of the design was the mechanical seal. Because fiberglass composites retain some flexibility, FEA predicted wall flex during draining and filling — meaning the connection to the outer pool wall couldn't be a rigid bond. I helped develop a design that supports and seals the wall while allowing it to slide.

I designed a full-scale cross section of the joint — the point where the wall meets the floor — and 3D printed it to test the seal design directly. This prototype validated the seal's performance, identified the most effective adhesive, and surfaced key design changes before we moved to a full-scale build.

{% include image-gallery.html images="IMG_1696.jpeg, IMG_1701.jpeg, IMG_1702.jpeg" height="400" %}

## Full-Scale Prototype:
After months of FEA, regulatory research, design work, rapid prototyping, and market research, we began construction of a full-scale prototype using designs I helped develop and drawings I authored. I helped oversee construction and am pictured below alongside SwimEx's Head Engineer in what became the first functional DepthSelect chamber.

{% include image-gallery.html images="IMG_1976.jpeg, 20260625_115324.jpg" height="400" %}

## Cross-Functional Design:
Delivering a project of this scale required close coordination across teams. I worked directly with the SwimEx sales team, exchanging renders and design input to ensure the product met client ergonomic and aesthetic expectations. I sat in on client meetings and helped present the concept in its early stages to build market support, and regularly briefed SwimEx's finance and administrative teams on design progress, incorporating their input on timeline and budget.
