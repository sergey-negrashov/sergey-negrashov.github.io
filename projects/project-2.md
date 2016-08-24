---
layout: project
type: project
published: true
image: images/mtc.png
title: miniTimeCube
permalink: projects/vacay
date: 2012
labels:
    - HEP
    - FPGA
    - ASIC
summary: A "portable" neutrino detector and neutron camera for basic research and non-proliferation applications.
---

<img class="ui medium right floated rounded image" src="{{ site.baseurl }}/images/mtc.png">

The miniTimeCube (mTC) is a novel compact multipurpose detector of elementary particles, aiming to detect not only neutrinos but also fast/thermal neutrons. Potential applications include the counterproliferation of nuclear materials and the investigation of antineutrino short-baseline effects. The mTC is a plastic 0.2% 10B-doped scintillator (13 cm)^3 cube surrounded by 24 Micro-Channel Plate (MCP) photon detectors, each with an 8x8 anode totaling 1536 individual channels/pixels viewing the scintillator. It uses custom-made electronics modules which mount on top of the MCPs, making our detector compact and able to both distinguish different types of events and reject noise in real time. The detector is currently deployed and being tested at the National Institute of Standards and Technology Center for Neutron Research nuclear reactor (20 MWth) in Gaithersburg MD. A shield for further tests is being constructed, and calibration and upgrades are ongoing. The mTC's improved spatiotemporal resolution will allow for determination of incident particle directions beyond previous capabilities.

In this project I developed electronics and fpga firmware which make up most of the detector. I designed the ADC carriers, calibration system, clock distribution, triggering system, and environmental monitoring. Furthermore I lead the field team during the detector deployment at the NIST thermal column and calibration facilities, managed software development team and mentored new employees. Finally I developed the toolkit for mTC data handling and analysis.

You can learn more at the [miniTimeCube](http://www.phys.hawaii.edu/~mtc).
