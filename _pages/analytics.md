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



### Survey data on water safety

![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)
![NumPy](https://img.shields.io/badge/NumPy-aaa?logo=numpy&logoColor=013243)
![SciPy](https://img.shields.io/badge/SciPy-aaa?logo=scipy&logoColor=8CAAE6)
![Pandas](https://img.shields.io/badge/Pandas-aaa?logo=pandas&logoColor=150458)
![GeoPandas](https://img.shields.io/badge/GeoPandas-aaa?logo=geopandas&logoColor=139C5A)

Leveraging the power of scientific practice to meet humanitarian needs can bring unparalleled satisfaction. I had the opportunity of doing so during a project concerned with [water safety in Timor-Leste](/community/#water-safety-in-timor-leste).

Combining qualitative and quantitative data from three survey points over 18 months, I could appraise the health benefits (both direct and indirect), identify the main distribution priorities, and explore the secondary socio-economic and environmental implications from the installation of ceramic water filters in households and schools.

>![Survey data on water safety](/assets/analytics/survey.jpg)
>*A selection of indicators from the survey data: on water sterilization methods (top row), opinion on the quality of filtered water, and on the health impact of consuming filtered water over time.*
{: style="width: 90%; font-size: 0.9rem;"}

Among the adopted techniques:
- Correlation evaluation
- Principal component analysis
- Hypothesis testing


### Quantum tomography

![C](https://img.shields.io/badge/C-fff?logo=c&logoColor=A8B9CC)
![Wolfram](https://img.shields.io/badge/Wolfram-fff?logo=wolfram&logoColor=DD1100)

Quantum tomography is a powerful technique used in photonics to understand the beahviour of quantum system. Several snapshots of a quantum state are collected using a technique called *homodyne detection*. These measurements are processed to adjust for the temporal mode (i.e., the "timing") of the state, then fed to advanced statistical algorithms in sets of hundreds of thousands in order to reconstruct the density matrix of the state.

I used these algorithms in the broader context of [quantum communication](/research/#quantum-communication), specifically to estimate the fidelity of
the generated quantum states (such as single photons and multi-mode hybrid entanglement of light) to the expected outcomes.

>![Quantum tomography](/assets/analytics/tomography.jpg)
>*Quantum tomography of a single-photon state. The processed quadrature values (plot on the left, black dots) are collected via homodyne detection. For a single photon, measurements should be independent of homodyne phase. The data is binned and compared to the probability distributions of a single photon, |1⟩, and of the standard vacuum solution, |0⟩. Any contribution from the latter is a loss in fidelity; in this case, the single photon has 84% purity.*
{: style="width: 70%; font-size: 0.9rem;"}

Analytical methods adopted:
- Maximum-likelihood reconstruction
- Bootstrapping
- Positive semidefinite programming


### Mirror curvature

![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)
![NumPy](https://img.shields.io/badge/NumPy-aaa?logo=numpy&logoColor=013243)
![SciPy](https://img.shields.io/badge/SciPy-aaa?logo=scipy&logoColor=8CAAE6)

Specialized mirrors used in research environments require precise coatings to prevent optical absorption due to impurities. One type of coating, known as IBS (from ion-beam sputtering), is known to apply ultra-high surface stress on the substrate to cause the coating layer(s) to flatten, therefore preventing the creation of tiny pockets where water vapour, one of the major causes of absorption, could accumulate.

What happens, however, when the substrate is so thin that the stress from the coating can actually modify its curvature? In this project, I analysed mirror surface data obtained through vertical scanning interferometry (VSI) on ultrathin fused silica mirror substrates. Utilizing signal processing and stochastic estimation techniques, I identified directional variations in stress-induced curvature that could significantly impact the success of experiments relying on high optical power — such as [optical levitation](/research/#levitation-of-a-mg-scale-mirror).

>![Mirror curvature](/assets/analytics/curvature.jpg)
>*Curvature estimation for an ultrathin 1-inch sample with acute aspect ratio differential. From left to right: raw VSI data; surface plot obtained by kernel deconvolution; histogram of axial radii (along the x and y directions) obtained by Monte-Carlo random sampling; the final estimated curvature ellipsoid, quantifying the deformation along different axes.*
{: style="width: 90%; font-size: 0.9rem;"}

Analytical methods adopted:
- Deconvolution
- Regression fitting
- Monte-Carlo sampling


### Photon statistics

![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)
![NumPy](https://img.shields.io/badge/NumPy-aaa?logo=numpy&logoColor=013243)
![SciPy](https://img.shields.io/badge/SciPy-aaa?logo=scipy&logoColor=8CAAE6)

Single-photon sources are the backbone of optical quantum technologies. Although no ideal source exists yet, solid-state emitters are commonly seen as one of the most viable options in terms of their brightness and efficiency. Their performance is characterised using Hanbury-Brown-Twiss interferometers, a particular type of detection where the photon flux is split into two different paths and detected by single-photon counters. If the source emits pure single photons at any single time, only one detector should be triggered at that instant.

This analysis involves the calculation of second-order correlations to show that the time-tagged data from the detectors shows indeed the negative correlation predicted by quantum mechanics.

>![Photon statistics](/assets/analytics/photon_statistics.jpg)
>*Photon emissions of a perovskite quantum dot (CsPbBr3) as a function of time. The two histograms on the right quantify the reduction in photon flux density over time.*
{: style="width: 80%; font-size: 0.9rem;"}

Analytical methods adopted:
- Correlation analysis
- Time-tagging
- Density estimation


### Sensitivity enhancement

![Wolfram](https://img.shields.io/badge/Wolfram-fff?logo=wolfram&logoColor=DD1100)
![LabVIEW](https://img.shields.io/badge/LabVIEW-fff?logo=labview&logoColor=FFDB00)

One of my research projects, on [nanowire force sensors](/research/#nanowire-force-sensing), combined hands-on laboratory processes, such as real-time detection and active feedback cooling, to the world of post-processing analytics. By using the experimental data to simulate virtual feedback, and by improving further on the latter's performance with optimal filtering techniques, I demonstrated a simple approach to improve the sensitivity of these nanowire and similar systems to external signals.

>![Sensitivity enhancement](/assets/analytics/sensing.jpg)
>*Left: simultaneous feedback cooling of multiple oscillatory modes, with temperature (the area under the peaks) reducing with increasing optical power (proportional to the feedback gain). Right: sensitivity enhancement by periodic quiescence of the feedback. The schematic at the bottom indicates the procedure followed. The wave in yellow represents an external impulse signal to be detected.*
{: style="width: 90%; font-size: 0.9rem;"}

Analytical methods adopted:
- Spectral analysis
- Time-series forecasting
- Kalman filtering


### Gravitational wave signature

![Wolfram](https://img.shields.io/badge/Wolfram-fff?logo=wolfram&logoColor=DD1100)
![Python](https://img.shields.io/badge/Python-fff?logo=python&logoColor=3776AB)

This project was designed to teach valuable data analysis skills to physics students at the tertiary level. I created multi-platform educational material to explain fundamental elements of signal processing and how they can be applied to real data. Following a detailed step-by-step tutorial, the reader is introduced to concepts such as spectral filtering and noise-whitening techniques. By the end, users have the abiity to extract the signature of the historical-first observation of a gravitational wave — GW150914, by the LIGO detectors in Hanford and Livingston — from authentic observatory data.

>![Gravitational wave signature](/assets/analytics/ligo.jpg)
>*From noise to signal. The original time series (top left) is first segmented using an appropriate convolution window, then spectrally filtered and its noise re-normalised to be 'white', and finally transformed back into the time domain to show the positive detection event.*
{: style="width: 90%; font-size: 0.9rem;"}

Analytical methods adopted:
- Spectral decomposition
- Noise whitening
- Feature extraction
- Time-frequency analysis


### Road safety in the ACT

![SQL](https://img.shields.io/badge/SQL-fff?logo=postgresql&logoColor=4169E1)
![ArcGIS](https://img.shields.io/badge/ArcGIS-999?logo=arcgis&logoColor=2C7AC3)

In this project, I combined local road infrastructue network data in the Australian Capital Territory (ACT) with public domain reports on cycling accidents. By merging databases and using geometry integration strategies, I mapped out sensitive safety hazard points that could inform future governance decisions.

>![Sensitivity enhancement](/assets/analytics/crashes.jpg)
>*A heatmap of cyclist crash density (pixel radius: 10 m, search radius: 200 m) highlighting the risk of accidents in proximity of major traffic intersection nodes.*
{: style="width: 70%; font-size: 0.9rem;"}

Analytical methods adopted:
- Coordinate system projection
- Kernel density estimation
