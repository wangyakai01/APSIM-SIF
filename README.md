# APSIM-SIF

<<<<<<< HEAD
（*Agricultural Production Systems Simulator - sun-induced chlorophyll fluorescence*）

## About APSIM-SIF
Sun-induced chlorophyll fluorescence (SIF) can be thought of as the byproduct of the absorbed photosynthetically active radiation times the plant’s fluorescence yield efficiency. Here, we have incorporated equations coupling SIF to photosynthesis in a crop model, the Agricultural Production Systems sIMulator (APSIM).
=======
（*Agricultural Production Systems Simulator - Sun-Induced chlorophyll Fluorescence*）

## About APSIM-SIF
Solar-induced chlorophyll fluorescence (SIF) can be thought of as the byproduct of the absorbed photosynthetically active radiation times the plant’s fluorescence yield efficiency. Here, we have incorporated equations coupling SIF to photosynthesis in a crop model, the Agricultural Production Systems sIMulator (APSIM).
>>>>>>> ddfd67ff0a84689972021eaf9bafaf0325534d5b


## Getting Started

#### *Minimum System Requirements*
1 GHz CPU 
512MB RAM

#### *Recommended System Requirements*
Quad Core 3GHz + CPU
4GB RAM


## Software Requirements

This software runs on the Windows operating system.

#### *Minimum Operating System*
Windows XP

#### *Recommended Operating System*
Windows 10

### Prerequisites

 The APSIM-SIF modules toolbox works in conjunction with the The Agricultural Production Systems Simulator (APSIM : [www.apsim.info](http:www.apsim.info)), in particular APSIM version 7.8. Register and download the APSIM (v7.8) installation software from the [https://www.apsim.info/download-apsim/](https://www.apsim.info/download-apsim/)website. And the toolbox  includes three modules, namely Photosynthesis, FLUSPECT and SIF, which can be downloaded from [here](https://github.com/wangyakai01/APSIM-SIF). The Photosynthesis module is derived from DCaPST (Diurnal Canopy Photosynthesis-Stomatal Conductance Simulator) ( see [DCaPST](https://github.com/QAAFI/DCaPST) for details). 



### Installing and demo

1. Install APSIM 7.8 software (Apsim7.8Setup.exe).

2. Install DCaPST software (DCaPSTInstall.msi) and make sure the installation path is the same with APSIM.

3. Open ApsimUI and start a new simulation using APSIM example 'Continuous Wheat.apsim'.
![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image1.png)

4.  Add APSIM-SIF toolbox (APSIM-SIF modules.xml) to  the Apsim User Interface.  First, click the Options button on the toolbar. Then, click “Add a toolbox” and browse to the location of the APSIM-SIF modules.xml file for the Toolbox and select OK. Finally,  you will see the new toolbox in the toolbox bar at the bottom of the APSIM window.
![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image2.png)
5.  Drag modules to paddock from the toolbox. Be sure to follow the order: Photosynthesis, FLUSPECT, SIF.
![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image3.png)
6.  In the modules script, the [Output] tag denotes a variable that APSIM can supply to output file when requested, you can set what variables you want reported in the 'outputfile' node.
![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image4.png)
![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image5.png)
7. Runing the simulation and create a graph to see the result.

![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image6.png)



## Running the tests

1. Once the "UIUC-SIF sim.apsim" simulation has be opened within the APSIM (v7.8) user interface then clicking the 'Run' button.

![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image7.png)

2. When the run is complete, click the ‘outputfile’ component to view the results and create a graph to see the simulated SIF with observed SIF.
The relationship between simulation and observation SIF values are reasonable when compared with satellite (TROPOspheric Monitoring Instrument, TROPOMI) and in situ tower measurements at the Energy Farm of the University of Illinois at Urbana-Champaign, USA (40.07°N, 88.21°W). Blue line represents the APSIM-SIF simulated SIF,  red dots represent ground-based measured SIF and green dots represent TROPOMI observed SIF. 

![image](https://github.com/wangyakai01/APSIM-SIF/blob/master/image/Image8.png)





## Acknowledgments

We are grateful to Kaiyu Guan for providing data on the ground-based observed SIF data at a 
soybean field in the University of Illinois at Urbana-Champaign, USA.
 The authors also acknowledged the DCaPST code support from Alex Wu in the University of Queensland, Brisbane, Queensland, Australia.
Acknowledgment is made to the APSIM Initiative which takes responsibility for quality assurance and a structured innovation programme for APSIM's modelling software, which is provided free for research and development use (see [www.apsim.info](www.apsim.info) for details).

