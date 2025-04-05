---
title: "Instrumentation"
layout: single
sitemap: true
permalink: /instrumentation/
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.2"
  overlay_image: assets/banner_instrumentation.jpg
  actions:
    - label: "Download CV"
      url: "assets/DeCamillis_CV.pdf"
toc: true
toc_label: "Instrumentation"
toc_icon: "gear"
toc_sticky: true
---


## Optical imaging


### 3D optical coherent tomography

Mapping inclusions inside a high-refractive material such as a gemstone is not simple task. High-energy imaging struggles to detect inclusions, as they are often made of the same material of the bulk crystal. Visible and infrared imaging are more suitable candidates due to their sensitivity to matter composition and structure. However, at lower photon-energy the effects of refraction significantly increase the complexity of any optical investigation. 

As part of the SmartLight team, I developed a novel solution able to accurately locate defects present inside the sample, without the application of any refractive index matching medium. For a complete reconstruction of the volumetric information, the sample is optically scanned using the Optical Coherent Tomography (OCT) technique. Several 3D images are acquired from different directions, covering almost the full solid angle of a sphere.

My main contributions have focused on the R&D work to deliver commercially viable scanning systems for 3D crystal mapping. My projects included:
- simplifying the design and manufacturing of the fibre-optic interferometer to minimise losses and improve optical stability,
- modelling the residual optical distortion with numerical simulations in Zemax and experimental measurements,
- establishing alignment requirements and calibration protocols of the opto-mechanical components, to facilitate system installation and remote maintenance.

>![OCT interferometer](/assets/rad/oct_scanning_system.PNG)
>*First prototype of the OCT scanning system: a fibre-spliced broadband interferometer is coupled with a multi-axis gantry system allowing the full sample rotation, the displacement of the focal plane and height adjustment.*
{: style="width: 65%; font-size: 0.9rem;"}


### Dual-beam confocal microscope

At Macquarie University, I developed and optimised a purpose-built bench-top scanning microscope to study [upconversion materials as fluorescent nanoprobes](/research/#non-linear-response-of-lanthanide-nanoparticles). The key feature of this microscope was the generation and alignment of two infrared laser modes with different radial profiles: Gaussian and annular. The experiment required an accurate characterisation of the beam point-spread-functions to guarantee central symmetry and collinearity of the two lasers.

The system features the tunability of the excitation power, the selection of different spectral windows, accurate translation of the sample in the 3D space, and the capability of single-photon detection. All these features were computer-controlled by a Labview program that I developed uing a modular and scalable architecture.

Beam alignment was fundamental to enable *[Stimulated Excitation Depletion microscopy](/research/#super-resolution-imaging)*, especially when applied to up-conversion nanoparticles. As a result of my system upgrades, the resolution performance of the instrument improved to the point of being able to resolve and characterise individual nanoparticles (50 nm), well beyond the diffraction limit.  

>![Dual-beam optical setup](/assets/rad/sted_setup.jpg)
>*Table-top confocal microscope providing a 976 nm Gaussian beam as excitation source, a 808 nm annular beam as depletion laser, and detection in different spectral windows.*
{: style="width: 65%; font-size: 0.9rem;"}

Link:
- [Centre of Excellence for Nanoscale Biophotonics](https://cnbplegacy.org.au/imaging/)
- S. De Camillis et al., *Controlling the non-linear emission of upconversion nanoparticles to enhance super-resolution imaging performance*, [Nanoscale 12, 20347 (2020)](https://doi.org/10.1039/D0NR04809G)


## Ultrafast mass spectroscopy


### Pump-probe experiments

Pump-probe laser experiments are currently the best candidate for studying electron dynamics in molecules. A laser pulse initiates the dynamics from a defined electronic state and its temporal evolution is probed at a given time delay by a second laser pulse, which induces molecular fragmentation. Due to the destructive nature of the experiment and the related uncertainties, the measurement is repeated many time (10^4-10^5 mass spectra) to improve the overall sensitivity. 

The first ever measurements of molecular dynamics in biomolecules in their neutral state were made possible thanks to:
- the development of a custom mass spectrometer including a composite arrangement of electrodes with tunable voltages to optimise the signal precision and high ultra-vacuum conditions to reduce the background noise,
- the generation of neutral isolated molecules in gas phase through gentle thermal desorption, carefully balancing the need for a high number of molecules at the interaction region without inducing their thermal decomposition,
- the delivery of the pump and probe laser pulses with accurate and variable temporal delay, both focused and well aligned at the centre of the interaction region.

The observation of pure [quantum oscillations](/research/#attosecond-charge-migration) in biomolecules requires laser pulses shorter than the characteristic timescale of the electron dynamics. For these projects, I also had the possibility to work with the STARLIGHT team at the IFN-CNR facility in Milano to build and perform attosecond pump-probe experiments.

>![Pump-probe laser setup](/assets/rad/KEIRA_setup.PNG)
>*The high-sensitive mass spectrometer is integrated into the attosecond XUV-IR beamline.*
{: style="width: 65%; font-size: 0.9rem;"}

Links:
- [Ultrafast Belfast laboratories](https://www.qub.ac.uk/research-centres/light-matter-interactions/Researchthemes/Ultrafastdynamicsinatomsandmolecules/)
- [STARLIGHT project](https://atto.cfel.de/research/research_projects/starlight/)


### Ultrashort VUV pulses

Next-generation biomolecular pump-probe measurements require the adoption of ultrashort excitation pulses with a different photon energy, aiming for a more selective study of charge and energy dynamics in DNA building blocks. For instance, UV radiation is resonant with aromatic chromophores, such as nucleobases and amino acids, therefore being an ideal candidate as pump pulse due to its property of site-selective ionisation.

I joined the STARLIGHT team through the early stages of the project to build a novel laser beamline producing few-fs UV pulses.  I was involved in the preliminary work assessing and optimising the optical conditions for the generation of UV pulsed radiation, compatible with the requirements of the attosecond beamline. Considering the limitations imposed by dispersive bulk materials for the generation of ultrashort UV pulses, we adopted the novel approach of strong-field interaction with gas-phased media characterised by limited optical dispersion.

This work demonstrated the possibility to achieve few-femtosecond laser pulses with conditions of gas pressure inside the cell sustainable for the vacuum system.
This work also represented a good learning about the hardware limitations for harmonic generation in gas media and inspired a new prototype of the gas cell, fabricated in fused silica.

>![VUV beamline development](/assets/rad/vuv_setup.png) 
>*Early experiments of ultrashort UV pulse generation. The process of third-harmonic generation in noble gases was attempted with a prototype metal cell.*
{: style="width: 65%; font-size: 0.9rem;"}

Links:
- [Few-fs UV light generation](https://atto.cfel.de/research/light_sources/few_femtosecond_uv_light_sources/)



## CMOS detectors


### Intra-pixel response

Modern space missions are capable of capturing stunning images of astrophysical objects, thanks to the tech advancements in the development of array detectors with high gain and low noise. However, when studying very large objects like galaxies, any additional information becomes invaluable. For instance, the EUCLID space mission seeks to precisely measure the shape of galaxies in relation to the distribution of dark matter along the line of sight. In such cases, understanding any variations in the intra-pixel response of the detector is crucial.

The experimental INTRAPIX project, conducted at the French research center CEA-Leti, aims to characterize the sub-pixel response of array detectors by using an illumination pattern with high spatial frequencies. A series of images captured with this illumination can be analyzed to reconstruct the detector's response at a higher resolution.

As part of this project, I was responsible for developing and testing various opto-mechanical components, including the vacuum system, cryostat, and high-precision piezoelectric stage, as well as implementing modular control software to automate the system's operations.

>![Intrapix](/assets/rad/intrapix_model.PNG)
>*Schematic of the optical experimental setup INTRAPIX positioned inside the high-vacuum cryostat.*
{: style="width: 55%; font-size: 0.9rem;"}

Links:
- T. Pichon et al., *Quantix and Intrapix: test benches dedicated to quantumbefficiency measurement and intra-pixel response of detectors from VIS to LWIR*, [Proc. of SPIE 12191, 121912I (2022)](https://doi.org/10.1117/12.2630232)


{% comment %}
### Radiation effects and quantum efficiency

Array detectors used for space applications have to undergo key optical characterisation, such as the effects of particle irradiation and the measurement of quantum efficiency.

Array detectors for space applications are designed to withstand the damaging stream of charged radiation.
In particular, studying the effects of energy deposition occurring both on the active medium of the detector and the substrate.

>![Quantix](/assets/rad/quantix_model.png)
>*DESCRIPTION OF THE IMAGE*
{: style="width: 55%; font-size: 0.9rem;"}

Links:
- T. Pichon et al., *Quantix and Intrapix: test benches dedicated to quantum efficiency measurement and intra-pixel response of detectors from VIS to LWIR*, [Proc. of SPIE 12191, 121912I (2022)](https://doi.org/10.1117/12.2630232)
{% endcomment %}