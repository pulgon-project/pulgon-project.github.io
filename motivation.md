---
layout: page
title: Motivation
---

Modern civilization is in a state of continuous demand for new and more finely tuned task-specific materials, and the role of computational materials science in the search for new solutions can hardly be overstated. For most of the 20th century, new materials were often discovered by accident, and theoretical approaches used to focus on explaining their good performance with a view to improving them. Nowadays, however, it is possible and necessary to scan through large libraries of candidate materials and obtain predictive estimates of their performance in a particular application, study their stability, and propose entirely new possibilities for experimentation.
Thermal transport is an important concern in many of those applications. For instance, keeping the temperature of electronic and microelectronic devices under control is crucial for extending their lifetimes, requiring efficient thermal dissipation, whereas low-thermal-conductivity materials are required to improve the efficiency of thermoelectric energy conversion. Both cases call for semiconductors, where thermal transport by lattice excitations is the dominant contribution.

Among the many options available to build new materials, nanostructuring has proven to be a very fertile avenue to obtain new properties. Its potential has been recognized from very early in the development of materials science, as attested by Feynman’s remark that "there’s plenty of room at the bottom". As could be expected, it is also extensively used in natural functional blocks. Nanostructures occupy a middle ground between molecular systems and bulk materials. This is reflected, e.g., in their synthesis, which is tackled using tools from traditional chemistry as well as from surface science but also, critically, in their conceptual and computational treatment. The theoretical formalisms for molecules and for crystalline solids are extremely well developed and widely known, and extensive software ecosystems have evolved around both for many decades. Therefore, nanostructures
are usually tackled as edge cases of molecular systems or, more frequently, periodic three-dimensional crystals. This leads to a patchwork of workarounds and partial solutions to alleviate the problems introduced along with this artifactual periodicity. To the extent that those approaches solve particular problems and that most practitioners are familiar with them, there is a relatively low degree of awareness about the existence of fundamental incompatibilities between the 3D crystal model and the actual structure of nanosystems.

A paradigmatic example are the artifacts introduced in the phonon spectrum of a quasi-1D system when it is treated as a 3D crystal. The following figure shows the results for a MoS<sub>2</sub> nanotube near the Γ point; see [this reference](https://doi.org/10.1039/c9cp00052f) for details. Comparing the phonon bands obtained using an appropriate formalism (colored lines) with the artifactual results afforded by the 3D formalism (grey lines), six kinds of problems can be observed: 

1. There are three acoustic branches instead of four.

2. Artifactual pockets of imaginary frequencies appear close to the Γ point.

3. Degeneracies are spuriously broken.

4. Crossings/avoided crossings are mispredicted.

5. [The flexural vibrational branches are not quadratic](https://doi.org/10.1080/21663831.2016.1174163).

6. Large errors are introduced in the predicted speeds of sound.

<p align="center">
  <img src="/images/phonon_artifacts_plain.svg" alt="Scientific questions and objectives" width="100%">
</p>

In light of the above, materials science faces the paradoxical situation where awareness of the formalism required for the description of many nanomaterials is not commensurate with their acknowledged relevance. More importantly, general implementations are lacking. That is precisely the motivation for the PULGON project. The central goal is to throw light on important open problems in thermal transport in quasi-1D nanostructures from a symmetry-adapted perspective that can go beyond the state of the art in terms of physical insight, accuracy and system size. In the process, a general software framework will be created to study such structures that can have a long-lasting impact in the community.