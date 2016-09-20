---
layout: essay  
type: essay  
title: Statement of Purpose  
date: 2016-08-31  
labels:
  - PhD Portfolio
--- 

Sensor networks are taking on a new face in an advent of the Internet of Things. Topologies which relied on mesh networked radios are being quickly with the end-to-end TCP/IP based devices. This trend continues as the semiconductor companies are introducing ever more integrated WIFI chip-sets, which combine analog and digital radio circuitry with an embedded CPU core in a singe package. These devices are able to run for months or even years on batteries, and are quickly displacing traditional low power radio chip-sets.  Furthermore, cheap Linux single board computers are filling the gap for IOT applications which require significant DSP resources. The leap in technology that powered IOT is now making its way into traditional sensor networks and distributed measurements. 


Many projects in literature develop IP based distributed measurement networks. With resent move towards cloud computing, sensor network acquisition has evolved to scalable cloud based systems. Architecture for such systems is well described and understood.<sup>1</sup> However hardly any of them operate in environments where a single instrument signal to noise ratio is bellow 1. In such topologies, data across several sensor nodes is required to make a decision on the global event. While in traditional sensor networks would resort to techniques such as self organization and voting to localize events of interest<sup>2</sup>, IP based networks simply acquire all of the high resolution data that the measurement devices record. Indeed IP sensor nodes do not have the luxury of communication with it peers without an intermediary, due to firewalls, and security constraints. If the event rate is low, compared to the sampling rate of the sensor node, the ratio of the event data to the acquired and transmitted data will be high

For my PHD thesis I would like to explore novel methods of data reduction, via an intelligent triggering in low signal to noise IP based sensor networks. A triggering front-end will be placed in front of the traditional acquisition system as described in [1] and constantly acquire feature extracted data sent from the sensor nodes. If the feature extracted triggering stream, shows an anomaly across multiple devices, a high resolution event data can be requested from the device nodes. I intend to show that such a system will outperform traditional acquisition paradigms, by optimizing the following two metrics:

1. Minimized bandwidth factor (ratio of the event data to the acquired and transmitted data.)
2. Maximized trigger efficiency (ratio of recorded events to the total events)

There are other benefits to an intelligent triggering system fronted described above. Privacy is becoming a major issue in sensor networks, as they are commonly deployed into residential environments and workplaces. Continuous acquisition in such networks may record events which originate from local disturbances, and may in-turn leak sensitive information. My smart triggering front-end would simply discard such events, since they would only appear in a single sensor node triggering stream.

This work is inspired in part by the High Energy Phyisics data acquisition systems.[5] Such systems consist of thousands of data channels each sampling in excess of 2Gsps. A traditional approach using flash ADCs would be unfeasible, due to cost and power requirements. Instead signal is sampled in analog form and stored in a capacitive storage array of 1us depth. A separate low resolution system in turn looks for events and decides which portions of analog storage array to digitize and store. Such systems provide a huge data/cost/power reductions, while maintaining high trigger efficiency. I hope by extending these ideas to IP based sensor networks, will lead to similar results.

References: 

1. A Framework for Real Time Processing of Sensor Data in the Cloud
2. Monitoring Volcanic Eruptions with a Wireless Sensor Network
3. Smart Grid Privacy via Anonymization of Smart Metering Data
4. http://bitsandwires.hopto.org/the-noise-we-make/
5. The large analog bandwidth recorder and digitizer with ordered readout (LABRADOR) ASIC
