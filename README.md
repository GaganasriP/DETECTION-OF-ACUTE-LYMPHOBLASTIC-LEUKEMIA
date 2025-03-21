# DETECTION-OF-ACUTE-LYMPHOBLASTIC-LUEKEMIA

Project Overview

This project focuses on identifying immature lymphoblast cells from normal lymphoblast cells using deep learning techniques. Specifically, it employs the Inception V3 pretrained deep convolutional neural network for object classification.

Dataset

The dataset used for this project is sourced from the ALL Challenge dataset of ISBI 2019 available on The Cancer Imaging Archive:

Citation: Gupta, A., & Gupta, R. (2019). ALL Challenge dataset of ISBI 2019 [Data set]. The Cancer Imaging Archive. DOI:10.7937/tcia.2019.dc64i46r

Methodology

1. Data Preprocessing

The dataset is split into training and validation sets with appropriate labeling.

2. Feature Extraction

The Inception V3 model (pretrained on ImageNet weights) is used for feature extraction.

3. Classification

The extracted features are passed through a Fully Connected Network (FCN) with a dropout rate of 0.3.

Classification is performed using an SVM classifier.

Comparative analysis is done with VGGNet Network architecture and SVM classifier.

4. Training and Optimization

Early stopping is implemented to halt training when there is no improvement in validation accuracy.

Various image classification models were tested to evaluate performance.

Analysis & Results

Validation Accuracy: 60-65.399%

Test Accuracy: ~78%

The model successfully differentiates between immature and normal blood cells.

The study highlights the need for better classification techniques for ALL subtypes, which are often ignored due to high interclass similarity and intraclass variability.

Conclusion

The model effectively detects immature blood cells, aiding in early leukemia diagnosis.

Further improvements can be made in subtype classification, which is crucial for precise medical treatment.

References

Deep Transfer Learning in Diagnosing Leukemia in Blood Cells - Mohamed Loey, Mukdad Naman, and Hala Zayed (Benha University, Egypt)

Medical Image Computing and Computer-Assisted Intervention (MICCAI 2017) - Descoteaux M., Maier-Hein L., et al.

Segmentation of Overlapping/Touched White Blood Cell Nuclei using ANN - CME Series on Hemato-Oncopathology, AIIMS, New Delhi.

Future Work

Improve classification accuracy using advanced deep learning techniques.

Explore attention-based models for better feature extraction.

Work on subtype identification to enhance leukemia diagnosis.
