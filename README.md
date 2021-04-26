# anomaly-detection
This repository contains the LHC Olympics 2020 anomaly detection datasets and some relevant scripts.

> LHC Olympics 2020 webpage: https://lhco2020.github.io/homepage/
> LHC Olympics 2020 R&D dataset: https://zenodo.org/record/4536377#.YHTfCBNKhTZ

## Description of the dataset:
This is the first R&D dataset for the LHC Olympics 2020 Anomaly Detection Challenge. It consists of 1M QCD dijet events and 100k W'->XY events, with X->qq and Y->qq. The W', X, and Y masses are 3.5 TeV, 500 GeV and 100 GeV respectively. The events are produced using Pythia8 and Delphes 3.4.1, with no pileup or MPI included. They are selected using a single fat-jet (R=1) trigger with pT threshold of 1.2 TeV. 

* Background + signal dataset: `events_anomalydetection_v2.features.h5`   
Background and signal (2-prong) are mixed with 10:1 ratio. 
* QCD background (without signal, 1M events): `events_anomalydetection_DelphesPythia8_v2_qcd_features.h5`
* 2-prong signal file (100k events): `events_anomalydetection_DelphesPythia8_v2_Wprime_features.h5`
* 3-prong signal file (100k eevents): `events_anomalydetection_Z_XY_qqq.features.h5`

## Data visualization
* [Explore dataset: background and 2-prong signal](https://github.com/uwepe-analysis/anomaly-detection/blob/main/notebooks/explore_dataset.ipynb) compares the 2-prong signal events with the background events
* [Explore dataset: background, 2-prong and 3-prong signal](https://github.com/uwepe-analysis/anomaly-detection/blob/main/notebooks/explore_3prong_dataset.ipynb) compares the 2-prong and 3-prong signal events with the background events
