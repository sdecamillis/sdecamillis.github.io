---
title: "Instrumentation"
layout: single
sitemap: true
permalink: /instrumentation/
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.2"
  overlay_image: assets/banner_research.jpg
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
- establishing alignment requirements and calibration protocols of the opto-mechanical components, to facilitate system installation and remote maintenance,
- modelling the residual optical distortion with numerical simulations in Zemax and experimental measurements.

>![OCT interferometer](/assets/rad/oct_scanning_system.png)
>*First prototype of the OCT scanning system: a fibre-spliced broadband interferometer is coupled with a multi-axis gantry system allowing the full sample rotation, the displacement of the focal plane and height adjustment.*
{: style="width: 65%; font-size: 0.9rem;"}

References:

- ...


### Dual-beam confocal microscope

The study of UCNPs had a specific list of requirements to address the following needs:
- excitation in the NIR
- detection in different spectral windows in the visible and in the excitation band
- single-photon detection
- tunable excitation power
- 3D scanning system

developed acquisition system in Labview.

To enable STED, a second excitation beam was introduced in the excitation optical path to allow for single or dual excitation channel.

In this research project, I developed a table-top confocal microscope suitable for imaging a selected type of UCNPs..


>![Dual-beam optical setup](/assets/rad/sted_setup.jpg)
>*Table-top confocal microscope providing a 976 nm Gaussian beam as excitation source, a 808 nm annular beam as depletion laser, and detection in a tunable spectral window.*
{: style="width: 65%; font-size: 0.9rem;"}

References:
- S. De Camillis et al., *Controlling the non-linear emission of upconversion nanoparticles to enhance super-resolution imaging performance*, [Nanoscale 12, 20347 (2020)](https://doi.org/10.1039/D0NR04809G)



## Ultrafast mass spectroscopy


### Pump-probe experiments

Pump-probe laser experiments are a reliable technique to study electron dynamics in molecules. 
Laser pulses can initiate dynamics from a given initial electronic state but we don't have the capability to record in real-time the change evolution, even less on a single molecule level.
The idea is to take snapshots of the change state by inducing photo-fragmentation with a second laser pulse. The fragmentation pattern is found to be directly related to the electron distribution of the molecule prior to the dissociative event.
As the initial electron state is always the same, the accuracy of the measurement relies on building a sufficiently large statistical sample of the fragmentation pattern (10^5 molecules * 10^4 spectra).

Three elements:
- neutral isolated molecules available in gas phase, through gentle thermal desorption, in proximity of the interaction region
- a mass spectrometer to collect and measure the products of the fragmentation events, requiring high-voltage electrodes in high ultra-vacuum
- pump and probe laser pulses with controlled and tunable temporal delay, focused at the centre of the interaction region of the mass spectrometer.


{% comment %} 
The dynamics can be initiated by an ultrashort laser pulse, and it can be subsequently probed by the interaction with a second laser pulse leading to the photo-dissociation

Pump-probe pulses to obtain time-dependent fragmentation of ionised molecules.
{% endcomment %} 

>![Pump-probe laser setup](/assets/rad/KEIRA_setup.png)
>*DESCRIPTION OF THE IMAGE*
{: style="width: 65%; font-size: 0.9rem;"}

Links:
- [Ultrafast Belfast laboratories](https://www.qub.ac.uk/research-centres/light-matter-interactions/Researchthemes/Ultrafastdynamicsinatomsandmolecules/)


### Ultrashort VUV pulses

Description of the project for generating VUV laser pulses

>![VUV beamline development](/assets/rad/VUV_setup.png)
>*DESCRIPTION OF THE IMAGE*
{: style="width: 65%; font-size: 0.9rem;"}

Links:
- [ELYCHE laboratories](https://www.attosecond.fisi.polimi.it/)


## CMOS detectors


### Intra-pixel response

Paragraph on Intrapix experiment

>![Intrapix](/assets/rad/intrapix_model.png)
>*DESCRIPTION OF THE IMAGE*
{: style="width: 55%; font-size: 0.9rem;"}

Links:
- T. Pichon et al., *Quantix and Intrapix: test benches dedicated to quantumbefficiency measurement and intra-pixel response of detectors from VIS to LWIR*, [Proc. of SPIE 12191, 121912I (2022)](https://doi.org/10.1117/12.2630232)


### Effects of ion radiation

Paragraph on Quantix experiment

>![Quantix](/assets/rad/quantix_model.png)
>*DESCRIPTION OF THE IMAGE*
{: style="width: 55%; font-size: 0.9rem;"}

Links:
- T. Pichon et al., *Quantix and Intrapix: test benches dedicated to quantumbefficiency measurement and intra-pixel response of detectors from VIS to LWIR*, [Proc. of SPIE 12191, 121912I (2022)](https://doi.org/10.1117/12.2630232)