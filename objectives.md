---
layout: page
title: Objectives
---

This project will develop the ability to systematically look at the physics of lattice thermal transport in quasi-1D systems with the scalability and level of detail afforded by the [line-group formalism](https://en.wikipedia.org/wiki/Line_group), overcoming the limitations of the 3D approach. It will shed light on issues of fundamental and technical importance for the design of next-generation electronic devices, and will enable significant avenues for further original work by removing the conceptual and practical limitations imposed by the makeshift approaches in current use.

The scientific aims of the project revolve around quasi-1D systems as candidates for energy recovery and heat transfer applications, where the fundamental aspects of thermal transport can determine the suitability of a proposed solution. Specifically, two sets of questions about particular systems will be tackled, shown below. In spite of their fundamental and technological relevance, these problems have not been addressed in enough depth because of the lack of an appropriate formalism. Therefore, they will also serve the dual purpose of showcasing the usefulness of line groups as a solution to current problems in materials science. Moreover, both of them will act as guiding threads for the development of general-purpose pieces of software to be released as open source. The main functional blocks of the software framework are also represented in the figure. Being structurally representative of the class of quasi-1D systems, showcasing the whole gamut of line groups, and having significant technological interest, nanowires (NWs) and nanotubes (NTs) and their thermal transport properties are the ideal targets for this project, and the research questions discussed below have been selected to maximize the transferability of the resulting solutions.

<p align="center">
  <img src="/images/puzzle_plain.svg" alt="Scientific questions and objectives" width="100%">
</p>

## Research question 1:

The first goal of this project will be to study lattice thermal transport in pristine Si NWs, i.e., in the absence of defects, to analyze the effect of diameter and symmetry on three-phonon scattering, the dominant component of anharmonicity in most bulk systems and the only one that is taken into account in most analyses. Besides providing a solid foundation for studies of quasi-1D thermal transport in the diffusive regime, this will also lead to a solver of the Boltzmann transport equation for quasi-1D structures built around [almaBTE](https://almabte.eu) that will be released to the community as open-source, and to the first version of the general-purpose line-group library at the core of this project. Next, the project will target Si and Ge NWs with defects on their surfaces. Instead of resorting to a Gaussian roughness model or even an atomistic treatment of random defects, here the possibility of controlled surface roughness with definite symmetries will be explored. Recent atomistic studies of defects in 3D have revealed that slightly different defects at the same concentration can have dramatically different effects on thermal transport through the phenomenon of [resonant scattering](https://doi.org/10.1039/C8TC00820E), which can be expected to be even more marked in one dimension, where defects can conceivably block phonon transport altogether. Defects introduce elastic scattering on top of the inelastic three-phonon scattering of perfect systems, and do so to a degree where a first-order perturbative treatment is woefully inadequate, as shown in 3D. Therefore, a byproduct of this second study will be a library for the study of elastic phonon scattering in quasi-1D systems that can be integrated with the Boltzmann transport equation.

## Research question 2:

Interfaces are the ultimate source of elastic scattering in that they derive from a mismatch between the spectrum at both sides and therefore cannot be treated as a bounded defect in
an otherwise periodic system. The software will be augmented with recently developed methods to deal with this problem and applied to the study of periodic arrays of atomically smooth interfaces created by crystallographic rotations in III-V semiconductor NWs, [known as crystal-phase and twin superlattices](https://doi.org/10.1039/C9NR05274G). This part of the project will be conducted in collaboration with the group of Dr. Riccardo Rurali at the ICMAB–CSIC in Barcelona. That group has accredited experience in the treatment of those systems at the ab-initio level and good contacts with experimental groups.

## Research question 3:

Regarding NTs, the work proposed here concerns itself with fully ordered structures based on Janus chalcogenide monolayers, building on the work already done on the vibrational properties [for the binary case](https://doi.org/10.1039/c9cp00052f). The goal is to use the phonon band structures to elucidate the synthesis parameters (chirality, diameter, composition) that should be targeted in applications with particular high thermal conductivity or high thermoelectric figure of merit requirements.

## Research question 4:

The fourth and final problem proposed is the exploration of thermal transport in multiwall NTs based on multilayers. With respect to single-wall NTs, this obviously increases the diversity of the class through the additional degrees of freedom afforded by stacking, and therefore expands the phase space for tuning thermal transport. Perhaps more importantly, the interactions between layers are generally dispersive, much weaker than the intralayer covalent bonds. Their contributions to the energy require a specific treatment. Moreover, weak interactions can increase anharmonicity to the point that the Boltzmann transport equation for phonons, where it is only treated perturbatively, loses its predictive power.

