---
permalink: /research/
title: "Research"
author_profile: true
---

{% include toc %}
{% include base_path %}

## Introduction

My REU summer project (Northwestern University, 2025) was to use the N-body integrator REBOUND to test the predictions of Laplace-Lagrange secular theory for the evolution of eccentric, self-gravitation protoplanetary disks. We found that REBOUND performs best with sharp edges, whereas tapered edges cause discontinuities and premature divergence from theory. However, we further discovered that this effect can be offset by proper mass scaling, as lower masses cause the simulation to maintain the modes for longer. Through these comparisons, we hope to further reveal the parameter choices necessary to trust REBOUND’s output and the physical consequences of different disk edge profiles. 

## Results

We tested the three edge profiles (see Figure 1) across 3 disk mass scalings, $10^{-6} M_\odot$, $10^{-7} M_\odot$, and $10^{-8} M_\odot$. We found that sharp disk edges preserve secular modes best, but lowering the disk mass can offset even poor edge profiles.

![Scaled surface densities]({{ base_path}}/images/density.png)
Figure 1: Scaled surface density $\sigma$ profiles of simulated disks

![Erms]({{ base_path}}/images/erms.png)
Figure 2: Growth of eccentricity RMS for three edge profiles across disk masses. Sharp edges most faithfully follow the expected secular trend, while tapered edges introduce faster eccentricity growth. At high disk masses, all profiles experience fast eccentricity growth. Extended Taper produces ejections (e ≥ 1). At intermediate mass, Sharp and Tapered maintain coherence somewhat longer, while the Extended Taper still fails early. At low mass, all profiles remain closer to the expected secular mode.

![pomega]({{ base_path}}/images/pomega.png)
Figure 3: Evolution of mean π for edge profiles across disk masses. Black line represents the expected precession rate as calculated by Laplace-Lagrange (LL) theory. At high disk masses, all profiles diverge rapidly. At intermediate disk masses, simulations maintain coherence for longer, but eventually diverge prematurely. At lower masses, all profiles approximately maintain the initial mode for the duration of the simulation.

For realistic protoplanetary disks, which are unlikely to feature perfectly sharp edges, these findings imply that disk mass may act as a governing factor in whether large-scale eccentric modes can persist over observable timescales. This provides a physical framework for interpreting observed eccentricities in disks, as both the sharpness of edges and the total mass content need to be considered in tandem.

Future work will focus on quantifying the dependence of mode lifetime on disk edge steepness, total disk mass, and disk width. Given these established parameters for mode coherence, we will then explore how various tapered edges evolve in time in comparison to sharper edges to gain a better understanding of the evolution of protoplanetary disks. Ultimately, these insights will help bridge the gap between idealized secular theory and the complex, noisy environments in which young planetary systems evolve. 


## Presentations & Publication

I presented initial results as a poster at a symposium at the end of the internship. 


Download: [PDF]({{ base_path }}/files/Final Poster.pdf)
