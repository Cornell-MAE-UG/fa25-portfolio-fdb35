---
layout: project
title: MAE 2250 Open Design Project
description: Class project on client outline for design
technologies:
image: /assets/images/MAE2250/DesignSketch.png
---

---
# Design Process 
The following document describes our teams design process to address the problem of Spotted Lanternflies in Upstate NY grape vineyards. Specifically addressing the subproblem: Spotted Lanternfly presence during mechanical harvesting.

Our product has evolved iteratively and undergone meaningful changes through our design process as we have recieved feedback from our clients and evaluated our prototypes. 

---

## Table of Contents
- <span style="font-size: 1.5em;">[Client Outline](#client-outline)</span>
- <span style="font-size: 1.5em;">[Functional Prototype](#functional-prototype)</span>

---
<a id="client-outline"></a>
<h1 style="color:#000080; font-weight:1200;">Client Outline</h1>


**Team:** Tree of Hell. **Client(s):** Cornell CALS Extension/E&J Gallo Winery/National Grape

####  Problem statement:

Currently for growers in upstate NY during the harvest process of vineyards, **Spotted Lanternfly (SLF) presence in grapes during the mechanical harvesting process** is contaminating the product. Trivial solutions are ineffective due to harvested grapes being partially liquified during collection and high quality standards of product. 

####  Impact:
We address the problem at a single point in the harvest process. The single modular attachment lowers cost and enables more efficient harvest by minimizing wasted and dumped product. 

####  Proposed direction:
During the harvest process before collection, separate juice from the grape-bug mixture, then separate bugs from grapes. Then, combine the grapes and juice once again in the collection. 

##### Primary Concept:
**What it is:** Pressurized water tunnel to separate grapes and SLFs. Can use water pressure (Figure 1) or centrifugal force (Figure 2). Filter juice, then filter SLFs, then remix juice/grapes.

**How it would be used:** Apparatus placed in-line between harvester and collection systems.

**Why it’s better than the status quo:** Prevents any SLFs from entering the final harvest collection and saves any excess or needed grape juice for product production.

**End-of-semester proof-of-concept:**
Prototype of water tunnel with filters. Grapes flow through and SLFs are successfully separated.

####  Key risks / unknowns:
- Altering safety/functionality of the harvesters - We will research rules and regulations for harvesters, and create a modular design that fits without interfering with the harvester.
- Buildup of grapes during filtration process - We’ll ensure the prototype can manage the upper limit of the harvester’s collection rate and/or have a staging area so that it meets that standard.
- Growers are not willing or able to install our design. We will ensure grower feedback is incorporated and maximize user-friendliness by testing ease of use with strangers.

####  Questions for the client:
1. **Precisely when and where are grapes partially liquified during the harvest process?**  
   We need to know when liquid is present and the state of the grapes in the grape mixture throughout the harvest to determine the best way to filter SLF out.
2. **Which harvesters (models) and designs are frequently used in upstate NY?**  
    We need to know harvester designs to decide where in the process to insert our product. Is harvesting and containing done by two different vehicles or trailers, or by one unit?
3. **How willing and able are farmers to implement new technology in harvest?**
     Rank the importance of efficiency, reliability, repairability, durability, and ease of use for the end user (1 through 5). Add any other attributes deemed critical for grower-friendly design. 


####  Figure

<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/MAE2250/PosterSketch.jpg' | relative_url }}" 
       alt="Preliminary sketches of prototype ideas developed so far."  
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Preliminary sketches of prototype ideas developed so far.</strong>
  </figcaption>
</figure>

---
<a id="functional-prototype"></a>
<h1 style="color:#000080; font-weight:1200;">Functional Prototype</h1>


####  Design Documentation:
####  Overview:
The design consists of a perforated tray supported by an adjustable aluminum frame and stabilized using a cable suspension system. The perforated PVC sheet acts as the filtration surface, allowing grape juice to pass through while retaining larger solids. This sheet is supported by aluminum rods which distribute the load and prevent excessive sagging. The rods are connected to a vertical frame constructed from aluminum rectangular tubes, which provide structural support and allow for height adjustability. The height adjustment mechanism is achieved by drilling multiple holes into the vertical tubes and inserting dowel pins through aligned holes to lock the structure at different positions. This enables adaptability to different gondola heights and working conditions in the field. Aluminum edge trim is used as an interface to attach the system to a gondola, ensuring that the prototype can be integrated into a real harvesting setup.
The cable system plays a critical role in both load distribution and motion control. Cables connect the tray to the frame, introducing tension-based support that reduces bending stress on the rods and allows for slight compliance under load. This compliance is beneficial, as it absorbs shock when grapes are dumped onto the tray and prevents sudden structural loading. The combination of rigid members (rods and frame) and flexible members (cables) creates a hybrid structure that efficiently manages forces.

<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/MAE2250/DesignSketch.png' | relative_url }}" 
       alt="Preliminary sketches of prototype ideas developed so far."  
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Sketch of prototype.</strong>
  </figcaption>
</figure>

<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/MAE2250/Prototype1.png' | relative_url }}" 
       alt="Preliminary sketches of prototype ideas developed so far."  
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Functional prototype.</strong>
  </figcaption>
</figure>

<div style="text-align:center; margin: 20px 0;">
<iframe width="367" height="653" src="https://www.youtube.com/embed/P9xF8VgrA7M" title="IMG 4884" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Video of Oscillation Test</strong>
  </figcaption>
</div>

##### Components: 
- PVC Perforated Sheet (24” x 24”; 0.188” Diameter Hole to Hole Center); McMaster Code: 92985T53
- Aluminum Rods (½” Diameter; 8’ Length); McMaster Code: 8974K28
- Aluminum Rectangular Tubes 
     - Inner Tube: 1 ⅛” Height and Width; McMaster Code: 6546K5
     - Outer Tube: 1 ⅜” Height and Width; McMaster Code: 6546K1
- Cables (found in the lab)

##### Fabrication: 
The aluminum rectangular tubes were drilled to create holes for the adjustable height mechanism, ensuring proper alignment for dowel pins. The aluminum rods and rectangular tubes were cut to size to form the tray supports and future dowel pins. 

##### Mechanical Functionality: 
The system exhibits both vertical and lateral motion characteristics due to its partially suspended design. In the vertical direction, the tray supports the applied load through a combination of bending in the aluminum rods and tension in the cables. The cables reduce the effective load on the rods by redistributing forces to the frame, allowing the system to support higher loads without excessive deformation. Future modifications will allow an adjustable height of basket. In the lateral direction, small oscillations occur when the tray is loaded, but these are limited by the tension in the cables and the stiffness of the frame. This slight movement is beneficial, as it prevents stress concentration and allows the system to dynamically respond to uneven loading.
Load transfer occurs through multiple paths: the applied load is first carried by the perforated sheet, then transferred to the aluminum rods, which experience bending. From there, forces are shared between the cables (tension) and the frame (compression). This multi-path load distribution improves overall structural performance and reduces the likelihood of failure in any single component. The system is self-supporting, with the frame providing a stable base and the cables enhancing load distribution and stability.

##### Assembly: 
The assembly of the prototype was designed to be modular, adjustable, and easy to reconfigure. The primary structure consists of a telescoping frame made from aluminum rectangular tubes, where a smaller tube is inserted inside a larger tube. This nested configuration allows the inner tube to slide vertically, enabling height adjustment of the system. Once the desired height is reached, aligned holes in both the inner and outer tubes are secured using aluminum dowel pins, locking the frame in place and preventing unintended movement. After establishing the frame height, aluminum rods are positioned horizontally to support the perforated PVC tray, which is cut to size and aligned with the structure. Cables are then attached from the tray corners to the upper portions of the frame, creating a tension-based support system that helps distribute load and stabilize the tray while still allowing slight compliance. Finally, aluminum edge trim is attached to provide an interface for mounting the system onto a gondola. This assembly approach allows for quick adjustments, secure locking, and efficient setup, making it well-suited for both testing and real-world application.

<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/MAE2250/AssemblyPrototype.png' | relative_url }}" 
       alt="Preliminary sketches of prototype ideas developed so far."  
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Assembly sketch.</strong>
  </figcaption>
</figure>

####  Design Tests:
To evaluate the structural performance of the prototype, a load-bearing test was conducted by distributing various weights evenly across the tray to simulate the weight of a grape harvest. Under this loading condition, the system demonstrated high strength and reliability, with minimal deflection observed in the aluminum rods and no signs of failure in the cables or frame. The load was effectively distributed through the combined action of the rods in bending and the cables in tension, confirming that the hybrid support system is capable of handling realistic operating conditions. This will continue to be used for future iterations of our prototype. 

In addition to static loading, a forced swinging test was performed by manually displacing the tray and allowing it to oscillate. This test evaluated the system’s dynamic stability and response to sudden movements, such as those that might occur during harvesting or transport. The tray exhibited controlled oscillations without excessive amplitude, and the motion gradually damped due to cable tension and structural resistance. The oscillations were easily allowed in the desired direction and restricted in the other due to the cable design. No loosening, detachment, or instability was observed, indicating that the system maintains integrity under both static and dynamic conditions. This dynamic system will continue to be used for future iterations of our prototype. 

The dowel system showed promise in the strength tests. However, there was some difficulty fitting the planned aluminum dowels into the slot, so pencils had to be used instead for now. This test showed us that in future iterations the dowels will need to be machined down on the lathe to have a cap and a slightly thinner diameter. 

####  Success Criteria: 
The primary success criterion is filtration effectiveness, defined as the ability to separate at least 80% of the liquid from solid material, which can be measured by comparing the volume of collected juice to the initial mass of crushed grapes. Another key criterion is load capacity, where the system must support at least 15 kg without structural failure or excessive deformation, verified through incremental loading tests such as the rock distribution experiment. Stability is also important, with the requirement that the system does not tip or excessively shift under uneven loading conditions. Adjustability is evaluated based on the ability to change the height of the tray within one minute using the dowel pin system. Finally, ease of integration is measured by how quickly and securely the system can be attached to a gondola, with a target time of under two minutes.
For demonstration purposes, the prototype can be evaluated by pouring a grape-like mixture including SLF models  onto the tray and visibly observing the separation of liquid through the perforated sheet. The effectiveness can be quantified by measuring the volume of liquid collected within a fixed time interval, such as 30 seconds, and by ensuring no SLF models make it through and thus contaminating the juice with the quassinoids.


####  Future Improvements/Conclusion:
The prototype successfully demonstrates a functional and mechanically sound approach to separating grape juice from solids. The system is strong, adjustable, and capable of supporting realistic loads, as evidenced by the rock distribution tests. The use of a hybrid structure combining rigid and flexible elements provides effective load distribution and resilience. Our final design will incorporate an integrated motor system to actively generate controlled oscillations in the tray, enhancing the sifting behavior and improving the separation efficiency between grape juice and solids. By introducing consistent, tunable vibrations, the system will promote faster liquid flow through the perforations while preventing clogging from skins and stems. In addition, the final iteration will utilize aluminum edge trim to securely attach the structure to the field gondola. This will improve overall stability, ensure proper alignment during operation, and make the system more practical for real-world vineyard integration.
