---
layout: page
permalink: /projects/UEFC/
---
<img src="/assets/UEFC.png" alt="">

&nbsp;

## Unified Engineering Flight Competition

<p style="font-size:120%;color:gray;">Spring 2021</p>

For my sophomore spring semester, my Fluid Dynamics and Thermodynamics classes came together to host a "unified" engineering flight competition, where students worked in teams to design and build their own model aircrafts and compete for the best performance. For our year's flight competition, plane performance was judged by a combination of payload mass and speed, meaning students were incentivized to design lightweight, fast planes with high coefficients of lift while maintaining stability and structural integrity. The semester-long competition was divided into three distinct parts: a preliminary analysis, the design phase, and the build phase.

## Preliminary analysis

In the preliminary analysis, each team leveraged the aerodynamic models we learned in class and explored how different geometric parameters of an aircraft's wing affect key performance parameters such as lift, drag, required thrust, and material bending in steady level flight. Since there were a lot of potential parameters to analyze, such as taper ratio, thickness, aspect ratio, span length, chord length, and surface area, my team decided to write python scripts to automate the model calculations and the collection of data on expected performance. We used these findings, as well as our intuition, to select an optimal wing design.

## Design phase

Equipped with a better understanding of how geometric parameters affect flight performance, our team moved forward and tackled the design of a complete model aircraft. In constrast to the preliminary analysis, we now had to model the dynamics of the entire plane, accounting for the tail surfaces, fuselage, propellors, batteries, controllers, and all of their effects on flight behavior. We also employed more in-depth aerodynamic models, such as the vortex-lattice method, which we used to analyze lift distribution across the wingspan. Lastly, we accounted for stability parameters such as static margin and spiral stability, making sure our plane was steady and controllable in flight.

By prioritizing a lightweight, smaller design instead of a larger, more stable aircraft, we were able to cut off a significant amount of dead weight and maximize our payload carrying capacity. We arrived at the following design:

&nbsp;

<div style="text-align:center">
	<img src="/assets/UEFC_model_toscale.jpg" alt="" width="600">
</div>

&nbsp;

## Build Phase

The next section of the competition was the build phase, where teams were given materials and tasked with making an aircraft from their designs. Due to COVID rules, off-campus students such as I weren't able to participate in building the aircraft, but my teammates did a great job and we ended up with the following final product.

&nbsp;

<div style="text-align:center">
	<img src="/assets/UEFC_plane.JPG" alt="" width="600">
</div>

&nbsp;

## Flight Testing

After the build phase, teams participated in final flight testing to compete for the best performance. Scoring was based on how fast the plane could fly in a circle as well as how large of a payload the plane was carrying.

&nbsp;

### Click below to watch our plane perform in the final flight testing!

[<div style="text-align:center"><img src="https://img.youtube.com/vi/KYgn3RhLSrY/0.jpg" alt="" class="center" width="600"></div>](https://www.youtube.com/watch?v=KYgn3RhLSrY)

&nbsp;

## Results

Shown below is the performance spread across all of the teams. On the X-axis is each team's expected performance from the design phase. On the Y-axis is each team's actual performance in the final flight testing.

&nbsp;

<div style="text-align:center">
	<img src="/assets/UEFC_performance_distribution.png" alt="" width="600">
</div>

&nbsp;

As you can see above, our team (team 8) had the highest expected performance from the design phase, but we fell short in the actual flight performance. Our Professors speculated on a few possible causes, such as unintentional differences between our build and design model. Watching our flight test also suggests there was a possible stability issue.

However, overall ratings weren't determined by final flight performance alone. Teams were scored based off of their performances in both the design phase and the final flight testing. Although our flight didn't go as planned, we excelled in the design phase, so we were still awarded third place overall!

&nbsp;

<div style="text-align:center">
	<img src="/assets/UEFC_results.PNG" alt="" width="600">
</div>

&nbsp;

Our team's largest strength was likely our use of automation. In the design phase, we spent a lot of time deriving the general system dynamics and migrating equations into python, which allowed us to create a script to automatically solve for performance parameters as a function of design variables. This significantly sped up our design iteration time, allowing us to quickly come up with a design, analyze its performance, and improve on its shortcomings.

On the other hand, our team's biggest mistake was likely overlooking the stability parameters, not allowing a large enough safety cushion to ensure stable flight. In our final flight test, we saw a significant speed lost due to the pilot having to re-direct the plane on course after flight perturbations.
