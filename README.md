# Self-Supervised Learning for Object Detection in Thermal Camera Data

This repository contains the code and configuration files used in the MSc thesis:
"Self-Supervised Learning for Object Detection in Thermal Camera Data for Autonomous Driving Applications"


# Overview

This project investigates the use of self-supervised learning (SSL) for improving object detection in thermal imagery, with a focus on the FLIR ADAS dataset.
Two approaches are compared:

Supervised Faster R-CNN (ResNet50 backbone)

SSL-pretrained Faster R-CNN (SimCLR backbone)

Evaluation is performed on validation and test splits of the FLIR dataset, reporting mAP@[0.5:0.95], mAP@0.5, and size-specific AP/AR metrics.

# DataSet 
This project uses the FLIR ADAS Thermal Dataset:

Official download page: FLIR Dataset https://www.flir.com/oem/adas/adas-dataset-form/

Due to licensing restrictions, the dataset cannot be redistributed in this repository.
