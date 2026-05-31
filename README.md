# DNN-Based Surrogate Model for Real-Time S11 Prediction and Inverse Design of Triangular Slot Antenna

## Overview
A Deep Neural Network surrogate model that predicts antenna S11 performance in real-time and suggests optimal antenna dimensions for a target frequency — deployed as a live web tool!

## Live Demo
👉 https://huggingface.co/spaces/ai-antenna-design-tool/ai-antenna-design-tool

## Results
- Model Accuracy: R² = 0.94
- Best S11 achieved: -44.62 dB
- Dataset: 4,60,460 samples from 460 CST simulations

## Features
### Forward Prediction
- Input antenna parameters → Get S11 curve instantly
- Shows resonance frequency and minimum S11
- No CST simulation needed!

### Inverse Design
- Input target frequency → Get top 5 antenna designs
- Results downloadable as CSV

## Dataset
- Antenna: Triangular slot-loaded microstrip patch
- Parameters varied: Lif2, Lif1, Lf, patch size (a), frequency
- Frequency range: 2–3 GHz
- Generated via CST parameter sweep (4 days of simulation!)

## Model Architecture
- Type: Deep Neural Network (DNN)
- Optimizer: Adam | Loss: MSE
- Epochs: 50 | Batch size: 1024

## Tools Used
- Python, TensorFlow/Keras
- CST Studio Suite
- HuggingFace Spaces (deployment)

## Author
  R.J. Abinaya Sree — M.E. Communication Systems, 
  Government College of Engineering, Tirunelveli
