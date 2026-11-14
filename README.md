# Gwangalli and Dadaepo Beach Object Detection with YOLOv8

This repository contains Jupyter notebooks for detecting and tracking objects in drone videos from Gwangalli and Dadaepo beaches in Busan, South Korea. The work was part of a Korea Maritime Institute (KMI) project related to beach safety and beachgoer behavior.

## Project overview

The notebooks explore custom object detection with **YOLOv8**, tracking with **ByteTrack**, and video annotation with **Supervision**. One saved model lists three classes: **drone, marine litter, and researcher**. The available classes depend on the dataset and trained weights used in each notebook.

## Code in this repository

- [Training a custom model](training/step1__new_model_yolo_weight.ipynb): Downloads a Roboflow dataset and trains, validates, and tests a YOLOv8 model.
- [Applying a custom model to video](video/step2_new_model_custom_dataset_application_23_09_12.ipynb): Detects and tracks objects frame by frame, then saves an annotated video.
- [Gwangalli Beach training experiment](<training/Project_sponsored by KMI_(Weight_part1_24.04.09).ipynb>): Trains a separate YOLOv8 model using a Gwangalli Beach dataset.
- [Additional video example](<video/KMI_project_part2(data_processing_part).ipynb>) and [pretrained model example](video/__yolov8_custom_YC_11_09_23.ipynb): Apply detection to video with different models and settings.
- [Reference files](reference/): Includes the original Roboflow dataset information and an empty notebook.

## Getting started

The notebooks were written for **Google Colab** and use Google Drive, Roboflow, and packages installed in notebook cells. To run them, provide the required dataset, video, and model weights, and update the paths and Roboflow credentials for your environment.

The notebooks use different datasets and weights. For example, the saved output in the training notebook lists **drone** and **researcher**, while the video notebook shows a model with three classes. Check the dataset labels and model names before applying weights to a video. Some package versions are from the original experiments and may require adjustment in a current environment.
