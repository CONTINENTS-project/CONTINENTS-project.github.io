---
layout: page
title: Webinars
---

# Upcoming webinars

**Title:** An Overview of the ECMWF's Data Handling Approaches

**Presenter:**  Nicolau Manubens, ECMWF and EPCC

**Abstract:**

Handling voluminous meteorological data for operational pipelines has associated challenges. This presentation will review the current data handling approaches for operational forecasting at ECMWF, starting by an introduction to the MARS ecosystem —a family of software services, tools, and libraries which enable operational applications to efficiently access meteorological data— where an index of the entire data domain is kept, and every two-dimensional data field can be referenced with a unique and scientifically meaningful identifier.
The presentation will first focus on the FDB library, which abstracts away the HPC file system behind the MARS language and is the operational backbone for data exchange. This will include a discussion on the suitability and performance of the DAOS and Ceph object stores as alternative storage backends for the FDB.

The presentation will then give an overview of Polytope, a technology recently developed by ECMWF which enables granular access to GRIB data (written by FDB or otherwise) with potential to dramatically improve efficiency of downstream applications that require data for specific geographical regions or data points; as well as ongoing developments to support Zarr access to FDB data.

Finally, this will discuss the results of a few I/O benchmarking experiments conducted in NCAR's HPC systems during Nicolau's (EPCC PhD student and ECMWF researcher) recent visit to NCAR, enabled by the CONTINENTS project, where a number of the presented data handling components were used in combination with the MILES-CREDIT framework for machine learning model training and inference.

**Date/Time:** 28th May 2026,  1.00-2.00 PM Mountain Time

**Link:** [https://sundog.ucar.edu/public/page/CISL](https://sundog.ucar.edu/public/page/CISL)

# Past webinars

**Title:** The Ai2 Climate Emulator: Capabilities, Challenges and Opportunities

**Presenter:** Oliver Watt-Meyer, AllenAI

**Abstract:**  
Ai2 Climate Emulator (ACE) is a fast machine learning model that simulates global atmospheric variability in a changing climate over time scales ranging from hours to centuries. It generates atmospheric phenomena such as the Madden Julian Oscillation, sudden stratospheric warmings, and tropical cyclones while also accurately simulating 20th century climate trends and El Niño-related interannual variability. Its efficienc running 1500 simulated years per day on an NVIDIA H100 will make climate models more accessible and enable the generation of very large ensembles.

[Recording][recording_oliver]  
[Slides][slides_oliver]

---

**Title:** Exploring Dataflow Architectures for Improved Efficiency in Earth System Models

**Presenter:** Justs Zarins, EPCC

**Abstract:**  
Earth system models are crucial for simulating environmental processes but demand significant computational resources and energy. In this presentation we will explore the potential of dataflow architectures to enhance both computational and energy efficiency of ESMs. We will primarily discuss the Cerebras Wafer Scale Engine, examining its capabilities and evaluating its suitability for the shallow water equation.

[Recording][recording_justs]  
[Slides][slides_justs]

---

[comment]: # Links
[slides_oliver]: webinar_slides/2025-04-22_Oliver_Watt-Meyer.pdf
[recording_oliver]: https://media.ed.ac.uk/media/t/1_m2one45k
[slides_justs]: webinar_slides/2025-03-13_Justs_Zarins.pdf
[recording_justs]: https://media.ed.ac.uk/media/t/1_hh95pqmp
