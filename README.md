# AppliedAIinBiomedicine
### Chest X-Ray images classification: Tuberculosis Detector (Final Project 2022 - 2023)
_Team members: Alix de Langlais, Felipe Pascutti, Gianmarco Tardini and Pedro Gianjoppe_  
M.Sc. Biomedical Engineering - Politecnico di Milano - Milan, Italy

## Dataset
The dataset used for this project is composed of 15470 X-Ray images, stored in PNG or JPEG format. These images come from healthy patients, patients with pneumonia or tuberculosis. A .csv file allows the name of a specific file to be associated with the class to which it belongs.  
The dataset is unbalanced according to the class distribution which is as follows: 9354 images for the normal patients, 4250 for the pneumonia patients, and 1866 for the tuberculosis patients.

![img](https://github.com/Adelanglais/AppliedAIinBiomedicine/blob/111de3d380857be3e0d20068a6ca7931acb31981/dataset_example.png)

## Models
Three different approaches were implemented for this classification problem:  
+ Convolutional Neural Networks (CNN)
+ Transfer learning applied to CNN
+ Machine learning classifier with features extracted with CNN
The dataset, the network architectures as well as the different training strategies are described in the report.

## Results

| Model          | F1 - Normal | F1 - Pneumonia | F1 - Tuberculosis |
| -------------- | ----------- | -------------- | ----------------- |
| CNN            | 0.8915      | 0.9108         | 0.9639            |
| EfficientNetB0 | 0.9882      | 0.9559         | 0.9908            |
| VGG19 + SVM    | 0.9800      | 1.0000         | 0.9800            |

## XAI
