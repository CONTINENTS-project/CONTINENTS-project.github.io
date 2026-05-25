---
layout: home
title: CONTINENTS
subtitle: International Centre-to-Centre Collaboration Project
permalink: /
---

**Title:** An Overview of the ECMWF's Data Handling Approaches

**Presenter:**  Nicolau Manubens, ECMWF and EPCC

**Abstract:**

Handling voluminous meteorological data for operational pipelines has associated challenges. This presentation will review the current data handling approaches for operational forecasting at ECMWF, starting by an introduction to the MARS ecosystem —a family of software services, tools, and libraries which enable operational applications to efficiently access meteorological data— where an index of the entire data domain is kept, and every two-dimensional data field can be referenced with a unique and scientifically meaningful identifier.
The presentation will first focus on the FDB library, which abstracts away the HPC file system behind the MARS language and is the operational backbone for data exchange. This will include a discussion on the suitability and performance of the DAOS and Ceph object stores as alternative storage backends for the FDB.

The presentation will then give an overview of Polytope, a technology recently developed by ECMWF which enables granular access to GRIB data (written by FDB or otherwise) with potential to dramatically improve efficiency of downstream applications that require data for specific geographical regions or data points; as well as ongoing developments to support Zarr access to FDB data.

Finally, this will discuss the results of a few I/O benchmarking experiments conducted in NCAR's HPC systems during Nicolau's (EPCC PhD student and ECMWF researcher) recent visit to NCAR, enabled by the CONTINENTS project, where a number of the presented data handling components were used in combination with the MILES-CREDIT framework for machine learning model training and inference.

**Date/Time:** [Thursday, 28th of May at 16h00 Mountain Time](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CONTINENTS+Webinar&iso=20260528T13&p1=1243&ah=1).

**Link:** [https://sundog.ucar.edu/public/page/CISL](https://sundog.ucar.edu/public/page/CISL)


{% comment %}
**New Date and Time**: TBC

**Title**: Scaling AI/ML Training Workflows for Earth System Prediction

**Presenter**: [Negin Sobhani][negins], [National Center for Atmospheric Research][NCAR].

**Abstract**:  

Artificial intelligence (AI) and machine learning (ML) are increasingly used in Earth system sciences, enabling faster modelling of complex physical processes and improved prediction of weather and climate. In recent years, fully data-driven AI/ML emulators have emerged that model the atmosphere—and other Earth system components—as a whole, offering the capability to generate global medium-range weather forecasts in minutes on a single GPU, a dramatic improvement over the computational demands of traditional Numerical Weather Prediction (NWP) models. Complementing these purely data-driven approaches, hybrid modelling strategies integrate physics-based models with AI/ML components, leveraging the strengths of both paradigms to improve predictive accuracy, enhance interpretability, and reduce computational costs while preserving physical consistency and improving the representation of subgrid-scale processes. Despite these advances, scaling AI/ML workflows to handle the massive, high-dimensional datasets characteristic of Earth system sciences remains challenging, often constrained by GPU memory limitations, I/O bottlenecks, and communication overhead inherent in distributed computing environments.

This presentation shares our experience in optimising distributed training workflows for large geospatial datasets to overcome these constraints. We explore strategies to mitigate severe I/O bottlenecks, highlighting the critical role of GPU-native dataloaders in maximising data throughput while minimising costly host-device transfers. We then detail how advanced parallelisation techniques, such as Distributed Data Parallel (DDP) and Fully Sharded Data Parallel (FSDP), combined with memory-saving methods like mixed-precision training and activation checkpointing, drastically reduce the GPU memory footprint. Finally, we discuss practical solutions for configuring communication backends (e.g., NCCL, MPI, Gloo) to ensure seamless data exchange across multi-node, multi-GPU HPC setups.

Our benchmarks demonstrate that integrating these optimisations leads to robust, scalable training workflows for large-scale geoscientific models and significant reductions in training time. Attendees will gain actionable insights and proven strategies for scaling their own AI/ML models, accelerating AI/ML based training for their workflows.


# Next webinar

**Date and Time**: [Thursday, 16th of March at 16h00 BST](https://www.timeanddate.com/worldclock/fixedtime.html?sort=2&p1=304&iso=20260416T1600&msg=CONTINENTS%20Webinar&ah=1).

[Download the calendar invite here](continents.ics).

{% endcomment %}

# Past webinars

**Title**: Accelerating Earth System Modeling by Leveraging a Standardized Coupling Framework for Hybrid Physics-ML Models

**Presenter**: [Ufuk Turuncoglu][ufukt], [National Center for Atmospheric Research][NCAR].

**Abstract**:  

Traditional Earth System Models (ESMs), while foundational to climate and weather research and applications, often face significant computational bottlenecks and struggle with accurately parameterizing complex sub-grid physical processes such as atmospheric convection, clouds, and radiation. Recent progress in Machine Learning (ML) and Artificial Intelligence (AI) provides a promising solution to these constraints by developing computationally efficient, data-driven surrogates for particular model components such as atmospheric solvers, sub-grid scale parameterizations, ensemble generation, and data assimilation to reduce biases.

This study presents a novel coupling architecture designed to seamlessly couple diverse ML-based model components with traditional physics-based Earth System Models to construct hybrid Earth system models with minimal effort. The proposed infrastructure and newly developed GeoGate co-processing component standardize the communication and interactions among the different types of model components, enabling asynchronous execution and flexible swapping of traditional physics components with their AI/ML-based data-driven counterparts to establish a true flexible hybrid modeling environment. We demonstrate that this generic coupling framework allows adaptation to different realistic ESM applications, such as regional configuration that couples atmosphere and ocean models to more sophisticated and multi-component applications that aim for Subseasonal-to-Seasonal (S2S) time scale global prediction. The proposed framework enhances model development flexibility, paving the way for the creation of next-generation computationally efficient and modular ESMs that can leverage the rapid innovation cycles of both physical and machine learning sciences in Earth system modeling while maintaining and, in some cases, improving simulation fidelity across various spatial and temporal scales.


[Recording][recording_ufukt]  
[Slides][slides_ufukt]

---

**Title**: Destination Earth: The Climate Change Adaptation Digital Twin

**Presenters**: [Ioan Hadade][ioanh] and [Sebastian Milinski][sebastianm], [European Centre for Medium-Range Weather Forecasts][ECMWF].

**Abstract**:  
We present the first digital twin framework that operationalizes the production of multi-decadal, global climate projections at kilometre-scale resolution, developed within the European Union’s Destination Earth initiative.
Using three coupled Earth system models and selected impact-sector applications, we have built end-to-end workflows for both regular and on-demand climate projections on two EuroHPC supercomputers, LUMI and MareNostrum5.
These workflows produced the first-ever multi-decadal simulations at 5 km resolution across all major Earth system components, using the same output parameters and grid, and achieving an average production throughput of 0.6 simulated years per day and a climate data portfolio of more than 10 petabytes.
We present the scalability of two of these Earth system models across both CPU- and GPU-based systems at global resolutions up to 1 km, across atmosphere, ocean, land, and sea-ice, and report full-machine performance on leading EuroHPC at record breaking efficiency at 1 km resolution.

[Recording][recording_ioanh]  
[Slides][slides_ioanh]

---

**Title**: Earth Embeddings: Learning Concept Maps in Neural Nets

**Presenter**: [Marc Rußwurm][marcr], [Wageningen University & Research][WUR].

**Abstract**:  
What makes a specific location unique? Traditional geospatial variables like temperature, land cover, or precipitation only tell part of the story — they are incomplete, coarse, and often hard to measure.
Instead, we can train AI to learn implicit representations of the planet directly from imagery and context.
This talk explores how geolocalization can serve as a powerful self-supervised training objective to build Earth Embeddings — dense, multimodal representations of the planet stored in neural networks.
By training models to play Satellite GeoGuessr, we teach them to infer a location’s coordinates from its visual appearance, forcing the network to capture the underlying environmental and societal patterns that make each place distinct.
The talk introduces two approaches: (1) neural location encoders, networks that map coordinates to continuous geospatial signals stored within network weights, and (2) SatCLIP Earth Embeddings, which align imagery and geolocation contrastively to produce rich embeddings encoding each location’s visual and contextual signature.
These learned concept maps act as a shared embedding space for environmental understanding — directly integrable into AI systems as location tokens or into scientific models as compact, learned representations of Earth.

[Recording][recording_marcr]  
[Slides][slides_marcr]

---

**Title**: Writing a complex atmosphere model, for a complex group of people, to run on complex architectures

**Presenters**: [Luca Bertagna][lucab], [Sandia National Laboratories][SNL] and [Aaron Donahue][aarond], [Lawrence Livermore National Laboratory][LLNL].

**Abstract**:  
EAMxx is the new atmosphere component of E3SM, the DOE flagship Earth System model.
It was built over a decade of work, starting by rewriting the spectral element dycore in C++, using the Kokkos library for on-node parallelism.
Following the dycore success, the whole atmosphere component was rewritten from scratch, including most of the physics parametrizations, as well as a full overhaul of the software infrastructure.

In this presentation we will discuss the choices behind the design of EAMxx.
We will discuss the clash of perspectives between software developers and domain scientists, the complex nonlinear iterations in the design and development cycles resulting from compromising the two point of views, and how software abstractions have helped in this process.

[Recording][recording_luca]  
[Slides][slides_luca]

---

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
[ufukt]: https://www.cgd.ucar.edu/people/ufuk-turuncoglu
[recording_ufukt]: https://media.ed.ac.uk/media/1_2gkovp0h
[slides_ufukt]: webinar_slides/2026-04-16_Ufuk_Turuncoglu.pdf
[negins]: https://www.cisl.ucar.edu/directory/negin-sobhani
[NCAR]: https://ncar.ucar.edu/
[ioanh]: https://orcid.org/0000-0002-9049-1952
[sebastianm]: https://orcid.org/0000-0001-5216-4662
[ECMWF]: https://www.ecmwf.int/
[recording_ioanh]: https://media.ed.ac.uk/media/t/1_ilfk8wk7
[slides_ioanh]: webinar_slides/2026-01-28_Ioan_Hadade.pdf
[marcr]: https://marcrusswurm.com/
[WUR]: https://www.wur.nl/en.htm
[recording_marcr]: https://media.ed.ac.uk/media/t/1_ha5f4r5w
[slides_marcr]: webinar_slides/2025-11-12_Marc_Russwurm.pdf
[lucab]: https://www.sandia.gov/ccr/staff/luca-bertagna
[SNL]: https://www.sandia.gov/
[recording_luca]: https://media.ed.ac.uk/media/t/1_qjhbcpwt
[slides_luca]: webinar_slides/2025-07-30_Luca_Bertagna.pdf
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
