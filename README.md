# **All-Optical-Brain-Computer-Interface BrainHack Vanderbilt 2025**

## **Leaders**
Graduate Student: Hailey Edelman 

Undergraduate Student: Maxwell Sharp

Principal Investigator: Daniel Gonzales, PhD

## **Project Description**
This project aims to use an all-optical BCI to study synaptic plasticity during sensorimotor learning in mice, providing insights into learning deficits in disease models. Using real-time imaging data from individual cortical neurons, animals will learn to modulate neural activity patterns and move a virtual cursor toward a target. In addition to the functional readout, the imaging also allows us to scan synaptic connections and observe how they change over the course of BCI training. This project will provide unprecedented insights into how subcellular synaptic processes drive skill acquisition. Once validated in healthy animals, this approach can be applied to disease models such as autism spectrum disorder (ASD) to uncover the aberrant synaptic mechanisms underlying learning deficits. This innovative combination of imaging, closed-loop neural control, and real-time adaptability makes the project uniquely positioned to inform therapeutic strategies and improve understanding of learning disorders.  

<img width="434" alt="Screenshot 2025-01-10 at 3 24 16 PM" src="https://github.com/user-attachments/assets/a49a6c3d-0505-4c46-b451-4bc297e9a1ad" />

## **Primary Objective**
Develop a rapid, real-time neural decoding algorithm to control a 2D cursor based on calcium transient dynamics recorded using two-photon imaging in healthy animals, with plans to extend this approach to ASD models. 

## **Onboarding Documentation**
### Getting Started
1. **Join our Discord channel**: Stay updated and collaborate with the team. Discord Channel Name: @2p_bci
2. **Download MATLAB**: [MATLAB Download](https://www.mathworks.com/downloads/) (Free with VU email address).
3. **Access The Google Drive Folder**: [Google Drive Folder](https://drive.google.com/drive/folders/1rSHFr5iAfE-CrYZfGHz9_dFOTBRGZBaF?usp=share_link)

**Note on Project Data**
For the purposes of Brainhack 2025 Conference timeline and duration, a sample data set will be utilized. This data set contains two-photon data from a study involving a mouse running on a wheel. There are two pistons near the face. When one piston shoots out, every time the animals whisks,the C1 whisker touches the piston. When the second piston is extended,the D1 whisker touches the piston during whisking. Only one piston is extended at a time. 

The platform developed using this sample data set will be modified to be used with the ASD project described above once data is collected. 

### **Useful Resources**
Check out these published papers!

[FluoAnalysis: An Open-Source MATLAB Toolbox for Analysis of Calcium Imaging Measurements of Oscillatory Astrocytic and Neuronal Networks](https://pmc.ncbi.nlm.nih.gov/articles/PMC11353153/)


[Pipeline for 2-photon all-optical physiology in mouse: From viral titration and optical window implantation to binarization of calcium transients](https://www.sciencedirect.com/science/article/pii/S2666166721007164)


[SmaRT2P: a software for generating and processing smart line recording trajectories for population two-photon calcium imaging](https://braininformatics.springeropen.com/articles/10.1186/s40708-022-00166-4)

## **Prerequisites**
Ensure you have the following:
- MATLAB 
- Python

## **Steps for Each Analysis**

### 1. Preprocessing
- Load Data
- Filtering
- Signal Normalization

### 2. Registration
- Tessellation: split image into non-overlapping polygon subregions to enable cluster analysis
- Motion Correction

### 3. Segmentation
- Feature Mapping: identify representative image patch features (e.g. mean intensity, local variance)
- Signal Localization: divide patches into groups based on signal state

### 4. Analysis
- Neural Network Design: design preliminary neural network (inputs / layers / # of neurons / outputs) using TensorFlow (Python Library)
- Model Training: split 2P subset into train/test sets and use to train/evaluate the model’s performance
- Spike Inference: use neural network outputs to dynamically update virtual cursor

## **Instructions to Begin Hacking**
- Access the [Google Drive Folder](https://drive.google.com/drive/folders/1rSHFr5iAfE-CrYZfGHz9_dFOTBRGZBaF?usp=share_link) and download 2P_split.mat and load_2P.m files in MATLAB. 














