---
layout: project
type: project
published: true
image: images/geiger.jpg
title: Cosmic Ray Telescope
permalink: projects/Geiger
date: 2016
labels:
  - PCB Mill
  - HEP
  - IOT
summary: A muon telescope based on four Soviet STS-5 geiger tubes.
---

<img class="ui medium right floated rounded image" src="{{ site.baseurl }}/images/geiger.jpg">

This is my personal project which embodies my fascination with High energy particle physics. I guess I am always drawn to the fundamentals, and there is nothing more fundamental then Nature. I spent a few years working on a neutrino physics experiments, but most of my effort was spent on FPGA and PCB work. I always wanted to make a particle physics measurement outside of work, and now thanks to a handful of cold war relics, I can. Geiger tube are among the oldest radiation detectors out there, and are still in use today. Old Soviet tubes in particular are easily acquired from your favorite online flea market. After a few decades of laying in a dusty civil defense warehouse, these devices are now trickling down to makers around the world.

For this project I designed and built a cosmic ray telescope which operates based on a coincidence principle. Terrestrial radiation in most places around the world, is mainly low energy "stuff". Barely enough to trigger a Geiger tube. Cosmic ray muons however, have more then enough energy to trigger multiple Geiger tubes. By looking at the coincidental signals across an array of geiger tubes I was able to create a device which essentially filters out terrestrial radiation, while providing some angular measurement for the cosmic rays it detects. 

This device is built almost entirely out of discrete components, and all of the PCBs were milled on my CNC mill. The only components which contain integrated circuits are the wallwart PSU and an ESP8266 wifi enabled MCU. ESP8266 allowed me to debug operate the device without having to attach it to a computer. Next iteration will have 8 tubes on a CNC pivotable enclosure for better angular resolution.

You can read about the development on my <a href="http://bitsandwires.hopto.org/tag/geiger/">blog</a>.
