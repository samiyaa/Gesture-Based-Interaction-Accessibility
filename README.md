# Gesture-Based-Interaction-Accessibility

code adapted from: 
https://github.com/kinivi/hand-gesture-recognition-mediapipe/blob/main/keypoint_classification_EN.ipynb
https://www.tensorflow.org/api_docs/python/tf/keras/Model
https://www.youtube.com/watch?v=a99p_fAr6e4&t=899s 
https://milvus.io/ai-quick-reference/what-are-negative-sampling-and-its-role-in-embedding-training
https://mediapipe.readthedocs.io/en/latest/solutions/hands.html

these models were obtained from Google's mediapipe website and are used for hand classification (hand landmarker) and gesture recognition (gesture recognize):
hand_landmarker.task (https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker) 
gesture_recognizer.task (https://ai.google.dev/edge/mediapipe/solutions/vision/gesture_recognizer) 

training phase is just for the brief practice phase before the actual study. 

model folder has the models made for back and zoom gestures.

annotations has the test, train, and val landmarks for the hands obtained from the HaGRIDv2 dataset, and downloaded from their GitHub: https://github.com/hukenovs/hagrid

all folders (except reference_images) need to be downloaded for the main code (Gesture_Prototype.ipynb) to run 

reference_images just has the hand landmarks from MediaPipe and different gesture classes from HaGRIDv2 which were used in the ideation phase of this project. 
