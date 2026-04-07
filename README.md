# EEG-Based Emotion Recognition using SVM

Implementation of the paper "Human Emotion Recognition from EEG Brain Signals using 
Enhanced Machine Learning Methods" using the SEED-IV dataset.
Link to the original paper: https://ieeexplore.ieee.org/abstract/document/10937822
This is an assignment for the course titled DSP (EC208)

## Overview

This project implements an EEG-based emotion recognition pipeline that classifies brain 
signals into four emotional states: happiness, sadness, fear, and neutrality. The pipeline 
includes signal preprocessing, time and frequency domain feature extraction, attention-based 
feature selection (AAFST), and a multi-class SVM classifier.

## Results

| Model | F1 Score |
|-------|----------|
| Vanilla SVM | 53% |
| SVM + PCA | 59% |
| SVM + AAFST | 83% |
| SVM + AAFST + Windowed Epochs | 85% |

## Requirements
numpy
scipy
scikit-learn
matplotlib
seaborn
os
glob

## Dataset

The SEED-IV dataset is not included in this repository. It can be requested from the 
BCMI Laboratory at Shanghai Jiao Tong University at:
https://bcmi.sjtu.edu.cn/home/seed/seed-iv.html

Once downloaded, update DATA_ROOT in the notebooks to point to your local dataset path.

## Usage

Run the notebooks. Make sure the dataset is downloaded and 
DATA_ROOT is set correctly before running.

## Citation

If you use this code, please cite the original paper and dataset:

**Paper:**

G. Ghous, S. Najam and A. Jalal, "Human Emotion Recognition from EEG-brain Signals using Enhanced Machine Learning Method," 2025 6th International Conference on Advancements in Computational Sciences (ICACS), 
Lahore, Pakistan, 2025, pp. 1-7, doi: 10.1109/ICACS64902.2025.10937822.

**Dataset:**

Wei-Long Zheng, Wei Liu, Yifei Lu, Bao-Liang Lu, and Andrzej Cichocki, EmotionMeter: A Multimodal Framework for Recognizing Human Emotions. IEEE Transactions on Cybernetics, 
Volume: 49, Issue: 3, March 2019, Pages: 1110-1122, DOI: 10.1109/TCYB.2018.2797176.

## Acknowledgements

This project was developed as part of a course assignment. All credit for the original 
methodology goes to the authors of the paper and the creators of the SEED-IV dataset.
