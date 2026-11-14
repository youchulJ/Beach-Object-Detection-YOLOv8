# Gwangalli and Dadaepo Beach Object Detection with YOLOv8

This repository contains Jupyter notebooks for detecting and tracking objects in drone videos from Gwangalli and Dadaepo beaches in Busan, South Korea. The work was part of a Korea Maritime Institute (KMI) project related to beach safety and beachgoer behavior.

## Project overview

The notebooks explore custom object detection with **YOLOv8**, tracking with **ByteTrack**, and video annotation with **Supervision**. One saved model lists three classes: **drone, marine litter, and researcher**. The available classes depend on the dataset and trained weights used in each notebook.

## Code in this repository

- **Step 1 — Training:** [Drone and researcher model](step1_training/step1_drone_training.ipynb) and [Gwangalli Beach model](step1_training/step1_gwangalli_training.ipynb) train separate YOLOv8 models and produce weights.
- **Step 2 — Video detection:** [Custom model](step2_video_detection/step2_custom_model_video.ipynb), [KMI video example](step2_video_detection/step2_kmi_video.ipynb), and [pretrained model](step2_video_detection/step2_pretrained_model_video.ipynb) apply detection to video. The custom model example also tracks objects.

The training folder also contains the original Roboflow dataset information. An empty notebook is preserved in the video detection folder.

## Getting started

The notebooks were written for **Google Colab** and use Google Drive, Roboflow, and packages installed in notebook cells. To run them, provide the required dataset, video, and model weights, and update the paths and Roboflow credentials for your environment.

The notebooks use different datasets and weights. For example, the saved output in the drone training notebook lists **drone** and **researcher**, while the custom video notebook shows a model with three classes. Check the dataset labels and model names before applying weights to a video. Some package versions are from the original experiments and may require adjustment in a current environment. The original Colab badges inside the notebooks may point to old paths; open the notebooks from the links above instead.
