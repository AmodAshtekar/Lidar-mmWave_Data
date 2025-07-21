# LiDAR-mmWave Indoor NLoS Dataset

This repository contains synchronized LiDAR and mmWave measurement data collected for the research project titled:  
**“LiDAR Backscatter-Driven mmWave Beam Alignment in Indoor NLoS Environments”**  
conducted at California State University, Sacramento.

## Overview

The dataset includes co-located LiDAR and mmWave data captured from 55 receiver grid points in a static, controlled indoor lab environment. The goal is to investigate whether LiDAR backscatter intensity can predict optimal mmWave beam directions in non-line-of-sight (NLoS) conditions.

## Data Collection Details

- **Location**: Electronics Laboratory, California State University, Sacramento  
- **Setup**: Static co-located configuration — mmWave receiver and LiDAR sensor mounted on the same tripod  
- **Collection Date**: Approximately two months before this repository's creation  
- **Height**: Transmitter and receiver both positioned at **1.6 meters**  
- **Receiver Grid Points**: 55 (transmitter fixed at a single location)  
- **Environment**: Non-Line-of-Sight (NLoS) with natural indoor reflectors (walls, furniture, lab equipment)

## Equipment

- **mmWave Transceiver**  
  - Model: *Sivers EVK02001* (60 GHz)  
  - Beam steering: ±45° azimuth, 5° resolution  
  - Receiver beamformed from −90° to +90° (in 10° steps)  
  - Signal captured using USRP and power spectral density analysis  
  - 📄 [Sivers EVK06002 Product Brief](https://www.sivers-semiconductors.com/wp-content/uploads/2021/10/Product-Brief-EVK06002-202110.pdf)

- **LiDAR Sensor**  
  - Model: *Quanergy M8*  
  - 360° horizontal field of view  
  - Captures both range and intensity data  
  - Data exported using QView and processed via CloudCompare  
  - 📄 [Quanergy M8 Product Page](https://www.quanergy.com/lidar/m8/)

## Repository Structure

- `/mmwave_data/`: Received Signal Strength (RSS) data across AoA/AoD directions  
- `/lidar_data/`: Angularly-binned LiDAR intensity values  

## License

This dataset is released for academic and non-commercial research use only.
