# Skin lesion classification
This project is part of the course Representation Learning for Computer Vision and Medical Imaging @ Telecom Paris - Institut Polytechnique de Paris
##  Context

A skin lesion is defined as a superficial growth or patch of the skin that is visually different and/or has a different texture than its surrounding area. 
Skin lesions, such as moles or birthmarks, can degenerate and become melanoma, one of the deadliest skin cancer. Its incidence has been increasing during the last decades,  
especially in the areas mostly populated by white people.
The most effective treatment is an early detection followed by surgical excision. This is why several approaches for melanoma detection have been proposed in the last years (non-invasive computer-aided diagnosis (CAD) ).

## Data 
The project is using the ISIC 2017 dataset (https://challenge.isic-archive.com/data/#2017) already pre-processed, resized and quality checked. 
It is divided into Training (N=2000), Validation (N=150) and Test (N=600) sets.

## Goal
The goal to classify images of skin lesions as either benign (nevus or seborrheic_keratosis) or melanoma (binary classification) using machine and deep learning algorithms.

## Implementation 
In the first part, we manually compute 13 different features relevant to the skin lesion classification (feature engineering)  and then classify images using "classical" ML algorithms such as:
- Logistic Regression
- SVM 
- Random Forests.

The features belonging to different classes of the ABCD rule, namely:
- Asymmetry
- Border
- Color (and Texture)
- Dimension (and Geometry)

In the second part, we test the features learnt with Deep Learning algorithms. We first train from scratch well-known CNN architectures (VGG, ResNet, DenseNet) 
and then leverage the representations learnt by these networks on a pre-training from Imagenet (fine-tuning, full-restimation).
