---
title: "Analytics"
layout: single
sitemap: true
permalink: /analytics/
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.2"
  overlay_image: assets/banner_analytics.jpg
  actions:
    - label: "Download CV"
      url: "assets/Guccione_CV.pdf"
toc: true
toc_label: "Analytics"
toc_icon: "gear"
toc_sticky: true
---


### Automated 3D data visualisation

![ParaView](https://img.shields.io/badge/ParaView-blue?style=plastic&amp)
![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)

The project of [volumetric inclusion mapping of crystals](/instrumentation/#3d-optical-coherent-tomography) at the ANU is based on a multi-view scanning approach, which involves calculating multiple layers to enhance feature extraction. For a reliable data review, it is crucial to effectively visualize these layers across all individual 3D views.

To accomplish this, I developed a pipeline that selects different layers, applies pre-defined masks, visualizes the data using effective colormaps, and captures screenshots from the most appropriate angles. This data visualization was enabled by utilising the well-documented Python API of Paraview software.

>![SIM simulation](/assets/analytics/crystal_crack.png)
>*3D visualisation of the optical rays and amplitude, with the application of a mask to analyse the internal plane feature of the crystal.*
{: style="width: 70%; font-size: 0.9rem;"}

Among the adopted techniques:
- Data manipulation and filtering
- Multi-dimensional data visualisation
- Automated pipeline through the Python-based API


### Correcting for optical distortions

![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)
![NumPy](https://img.shields.io/badge/NumPy-aaa?logo=numpy&logoColor=013243)
![SciPy](https://img.shields.io/badge/SciPy-aaa?logo=scipy&logoColor=8CAAE6)
![Zemax](https://img.shields.io/badge/Zemax-fff?logo=ansys&logoColor=FFB71B)


Optical systems are often inherently subject to distortions, which can compromise the accuracy of the instrument. This was the case with the [3D scanning systems](/instrumentation/#3d-optical-coherent-tomography) I developed at the ANU. To mitigate these effects, the only practical solution was to model the distortion and apply a correction algorithm in data post-processing.

I created several numerical simulations of our scanning system under various conditions by using the Zemax software, and automated the execution with the Python-based API. After analyzing the simulation results, I developed an optical model that focused on two key factors: distortion along the direction of laser propagation (axial distortion) and ray tilt (telecentricity).

Finally, by applying non-linear regression to the experimental data, I validated the model’s accuracy, which was then used to correct the optical distortions.


>![Optical distortion and correction model](/assets/analytics/axial_distortion.png)
>*Graphical representation of axial distortion (left) and ray tilt distortion (right). The experimental data, available only in the first case, is depicted using color, while the numerical model is represented by black lines or arrows.*
{: style="width: 80%; font-size: 0.9rem;"}

Among the adopted techniques:
- Linear and non-linear regression
- Model validation
- Automated pipeline through the Python-based API


### Measuring ultrafast charge oscillation

![Matlab](https://img.shields.io/badge/MATLAB%C2%AE-orange?style=plastic&amp)

A rigorous statistical analysis of the data is often necessary to confirm the presence of a pattern beyond the experimental uncertainty. For example, such an analysis was essential in my PhD project to validate the first observation of [quantum charge oscillations in molecules](/research/#attosecond-charge-migration).

The typical fragmentation signal observed in this experiment features a resonant peak near zero delay, followed by an exponential decay at later times. This behavior can be accurately modeled using a convolution function that combines a Gaussian distribution with an exponential decay. The optimal fit to the experimental data was obtained through a multi-variable regression approach.

Precisely characterizing the slow fragmentation dynamics was critical for isolating the faster and weaker periodic signal. The figure below illustrates the oscillatory pattern that becomes clearly visible after subtracting the best-fit convolution curve from the raw data. To further analyze the quantum beating phenomenon, I performed a time-gated spectral analysis, which uncovered a variable oscillatory trend with a dominant frequency component at 0.23 PHz — equivalent to a period of approximately 4 femtoseconds. 

{% comment %}

Ultrafast mass spectrometry experiments produce large datasets of time-dependent molecular fragmentation patterns. The analysis requires an initial step of data preparation, involving the integration of each fragment peak from the mass spectrum after background subtraction, followed by averaging over thousands of acquisitions at each time delay.

Tipically, the fragmentation yield exhibits two components: a resonant production near zero delay and an exponential decay at later delays. This behavior can be modeled using a convolution function that combines a Gaussian and an exponential curve. The optimal fit for the experimental data was determined using a multi-variable regression approach.

In experiments involving attosecond-driven charge dynamics, a distinct oscillation in the fragmentation signal is observed at positive delays (see figure). This oscillation becomes clearer after subtracting the best-fitting convolution function. The quantum beating is not characterised by a constant period. Time-gated spectral analysis revealed that the oscillation begins with two frequency components and ultimately converges to a dominant frequency of 0.23 PHz, corresponding to a period of about 4 femtoseconds.

{% endcomment %}

>![Time-resolved charge oscillation](/assets/analytics/phe_charge_oscillation.png)
>*Quantum oscillations of the electron density are observed in the fragmentation yield, after accounting for the slower molecular dynamics using the Gaussian-exponential convolution function. At longer time delays, the charge oscillations exhibit a dominant frequency of 0.23 PHz.*
{: style="width: 70%; font-size: 0.9rem;"}

Among the adopted techniques:
- Multi-variable regression
- Time-gated spectrum analysis

### Modelling imaging performance

![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)
![NumPy](https://img.shields.io/badge/NumPy-aaa?logo=numpy&logoColor=013243)

Non-linear Structured Illumination Microscopy (NL-SIM) relies on the interference of a series of patterned light applied to a sample, enabling the extraction of information at higher spatial frequencies and thus allowing for image reconstruction with enhanced resolution.

NL-SIM is expected to be a suitable technique for upconversion nanoparticles, considering their strong non-linear emission. To evaluate its feasibility, I developed the NL-SIM reconstruction algorithm and conducted numerical experiments to simulate the optimal results achievable with our confocal microscope.

>![SIM simulation](/assets/analytics/sim_simulation.png)
>*The NL-SIM algorithm enhances image resolution by extracting information at higher spatial frequencies, analyzing a series of confocal images obtained with patterned illumination. This technique has been shown to perform effectively with upconversion nanoparticles.*
{: style="width: 70%; font-size: 0.9rem;"}

Among the adopted techniques:
- 2D Fourier transform
- Spectral domain manipulation


### Solar energy monitoring

![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)
![Pandas](https://img.shields.io/badge/Pandas-aaa?logo=pandas&logoColor=150458)

Regularly monitoring the energy usage is an effective way to save money and improve efficiency. A detailed analysis of the consumption data can help optimise the electricity usage to more cost-effective time-of-use rates and can also identify potential issues with electric appliances before they develop into more serious problems.

Below is a comparison of two different energy plans based on average annual consumption, which clearly highlights the best option. This breakdown also aids in making informed decisions about sustainability and transitioning to cleaner energy.

>![Estimation of electricity bill](/assets/analytics/electricity_bill.png)
>*Comparison of two time-of-use plans based on the average monthly energy consumption of a household over several years, categorized into different time-of-use tiers.*
{: style="width: 80%; font-size: 0.9rem;"}

Analytical methods adopted:
- Scrubbing and standardizing data
- Multivariate data representation
