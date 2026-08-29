# Video Caption Generation using Spatio-Temporal Attention

## Overview

This project generates natural language captions for videos from the MSVD (Microsoft Video Description) dataset. The model combines visual appearance information and motion dynamics to produce descriptive captions for short video clips.

## Dataset

- **MSVD Dataset**

## Feature Extraction

### Global Appearance Features

- Extracted using **InceptionV3**
- Captures scene-level visual information from video frames

### Motion Features

- Extracted using **C3D (3D Convolutional Neural Network)**
- Captures temporal motion patterns and actions occurring in videos

## Model Architecture

- **GRU Encoder** processes visual and motion features
- **Attention Mechanism** learns to focus on the most relevant video information during caption generation
- **GRU Decoder** generates captions word-by-word based on encoder outputs and attention context

## Workflow

1. Extract global visual features using InceptionV3.
2. Extract motion features using C3D.
3. Encode video representations using a GRU-based encoder.
4. Apply attention to identify important visual and temporal cues.
5. Generate captions through a GRU decoder.

##

## Results

The model successfully learns visual and motion representations from videos and generates descriptive captions for unseen video clips from the MSVD dataset.
