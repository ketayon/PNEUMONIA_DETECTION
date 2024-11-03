
# PNEUMONIA_DETECTION

This project aims to develop quantum machine learning (QML) models for the screening and detection of pneumonia from chest X-ray images. By harnessing the potential of quantum computing, these models strive to improve the accuracy and efficiency of pneumonia diagnosis, supporting timely medical interventions.

## Project Overview

Pneumonia is a serious respiratory condition with high morbidity and mortality rates. Early detection is crucial for effective treatment. This project explores various quantum machine learning techniques for classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories.

## Models Implemented

The project includes multiple quantum machine learning models, each exploring different classification techniques:

- **PennyLane Model** (`pennylane_pneumonia_detection`)
- **Qiskit Hybrid Model** (`qiskit_hybrid_pneumonia_detection`)
- **Quantum Model** (`quantum_pneumonia_detection`)
- **Qiskit Machine Learning Model** (`qiskit_ml_pneumonia_detection`)
- **Piqture Library Model** (`piqture_pneumonia_detection`) - Utilizes specific layers from the `piqture` library.

## Classification Reports

### 1. PennyLane Model

```
              precision    recall  f1-score   support

      NORMAL       0.85      0.54      0.66       234
   PNEUMONIA       0.77      0.94      0.85       390

    accuracy                           0.79       624
   macro avg       0.81      0.74      0.75       624
weighted avg       0.80      0.79      0.78       624
```

### 2. Qiskit Hybrid Model

```
              precision    recall  f1-score   support

      NORMAL       0.98      0.23      0.37       234
   PNEUMONIA       0.68      1.00      0.81       390

    accuracy                           0.71       624
   macro avg       0.83      0.61      0.59       624
weighted avg       0.80      0.71      0.65       624
```

### 3. Quantum Model

```
              precision    recall  f1-score   support

      NORMAL       0.94      0.48      0.63       234
   PNEUMONIA       0.76      0.98      0.86       390

    accuracy                           0.79       624
   macro avg       0.85      0.73      0.75       624
weighted avg       0.83      0.79      0.77       624
```

### 4. Qiskit Machine Learning Model

```
Accuracy from the training data: 49.6%
***************************************************
Accuracy from the test data: 48.33%
***************************************************
Accuracy: 47.92%
```

### 5. Piqture Library Model

The `piqture_pneumonia_detection.ipynb` model is the latest addition, and it integrates specialized layers from the `piqture` library. Its initial performance with the current configuration is as follows:

```
Accuracy from the training data: 49.6%
***************************************************
Accuracy from the test data: 48.33%
***************************************************
Accuracy: 47.92%
```

## Performance Summary

- **PennyLane Model**: Shows the best overall performance, with a balanced precision and recall.
- **Qiskit Hybrid Model**: High precision for the NORMAL class but struggles with recall.
- **Quantum Model**: Offers reasonable performance but needs consistency across classes.
- **Qiskit Machine Learning Model**: Requires further refinement due to lower accuracy.
- **Piqture Library Model**: Uses advanced layers, demonstrating the potential of model customization.

## Usage

### Requirements

To run the models, you need the following:

- **Python 3.7** or later
- Key libraries:
  - `pennylane`
  - `qiskit`
  - `numpy`
  - `scikit-learn`
  - `torch`
  - `matplotlib`
  - `PIL` (Pillow)
  - `piqture` (if using the `piqture_pneumonia_detection.ipynb` model)

Install the libraries via pip:

```bash
pip install pennylane qiskit numpy scikit-learn torch matplotlib pillow piqture
```

### Running the Models

Each model is in its respective notebook:

- **PennyLane Model**: `pennylane_pneumonia_detection.ipynb`
- **Qiskit Hybrid Model**: `qiskit_hybrid_pneumonia_detection.ipynb`
- **Quantum Model**: `quantum_pneumonia_detection.ipynb`
- **Qiskit Machine Learning Model**: `qiskit_ml_pneumonia_detection.ipynb`
- **Piqture Library Model**: `piqture_pneumonia_detection.ipynb`

### Dataset

Ensure that the dataset of chest X-ray images is organized into separate folders for **NORMAL** and **PNEUMONIA** classes. Update dataset paths as needed in each notebook.

## Conclusion

This project highlights the promise of quantum machine learning in medical imaging, particularly for detecting pneumonia from chest X-ray images. However, **improving the accuracy and generalization of qiskit_machine_learning models requires powerful devices equipped with GPUs**. These resources facilitate faster computation, especially when optimizing parameters, thus enabling better performance and consistency.

## Acknowledgements

We thank the quantum computing and medical imaging communities for their foundational work, which has been instrumental in this project.
