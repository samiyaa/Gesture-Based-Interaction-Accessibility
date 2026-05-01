# Gesture-Based-Interaction-Accessibility

## Overview
This project explores touchless interaction using mid-air hand gestures, focusing on the trade-off between user-defined and system-defined gestures. A real-time prototype was developed using MediaPipe and TensorFlow Lite.

## Features
Webcam-based hand tracking
Pre-trained static gesture recognition
Custom classifiers for Back and Zoom
Lightweight, real-time system (CPU-friendly)

## Structure
```
Gesture_Prototype.ipynb  # Main system
model/                   # Trained classifiers
annotations/             # (Not included – see below)
data/                    # (Not included – see below)
reference_images/        # Gesture examples
```
### dataset
Uses HaGRIDv2: https://github.com/hukenovs/hagrid

Download these gesture classes:
- Back: three_gun
- Zoom: thumb_index
- Negatives: peace, dislike, like, palm, point

Place them in `/annotations/` (train/val/test splits).

## SETUP
**Install dependencies:**
pip install mediapipe tensorflow opencv-python numpy

**Download MediaPipe models:**
Hand Landmarker
Gesture Recognizer
Run:
Gesture_Prototype.ipynb

## NOTES:
annotations/ not included due to size
Models for Back and Zoom are pre-trained
Practice phase in notebook is for user familiarisation only
CSV files for Back and Zoom will be automatically generated in the data/ folder when running the training scripts (not included due to size)


## References: 
1. https://github.com/kinivi/hand-gesture-recognition-mediapipe/blob/main/keypoint_classification_EN.ipynb
2. https://www.tensorflow.org/api_docs/python/tf/keras/Model
3. https://www.youtube.com/watch?v=a99p_fAr6e4&t=899s
4. https://milvus.io/ai-quick-reference/what-are-negative-sampling-and-its-role-in-embedding-training
5. https://mediapipe.readthedocs.io/en/latest/solutions/hands.html
6. hand_landmarker.task: https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker)
7. gesture_recognizer.task: https://ai.google.dev/edge/mediapipe/solutions/vision/gesture_recognizer) 
