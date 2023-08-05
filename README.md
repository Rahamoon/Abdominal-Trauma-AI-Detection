# AI-driven Abdominal Trauma Detection

This repository contains the code, models, and methodologies for detecting and grading abdominal injuries using CT scans. It was created as part of the RSNA Abdominal Trauma Detection AI Challenge, with the goal of developing a robust and accurate AI system to enhance trauma care.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Results](#results)
- [License](#license)
- [Contributing](#contributing)

## Introduction
Traumatic injury is a major public health problem and the most common cause of death in the first four decades of life. This project aims to leverage machine learning techniques to assist in the rapid and precise detection of injuries from CT scans, specifically focusing on injuries to the liver, kidneys, spleen, and bowel.

## Installation
Clone the repository and install the required dependencies:

```bash
git clone https://github.com/username/repo-name.git
cd repo-name
pip install -r requirements.txt
```

## Data Preprocessing
The dataset consists of CT scans in DICOM format along with accompanying CSV files that contain labels and metadata. Preprocessing involves loading, cleaning, augmenting, and normalizing the data to make it suitable for training deep learning models.

### Steps
1. **Loading Data**: Load DICOM images using Pydicom and CSV files using Pandas.
2. **Cleaning Data**: Remove or impute any missing values or anomalies.
3. **Data Augmentation**: Apply techniques like rotation, flipping, etc., to increase dataset diversity.
4. **Normalization**: Scale pixel values to the range [0, 1].

Refer to the `src/preprocessing` directory for scripts and detailed instructions.

## Model Training
The project uses a deep learning architecture designed specifically for detecting and grading abdominal injuries. The training involves the following steps:

1. **Model Definition**: Define the architecture using frameworks like TensorFlow or PyTorch.
2. **Training**: Train the model using the preprocessed data.
3. **Validation**: Validate the model using a separate validation set.
4. **Hyperparameter Tuning**: Optimize hyperparameters using techniques like grid search.

Scripts and notebooks related to model training can be found in the `src/models` and `notebooks` directories.

## Evaluation
Model evaluation is conducted using metrics such as accuracy, precision, recall, F1-score, and AUC-ROC. Detailed evaluation scripts are available in the `src/training` directory.

## Results
The trained models demonstrated promising results in detecting and grading injuries with high accuracy. For detailed results, visualizations, and discussion, please refer to the `results` directory.

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Contributing
Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

