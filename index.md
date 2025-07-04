---
layout: home
title: CONTINENTS
subtitle: International Centre-to-Centre Collaboration Project
permalink: /
---

# Next webinar

**Date and Time**: [Wednesday, 30th of July at 17h BST](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CONTINENTS+Webinar&iso=20250730T17&p1=304&ah=1).

**Title**: Writing a complex atmosphere model, for a complex group of people, to run on complex architectures

**Presenter**s: [Luca Bertagna][lucab], [Sandia National Laboratories][SNL] and [Aaron Donahue][aarond], [Lawrence Livermore National Laboratory][LLNL].

**Abstract**:  
EAMxx is the new atmosphere component of E3SM, the DOE flagship Earth System model.
It was built over a decade of work, starting by rewriting the spectral element dycore in C++, using the Kokkos library for on-node parallelism.
Following the dycore success, the whole atmosphere component was rewritten from scratch, including most of the physics parametrizations, as well as a full overhaul of the software infrastructure.

In this presentation we will discuss the choices behind the design of EAMxx.
We will discuss the clash of perspectives between software developers and domain scientists, the complex nonlinear iterations in the design and development cycles resulting from compromising the two point of views, and how software abstractions have helped in this process.

[Download the calendar invite here](continents.ics).

# Past webinars

**Title**: Performance portability on novel energy efficient architectures: feasible or fantasy?

**Presenter**: [Nick Brown][nickb], [EPCC][epcc]

**Abstract**:  
Whilst specialised hardware, often designed for AI, has the potential to provide significant performance and energy efficiency benefits, the programming of such technologies is far from simple.
Often involving new concepts and APIs, this requires at the very least expertise of the target hardware and significant changes to a code base - and not infrequently entire rewriting of kernels in new languages.

In short, scientific programmers have neither the expertise or inclination to port their codes to these specialist hardware, especially because work done targeting one architecture is often rather different from that required to target another.
Consequently, these programmability challenges are a major barrier to the HPC community gaining improved performance and/or energy efficiency.

In this talk I will describe work done in the compiler space, using MLIR, to address these programmability challenges.
By leveraging a composable compiler ecosystem, it is possible to more easily drive optimisations for these future architectures from existing languages and programming models such as extracting domain specific abstractions from code and leveraging OpenMP.

[Recording][recording_nick]  
[Slides][slides_nick]

---

**Title**: Towards Safe and Fearless Lossy Compression of Weather and Climate Model Data

**Presenter**: [Juniper Tyree][junipert], [INAR, University of Helsinki][uhelsinki]

**Abstract**:  
While the output volumes from high-resolution weather and climate models are increasing exponentially, data storage, access, and analysis methods have not kept up. Data size reduction is needed to avoid data storage cost concerns eventually restricting model development and use. Data compression is a vital tool for data size reduction. As lossless compression is no longer sufficient to produce the required compression ratios, lossy compression methods should be applied instead. However, as information loss can be scary - what if important details are lost - lossy compression has not yet been adopted by the weather and climate community.

As part of the [EuroHPC ESiWACE, Phase 3, Centre of Excellence](https://www.esiwace.eu/), we are working to make lossy compression safe and fearless by bridging the gap between advancements in lossy compression and safety concerns in weather and climate science. In this presentation, Juniper Tyree will provide an overview of the ongoing work on data compression that she leads in ESiWACE3: investigating and collecting safety requirements for lossy compression, benchmarking existing compression methods for performance and safety, and guaranteeing that user-provided safety requirements are upheld by lossy compression.

We believe that trusting lossy data compression requires convincing yourself by trying it out, on your own data, with your own analyses. We have thus developed an [open science online laboratory](https://lab.climet.eu) in which anyone can [conveniently explore data compression](https://compression.lab.climet.eu) without any setup. We provide this online laboratory as a service to the community to share computational examples, host interactive code documentation and research results, compression-related or not. We will provide a short live demonstration of this laboratory during the presentation.

[Recording][recording_juniper]  
[Slides][slides_juniper]

---

**Title:** The Ai2 Climate Emulator: Capabilities, Challenges and Opportunities

**Presenter:** [Oliver Watt-Meyer][oliverwm], [AllenAI][allenai]

**Abstract:**  
Ai2 Climate Emulator (ACE) is a fast machine learning model that simulates global atmospheric variability in a changing climate over time scales ranging from hours to centuries. It generates atmospheric phenomena such as the Madden Julian Oscillation, sudden stratospheric warmings, and tropical cyclones while also accurately simulating 20th century climate trends and El Niño-related interannual variability. Its efficient running 1500 simulated years per day on an NVIDIA H100 will make climate models more accessible and enable the generation of very large ensembles.

[Recording][recording_oliver]  
[Slides][slides_oliver]

---

**Title:** Exploring Dataflow Architectures for Improved Efficiency in Earth System Models

**Presenter:** [Justs Zarins][justsz], [EPCC][epcc]

**Abstract:**  
Earth system models are crucial for simulating environmental processes but demand significant computational resources and energy. In this presentation we will explore the potential of dataflow architectures to enhance both computational and energy efficiency of ESMs. We will primarily discuss the Cerebras Wafer Scale Engine, examining its capabilities and evaluating its suitability for the shallow water equation.

[Recording][recording_justs]  
[Slides][slides_justs]

---

[comment]: # Links
[lucab]: https://www.sandia.gov/ccr/staff/luca-bertagna
[SNL]: https://www.sandia.gov/
[aarond]: https://people.llnl.gov/donahue5
[LLNL]: https://www.llnl.gov/
[nickb]: https://www.epcc.ed.ac.uk/about-us/our-team/dr-nick-brown
[recording_nick]: https://media.ed.ac.uk/media/1_kpgo8jcg
[slides_nick]: webinar_slides/2025-06-26_Nick_Brown.pdf
[junipert]: https://researchportal.helsinki.fi/en/persons/juniper-tyree
[uhelsinki]: https://www.helsinki.fi/en/inar
[recording_juniper]: https://media.ed.ac.uk/media/1_ac1aq92p
[slides_juniper]: webinar_slides/2025-05-28_Juniper_Tyree.pdf
[oliverwm]: https://oliverwm1.github.io/
[allenai]: https://allenai.org/
[slides_oliver]: webinar_slides/2025-04-22_Oliver_Watt-Meyer.pdf
[recording_oliver]: https://media.ed.ac.uk/media/1_m2one45k
[justsz]: https://www.epcc.ed.ac.uk/about-us/our-team/dr-justs-zarins
[epcc]: https://www.epcc.ed.ac.uk/
[slides_justs]: webinar_slides/2025-03-13_Justs_Zarins.pdf
[recording_justs]: https://media.ed.ac.uk/media/1_hh95pqmp
