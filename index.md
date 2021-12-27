## Project Overview

The EdgeFlooding project is funded by the [NGIatlantic](https://ngiatlantic.eu/) initiative under the [3rd open call for experiments](https://ngiatlantic.eu/ngiatlanticeu-3rd-open-call). The project is a bilateral project between the [Department of Information Engineering at the University of Pisa](https://www.dii.unipi.it) and the [Department of Information Systems at the University of Maryland Baltimore County](https://informationsystems.umbc.edu/). 

The project aims at assessing whether a distributed computing architecture based on the edge/cloud computing paradigm can be adopted for the implementation of a flash flood monitoring system. Existing flood monitoring systems adopt a centralized cloud-based approach where monitoring stations are deployed in flood-prone areas and transmit their data (sensor data and images) to a cloud-based service for analysis. Edge/fog computing extends the centralized cloud computing architecture by introducing an intermediate computing layer in proximity of the physical systems. The goal of EdgeFlooding is to develop a prototype of a flood monitoring system based on the edge/cloud computing paradigm and measure its performance via a set of experiments. The aim is to highlight the advantages and the drawbacks of adopting such distributed approach to perform data analysis at the edge, in proximity of the monitoring sites. The project will leverage an existing implementation of [a cloud-based flood monitoring system developed at UMBC](https://mpsc.umbc.edu/projects/flash-flood-monitoring). The system exploits the fusion of multiple data sources (e.g. environmental sensor data, social media data and smart camera images) to detect any potential flood events and assess their impact. A testbed prototype of the flooding monitoring system has been already developed and deployed in the Baltimore County area. 

EdgeFlooding will be extended the current implementation to obtain a novel implementation of the system that adopts an edge/cloud approach, where a part of data analysis, namely the image analysis, is moved at the edge, in proximity of the monitoring sites. A modular architecture based on microservices will be adopted in order to ensure the possibility to restructure the architecture of the platform, thus allowing their deployment on different computing nodes. 

Different experiments will be carried out:
1. one *cloud configuration* where all the services are deployed on the cloud as in the original implementation;

![image1](https://user-images.githubusercontent.com/8784059/147485873-532476de-b9be-453e-9d00-bbbd8aa7c5fb.png)

2. one *edge configuration* where the image analysis services are deployed on edge nodes while the social media and data aggregation services are hosted on the cloud. 

![image2](https://user-images.githubusercontent.com/8784059/147485911-9d7821be-ac7d-4f1e-813d-881bd1e0e612.png)

An extensive experimentation will be run to evaluate the performance of the system with the two configurations (cloud vs edge) and assess the feasibility of adopting the edge/cloud approach in real deployments and measure its advantages/drawbacks. 
The experimentation will be organized into the following two phases. A first phase in which a realistic deployment is emulated using the nodes of the [Grid’5000 testbed](https://www.grid5000.fr/w/Grid5000:Home), a large-scale testbed for experiment-driven research in the area of parallel, distributed computing and cloud managed by a scientific interest group (GIS) and hosted by Inria .Nodes from different locations of the testbed and with different computing capabilities will be exploited to emulate cloud computing nodes (top-range servers with powerful CPUs and GPUs) and edge computing nodes (mid-range servers with less powerful CPUs and mid-level GPUs). A second experimentation phase in which the edge computing layer is emulated with nodes external to the Grid’5000 testbed to assess the performance of the system when the edge layer is implemented with constrained devices, e.g. a PC or an embedded system, installed in proximity of - or co-located with - the cameras. To this aim the PCs available at the [Virtual Wall](https://www.ugent.be/ea/idlab/en/research/research-infrastructure/virtual-wall.htm) testbed, hosted at and managed by imec IDLabt ilab.t in Ghent, will be exploited in addition to the embedded systems available on the Fog testbed available at the [Cloud Compuiting, Big Data and Cybersecurity crosslab](https://crosslab.dii.unipi.it/cloud-computing-big-data-cybersecurity-lab) at the Department of Information Engineering of the University of Pisa. 

The analysis of the results of the experiments will aim at the following: (i) assess the feasibility of adopting the edge/cloud implementation in real systems and, in particular, verify the feasibility of implementing the image analysis algorithms on edge nodes; (ii) measure metrics such as analysed FPS, latency, bandwidth and CPU/RAM occupation to compare the two edge/cloud and cloud configurations and highlight advantages/disadvantages of both. Such results and conclusions are expected to be of interest not only for future flood monitoring systems but in general in the area of environmental monitoring.

## Distributed Edge flooding platform
The distributed edge flooding platform is currently under development. The platform will be made available as opensource project at the following repository: [EdgeFloodingPlatform](https://github.com/EdgeFlooding/EdgeFloodingPlatform) 

## Results analysis
A public summary of the results obtained by the project will be published on this website at the end of the project.

## Our team
The project is a bilateral project between UNIPI and UMBC. The following personnel is involved:
* [Carlo Vallati](http://www.iet.unipi.it/c.vallati/), University of Pisa, PI
* [Francesca Righetti](http://for.unipi.it/francesca_righetti/), University of Pisa
* [Giuseppe Anastasi](http://www.iet.unipi.it/g.anastasi/), University of Pisa
* [Nicola Tonellotto](https://tonellotto.github.io/), University of Pisa
* [Andrea Klaus Tubak](), University of Pisa
* [Nirmalya Roy](), University of Baltimore County
* [Aryya Gan-gopadhyay](https://sites.google.com/site/homearyya/), University of Baltimore County
* [Bipen Basnyat](), University of Baltimore County

![immagine](https://user-images.githubusercontent.com/8784059/147487303-a7a87a17-48e2-4c5d-964a-d147089b15cf.png)     ![immagine](https://user-images.githubusercontent.com/8784059/147487345-dce82632-a1e4-4486-b662-1f5ffba9e3dd.png)


