---
layout: project
title: ENGRD 2210 Portfolio Assignment
description: Class project with Graphs
technologies: [Thermodynamics]
image: /assets/images/ENGRD2210/tower.png
---

## The assignment:
Please select a real-world instance of a device or system that we have learned about in this course, explain how it works in detail, and then discuss how its performance would change under a change in design or operating conditions. Your report should include:

-   photos and schematics of the device or system
-   a qualitative description of the device or system
-   a system diagram of the device or system operating (either CV or CM), showing work and heat transfer interactions as well as any relevant mass flows
-   mass balance, energy balance, and entropy balance equations (as relevant) capturing the physics more central to the device or system operation
-   describe a change to device or system design or operating conditions and then how that change influences device performance

## Nuclear Power Plant Cooling Towers & The Palo Verde Generating Station:

{% assign figure_counter = 0 %}

{% assign figure_counter = figure_counter | plus: 1 %}
<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/ENGRD2210/birdview.jpg' | relative_url }}" 
       alt="Aerial view of Palo Verde Generating Station outside Phoenix, AZ. Note the layout of 3 cooling towers for each of the 3 reactors." 
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Figure {{ figure_counter }}:</strong> Aerial view of Palo Verde Generating Station outside Phoenix, AZ. Note the layout of 3 cooling towers for each of the 3 reactors.
  </figcaption>
</figure>

This report will cover the design and operation of the cooling towers used in thermal power plants and particularly those associated with nuclear energy. Although design can vary drastically, hyperboloid cooling towers and their derivatives are commonly associated with nuclear plants. The Palo Verde Nuclear Generating Station outside of Phoenix, AZ will be used as a case study to analyze the effects of climate on these cooling towers. The Palo Verde plant was the largest nuclear single site facility in the US (until 2024) generating on average 32,000,000 megawatt hours annually [1]. One of nine plant cooling towers can be seen below:

{% assign figure_counter = figure_counter | plus: 1 %}
<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/ENGRD2210/tower.png' | relative_url }}" 
       alt="One of the nine Marley Class 700 cooling towers used at the Palo Verde Generating Station" 
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Figure {{ figure_counter }}:</strong> One of the nine Marley Class 700 cooling towers used at the Palo Verde Generating Station.
  </figcaption>
</figure>


The plant is a Pressurized Water Reactor (PWR) that follows the general system diagram shown below:

{% assign figure_counter = figure_counter | plus: 1 %}
<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/ENGRD2210/PWR.png' | relative_url }}" 
       alt="Typical Pressurized Water Reactor (PWR) system layout" 
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Figure {{ figure_counter }}:</strong> Typical Pressurized Water Reactor (PWR) system layout [2].
  </figcaption>
</figure>


The towers act as heat exchangers (condensers), and the relevant system loop (the steam generator loop) they are involved in can be modelled as a Rankine cycle. The towers cool hot steam coming out the turbines and turn it back into liquid water before entering the pump and later the hot heat exchanger between the inner reactor and outer generator loop. The rankine cycle can be visualized below:

{% assign figure_counter = figure_counter | plus: 1 %}
<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/ENGRD2210/Rankine.png' | relative_url }}" 
       alt="Control mass Rankine cycle of the generator loop" 
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Figure {{ figure_counter }}:</strong> Control mass Rankine cycle of the generator loop.
  </figcaption>
</figure>

We can calculate an approximate rate of heat transfer of these cooling towers by using the first law of thermo dynamics and modelling them as a control volume system. The water flow through 1 of 3 cooling systems (three towers per reactor unit) is approximately 580,000 gallons of water per minute or 12,185 kg/s of water per tower using 1kg = 1L of water [3]. The temperature of the hot water in is reported to be 48.2°C and the water temperature out is 30.7°C [3]. Note, this temperature difference may seem low for a nuclear reactor, but it is important to note the sheer scale of the water throughput these towers experience. Additionally, it is important to note that the cooling towers at Palo Verde are not passive, and do include mechanical draft systems (fans). However, the electricity required compared to the generation of a nuclear reactor is negligible and thus will be assumed to be 0. Additionally, potential and kinetic energy changes are approximated as 0. For now we will ignore mass exiting the system as evaporation and treat the device as a black box, but this will be revisited later. Specific heat capacity of water is approximately 4184 Joules per kilogram Kelvin.

{% assign figure_counter = figure_counter | plus: 1 %}
<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/ENGRD2210/Cooling.png' | relative_url }}" 
       alt="Control volume diagram of cooling tower for piped water" 
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Figure {{ figure_counter }}:</strong> Control volume diagram of cooling tower for piped water.
  </figcaption>
</figure>

Under these assumptions, we can use the first law to find heat transfer rate out of the tower: 

$$
\begin{aligned}
\dot{E} &= \dot{Q}_{\text{tower}} - \dot{W} + \dot{m}_{\text{water}}(h_i - h_e) \\
\dot{Q}_{\text{tower}} &= - \dot{m}_{\text{water}} c_p (T_i - T_e) \\
|\dot{Q}_{\text{tower}}| &= 12185 \cdot 4184 \cdot (48.2 - 30.7) \\
|\dot{Q}_{\text{tower}}| &\approx 892 \cdot 10^6 \ \text{W} = 892 \ \text{MW}
\end{aligned}
$$

With the cooling tower, we can find the efficiency of the site using formula:

$$\eta = 1 - \frac{|Q_{out}|}{|Q_{in}|}$$

Note the thermal energy of a single PWR core at Palo Verde is stated to be 3990 thermal MW. With three reactors and nine cooling towers (three per reactor) We find the efficiency to be:

$$\eta = 1-\frac{892\cdot9}{3990\cdot3} = 0.329$$

We can confirm this number using the average annually generated power by the plant, 32,000,000 megawatt hours per year ($$\approx3653$$ MW).

$$\eta = \frac{|W_{net}|}{|Q_{in}|} = \frac{3653}{3990\cdot3} = 0.305$$

Thus the efficiency estimates using the cooling towers and the Rankine cycle model excellently match those calculated using raw power and thermal data. This confirms the simplified Rankine cycle is a good model for the very complex nuclear plant.

The actual net efficiency is expected to be below the one achievable assuming perfect cooling to power ratios as power plants themselves require significant energy to run. This is called \"auxiliary power\" and includes everything from running the mechanical draft cooling towers, pumps, safety systems, air conditioning, lights, and much more. This was not included in estimates based on cooling as work was set to 0 in the energy balance of the cooling towers, but is typically 5% [4]. Note, both estimations are engineering estimates based on actual heat or work flow and not a theoretical estimate, such as found with carnot efficiency.

Now we will evaluate the more complicated case considering the evaporation of water from the cooling tower. We will be calculating the evaporation rate of the towers given the needed cooling rate found previously. At the Palo Verde plant, water is taken from an external, artificial reservoir to compensate for the water lost as evaporation [3]. These reservoirs can be seen in Figure 1. Uniquely, Palo Verde is the only nuclear facility in the world not located on or near a natural body of water and entirely depends on the treated municipal effluent (grey water) from Phoenix, AZ [1]. However, all water in the arid Southwest is extremely valuable and any water lost through evaporation is water not able to be used in irrigation, industrial applications, or further purification. Thus, it is critical to track the loss of this resource through evaporation. To do so, we will assume reservoirs to be the same temperature as the average ambient temperature. The following device control volume is shown is used:


{% assign figure_counter = figure_counter | plus: 1 %}
<figure style="text-align: center; width: 100%;">
  <img src="{{ '/assets/images/ENGRD2210/Cooling.png' | relative_url }}" 
       alt="Control volume diagram of cooling tower for evaporation of water" 
       style="width: 100%;">
  <figcaption style="text-align: center; font-size: 0.9em; color: #2b2b2bff;">
    <strong>Figure {{ figure_counter }}:</strong> Control volume diagram of cooling tower for evaporation of water.
  </figcaption>
</figure>


Using the same assumptions as above except that steam is no longer negligible and is the sole source of cooling, the 1st law for this device can be written as follows:

$$\dot{E}=\dot{Q}_{tower}-\dot{W}+\dot{m}_{in,resevoir}(h_{res})-\dot{m}_{out,evap}(h_{evap})$$
Assume steady-state conditions such that
$$\dot{m}_{in,resevoir}=\dot{m}_{out,evap}=\dot{m}_{evap}$$. Therefore,

$$\dot{Q}_{tower}=\dot{m}_{evap}(h_{evap}-h_{res})$$

To estimate $$h_{evap}$$ and $$h_{res}$$, steam tables will be used. To find $$h_{evap}$$, $$h_{fg}$$ at the temperature $$T_{in}=48.2$$°C gives $$h_{evap}\approx2382.7$$ kJ/kgK. Under the assumptions stated, $$h_{res}$$ follows climate data and thus operating conditions change according to season. We will consider the two extremes of January and July. The average temperature in Phoenix in January is 13.5°C and in July is 34.5°C. This gives the corresponding approximated values using saturated liquid enthalpies of $$h_{winter}=54.60$$ and $$h_{summer}=146.68$$ kJ/kgK, respectively. Using $$|Q_{tower}|$$=892MW we get the following evaluations:
$$h_{evap}$$
$$
892 \cdot 10^6 = \dot{m}_{\mathrm{evap,winter}} (2382.7 - 54.60) \cdot 10^3 \rightarrow \dot{m}_{\mathrm{evap,winter}} = 383.14 \text{ kg/s}, \quad
$$
$$
892 \cdot 10^6 = \dot{m}_{\mathrm{evap,summer}} (2382.7 - 146.68) \cdot 10^3 \rightarrow \dot{m}_{\mathrm{evap,summer}} = 398.92 \text{ kg/s}
$$


As one might expect, the summer evaporation rate is higher than that in winter. Critically, we just thermodynamically proved that for the same cooling rate, increased water consumption is needed during the driest part of the year. This corresponds to roughly 18200 to 18900 gallons of water per minute across the year per unit (3 towers). This is actually a very accurate estimate as actual evaporation values range from 13,500 gal/min-18,500 gal/min, per unit depending on the time of year [3]. The lower bound in winter is likely due to difference in humidity, dew point, and increased efficiency due to colder water not accounted for in the above calculations. With three units, the water consumption can be immense during the summer.

Ultimately, an analysis of nuclear power plant cooling towers and specifically that of the Palo Verde Generating Station has been given. Heat exchange rate, nuclear plant efficiency, and evaporation rate has been calculated and verified using data that is easily tracked at the plant. Varying operating conditions in the form of climate and its impacts on cooling towers has been considered. Detailed system and device behavior has been successfully modelled.

## References
[1] Howard Kaikow. The PALO VERDE WATER CYCLE MODEL (PVWCM) DEVELOPMENT OF AN INTEGRATED MULTI-PHYSICS AND ECONOMICS MODEL FOR EFFECTIVE WATER MANAGEMENT. [Online; accessed 2025- 11-23].

[2] NRC . Pressurized Water Reactor (PWR) Systems. https://www.nrc.gov/reading-rm/basic-ref/students/for-educators/04.pdf. [Online; accessed 2025-11-23].

[3] Caroline. An oasis filled with grey water. https://www.neimagazine.com/advanced-reactorsfusion/an-oasis-filled-with-grey-water/, jun 25 2013. [Online; accessed 2025-11-23].

[4] U. S. Energy Information Administration . Monthly Energy Review October 2025. https://www.eia.gov/totalenergy/data/monthly/pdf/sec8 n.pdf. [Online; accessed 2025-11-23].