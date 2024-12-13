This repository contains a project aimed at detecting hazardous material (Hazmat) placards on containers using YOLOv8 (You Only Look Once) object detection technology. The system is designed to train a custom YOLOv8 model on a dataset of Hazmat placards, validate the trained model, and predict placards on test images.

Features
Custom Dataset Training: Trains a YOLOv8 model on a specialized dataset for Hazmat placard detection.
Model Evaluation: Validates the trained model and visualizes the validation results using confusion matrix and annotated images.
Real-Time Detection: Uses the trained model to detect Hazmat placards in test images with a confidence threshold.
Visualization: Displays intermediate results such as confusion matrix images to analyze performance.
Workflow
Mount Google Drive: Integrates Google Drive for easy access to the dataset and storage of results.
Install Dependencies: Installs YOLOv8 and supporting libraries for image processing.
Training:
Trains the YOLOv8 model (yolov8n.pt) for 25 epochs with an input size of 640x640 pixels.
Saves the best-performing weights for future inference.
Generates training progress plots.
Validation:
Evaluates the model on validation data.
Displays images with annotated labels and bounding boxes.
Prediction:
Applies the trained model to a test dataset.
Detects Hazmat placards and saves the results with bounding box annotations.
Requirements
Python 3.7+
Libraries: ultralytics, Pillow
