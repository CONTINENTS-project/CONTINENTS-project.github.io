---
layout: page
title: CONTINENTS
subtitle: International Centre-to-Centre Collaboration Project
permalink: /about
---

# The CONTINENTS project

The CONTINENTS project is an EPSRC funded project, headed by [EPCC](https://www.epcc.ed.ac.uk/), the supercomputing centre at the University of Edinburgh, and in collaboration with the [National Centre for Atmospheric Science](https://ncas.ac.uk/) in the UK and the [National Center for Atmospheric Research](https://ncar.ucar.edu/) in the USA.

This ambitious collaborative programme of research, CONTINENTS will drive innovations in data centre and system operation, optimal exploitation of hardware, machine learning applied to data analysis and numerical modelling, and software design and implementation strategies, with the aim of minimising energy consumption and improving compute efficiency.

EPCC, NCAS and NCAR are creating an interdisciplinary collaboration between world leading centres of HPC research and service provision, atmospheric science experts, and numerical and machine learning application developers.

# The work streams

The different activities of the CONTINENTS projects will focus on the following six different work streams.

### Collaboration and Knowledge Exchange

We aim to deliver a broad programme of activities, including online webinars of topics relevant to the other project work streams, biannual workshops at major conferences, and research visits and secondments for technical staff and PhD and MSc students.

### Operational Efficiency of Data Centres

Data centres are the foundation for all large scale HPC activities undertaken by academia and industry.
The sizes can vary from small rooms with a single rack of equipment to large, multi-room, purpose-built buildings requiring tens or hundreds of megawatts of power.

Cooling and power distribution overheads consume energy above what is required to operate the compute hardware itself.
This work stream will research power distribution, cooling, and data centre configuration alternatives to evaluate how to decrease the overheads of power and cooling distribution across a range of hardware, climate conditions, and workloads.

### Efficient and Specialised Hardware

Custom hardware design and manufacturing has seen increasingly lower costs recently, which has lead to the emergence of large areas of specialisation in compute workloads, including Machine Learning.
This has lead to an increase in the availability of specialised hardware, such as Cerebras wafer scale engines, AMD Xilinx AI engines, Graphcore IPUs, RISC-V, etc.

However, specialised hardware is hard to use effectively in existing workflows and applications, partly due to the inertia and cost associated with adapting large code bases, and partly due to the heterogeneity of computational workloads, making it difficult to exploit such hardware efficiently across large HPC systems.
This work stream will investigate the impact, in both performance and energy use, of new and prototype level hardware systems for HPC and ML workloads, we will performance/energy models and quantify best practise to aid mapping applications to specialised custom accelerators and processors, and we will help improve software support for application offloading and decomposition.

### Software Abstractions for Energy Efficiency

To help scientists make efficient use of the hardware described above, it is essential to enable scientific programmers to describe algorithms in an abstract manner.
Software abstractions are a rich source of information that allows compilers to make low level decisions around parallelism and hardware-specific tuning.
This work stream will leverage the MLIR/LLVM compiler technology stack to enable a common underlying ecosystem and interoperability across hardware.

### Data Movement and Locality

Data movement, in an HPC context, is expensive.
Moving data within memory hierarchies in a compute node can be orders of magnitude more expensive (in both energy, and time) than computing on the data.
Once data needs to move outside a node, across a network or to filesystems and other external storage, the cost increases even more.
Single applications usually apply optimisations that ensure that data locality is exploited as much as possible, but users oftentimes deploy workflows of multiple applications that operate on the same data.

This work stream will research tools and techniques that could enable data movement and locality optimisations to the entire data life cycle, to minimise the costs of increasingly complex workflows.

### Leveraging Machine Learning

Machine Learning (ML) approaches applied to numerical applications have the potential to significantly speed up a range of computational kernels by learning desired responses to a range of input data.
This is challenging both in terms of result robustness and the computational cost of generated the trained ML models.

This work stream will evaluate the costs and benefits of ML use in weather and climate research, optimise the training costs for computational simulations in atmospheric science, and finally explore the theoretical integration of ML inference and re-training procedures in traditional scientific workflows.
