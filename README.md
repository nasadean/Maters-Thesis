# Self-Supervised Learning for Object Detection in Thermal Camera Data

This repository contains the final code and configuration files used in the MSc thesis, devloped on Google Colab:
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

# Results (Summary)

"1st time" Validation performance after 20 epochs:

Supervised Faster R-CNN: mAP[.5:.95] = 0.022

SSL Faster R-CNN: mAP[.5:.95] = 0.026

Final test performance:

Both models: mAP[.5:.95] = 0.002 (poor generalization, strong domain shift).

After adding more Augmentation::

Validation performance after 20 epochs:

Supervised Faster R-CNN: mAP[.5:.95] =  0.206

SSL Faster R-CNN: mAP[.5:.95] = 0.189

Final test performance:

Supervised Faster R-CNN: mAP[.5:.95] =  0.110

SSL Faster R-CNN: mAP[.5:.95] = 0.094


# Future Work

Larger and more diverse thermal datasets.

Stronger SSL methods (BYOL, MoCo v3).

Domain adaptation from visible-light to thermal.

Longer training with improved compute resources.

# License

This repository is for academic use only as part of an MSc research project.
Please cite the thesis if you use this code.

# Acknowledgements

FLIR Systems for providing the dataset.

PyTorch Detection reference implementations.

SimCLR authors for the backbone pretraining methodology.
