# Retinal OCT Disease Classification

A deep learning pipeline for classifying retinal OCT images into four disease categories using VGG19 features, a lightweight custom CNN head, and data augmentation, with LIME explainability.

![GitHub stars](https://img.shields.io/github/stars/Abrar-Islam-Oitijjho/Retinal-OCT-Disease-Classification?style=social)
![GitHub forks](https://img.shields.io/github/forks/Abrar-Islam-Oitijjho/Retinal-OCT-Disease-Classification?style=social)
![GitHub issues](https://img.shields.io/github/issues/Abrar-Islam-Oitijjho/Retinal-OCT-Disease-Classification)
![GitHub pull requests](https://img.shields.io/github/issues-pr/Abrar-Islam-Oitijjho/Retinal-OCT-Disease-Classification)
![GitHub last commit](https://img.shields.io/github/last-commit/Abrar-Islam-Oitijjho/Retinal-OCT-Disease-Classification)


![Python](https://img.shields.io/badge/python-%233776AB.svg?style=for-the-badge&logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23F37626.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)

  
## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Method](#method)
- [Result](#result)
- [Quick Start](#quick-start)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Associated Publication](#associated-publication)
- [Contributing](#contributing)
- [Support](#support)
- [Acknowledgments](#acknowledgments)

## About

This project develops a deep learning pipeline for classifying retinal OCT images into four disease categories. The workflow includes sample visualization, image preprocessing, stratified train–test splitting, and real-time data augmentation to improve robustness. A pretrained VGG19 backbone is used as a fixed feature extractor, and a custom CNN classifier head is added to learn discriminative features specific to retinal pathology. The model is trained with checkpointing to preserve the best weights, and training dynamics are monitored through accuracy and loss curves. Final evaluation on a held-out test set provides a clear measure of real-world performance, demonstrating an effective end-to-end solution for automated retinal disease detection.

The proposed self-developed CNN model is comparatively smaller and simpler along with the use of Lime that introduces Explainable AI to the study and helps to increase the interpretability of the model. This addition will be an asset to the medical experts for getting major and detailed information and will help them in making final decisions and will also reduce the opacity and vulnerability of the conventional deep learning models.

This work has been published in IEEE Conference. The link to that can be found in the following section. 

## Features

- 🎯 **Disease Classification**: Accurately classifies OCT images into four categories: CNV, DME, Drusen, and Normal.
- ⚡ **Performance**: Utilizes deep learning techniques for high accuracy and efficient processing of OCT images.
- 🎨 **Visualization**: Provides tools for visualizing the model's predictions and understanding its decision-making process.
- 🔄 **Transfer Learning**: Leverages pre-trained models for faster training and improved performance.
- 🛠️ **Extensible**: Designed to be easily extended with new disease categories and imaging modalities.

## Method
| Step | Description |
|------|------------|
| Sample Visualization | Display a few images from each class |
| Data Preprocessing | Load images, resize to 224×224, normalize |
| Train–Test Split | Stratified 80/20 split |
| Data Augmentation | Rotation, shift, zoom during training |
| VGG19 Feature Extractor | Pretrained VGG19 with frozen convolutional layers for feature extraction |
| Custom Classification Head | Extra Conv layers, PReLU, Flatten, Dense, final Softmax |
| Model Compilation | Define loss, optimizer, and metrics |
| Model Training | Train with augmentation, save best weights |
| Training Curve Plots | Plot accuracy and loss across epochs |
| Final Evaluation | Load best model and evaluate on test data |

## Result

## Quick Start

Clone the repository and run the Jupyter Notebook:

```bash
git clone https://github.com/Abrar-Islam-Oitijjho/Retinal-OCT-Disease-Classification.git
cd Retinal-OCT-Disease-Classification
pip install -r requirements.txt
jupyter notebook Retinal-OCT-Disease-Classification.ipynb
```

Follow the instructions within the notebook to train and evaluate the model.

## Installation

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- TensorFlow
- Keras
- Other dependencies listed in `requirements.txt`

## Project Structure

```
Retinal-OCT-Disease-Classification/
├── 📄 retinal-xai-transfer-learning-vgg.ipynb  # Main Jupyter Notebook
├── 📄 OCT_CUSTOM_model.h5                      # The model
├── 📄 OCT_CUSTOM_weight.h5                     # The model's weight
├── 📄 requirements.txt                         # Python dependencies                   
└── 📄 README.md                                # This file
```

## Associated Publication

[Demystifying Deep Learning Models for Retinal OCT Disease Classification using Explainable AI](https://ieeexplore.ieee.org/abstract/document/9718400)

## Contributing

Contributions are welcome!

### Quick Contribution Steps
1. 🍴 Fork the repository
2. 🌟 Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. ✅ Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push to the branch (`git push origin feature/AmazingFeature`)
5. 🔃 Open a Pull Request


## Support

- 📧 **Email**: abraroitijjho35@gmail.com
- 🐛 **Issues**: [GitHub Issues](https://github.com/Abrar-Islam-Oitijjho/ARIMA-Modeling-on-EEG-Time-Series-Data/issues)

## Acknowledgments

🌟 Special thanks: to the co-authors of this paper.
