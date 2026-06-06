# MedTrack-TX System Design

## Input

* Dermoscopic Image (Visit 1)
* Dermoscopic Image (Visit 2)
* Dermoscopic Image (Visit 3)

## Module 1: Segmentation

Model: SegFormer

Input:

* Skin lesion image

Output:

* Lesion mask

## Module 2: Feature Extraction

Model: Vision Transformer (ViT)

Input:

* Segmented lesion

Output:

* Feature vector

## Module 3: Temporal Analysis

Model: Temporal Transformer

Input:

* Visit 1 features
* Visit 2 features
* Visit 3 features

Output:

* Growth trend
* Shape change
* Color change
* Border evolution

## Module 4: Risk Prediction

Output:

* Low Risk
* Medium Risk
* High Risk

## Module 5: Clinical Report

Output:

* PDF Report
* Lesion comparison visualization
* Risk assessment summary
* Growth statistics
