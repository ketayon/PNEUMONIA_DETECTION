
# PNEUMONIA_DETECTION

This project aims to develop quantum machine learning (QML) models for screening and detecting pneumonia from chest X-ray images. By harnessing the potential of quantum computing, these models strive to improve the accuracy and efficiency of pneumonia diagnosis, supporting timely medical interventions.

## Download latest version
[Chest X-ray Pneumonia Dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

## Project Overview

Pneumonia is a serious respiratory condition with high morbidity and mortality rates. Early detection is crucial for effective treatment. This project explores various quantum machine learning techniques for classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories.

## Models Implemented

The project includes multiple quantum machine learning models, each exploring different classification techniques:

- **PennyLane Model** (pennylane_pneumonia_detection.ipynb)
- **Qiskit Hybrid Model** (qiskit_hybrid_pneumonia_detection.ipynb)
- **torch Quantum Model** (torch_quantum_pneumonia_detection.ipynb)
- **Qiskit Machine Learning Model** (qiskit_ml_pneumonia_detection.ipynb)
- **Piqture Library Model** (piqture_pneumonia_detection.ipynb)
- **Quantum Kernel Trainer Model** (QuantumKernelTrainer_qiskit_pneumonia_detection.ipynb)
- **Ingenii Hybrid Model** (ingenii_pneumonia_detection.ipynb)
- **Fidelity Quantum Kernel Model** (FidelityQuantumKernel_qiskit_pneumonia_detection.ipynb)
- **QNNCircuit Model** (QNNCircuit_qiskit_pneumonia_detection.ipynb)
- **Pegasos Kernel Model** (Pegasos_qsvc_qiskit_pneumonia_detection.ipynb)

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

### 3. torch Quantum Model

```
precision    recall  f1-score   support

      NORMAL       0.94      0.48      0.63       234
   PNEUMONIA       0.76      0.98      0.86       390

    accuracy                           0.79       624
   macro avg       0.85      0.73      0.75       624
weighted avg       0.83      0.79      0.77       624
```

### 4. Quantum Kernel Trainer Model

```
Classification Report:
              precision    recall  f1-score   support

      NORMAL       1.00      0.10      0.18        10
   PNEUMONIA       0.76      1.00      0.87        29

    accuracy                           0.77        39
   macro avg       0.88      0.55      0.52        39
weighted avg       0.82      0.77      0.69        39

Confusion Matrix:
[[ 1  9]
 [ 0 29]]

ROC AUC Score: 0.6448275862068965
```

### 5. Ingenii Hybrid Model

```
Classification Report:
              precision    recall  f1-score   support

      NORMAL       0.92      0.59      0.72       234
   PNEUMONIA       0.80      0.97      0.88       390

    accuracy                           0.83       624
   macro avg       0.86      0.78      0.80       624
weighted avg       0.84      0.83      0.82       624
```

### 6. Pegasos Kernel Model

```
Pegasos Kernel Classification Report:
              precision    recall  f1-score   support

           0       0.39      0.50      0.43       234
           1       0.64      0.53      0.58       390

    accuracy                           0.52       624
   macro avg       0.51      0.51      0.51       624
weighted avg       0.54      0.52      0.52       624

Confusion Matrix:
[[116 118]
 [184 206]]
```

### 7. Updated Pegasos Kernel Model

Pegasos Kernel Classification Report:
              precision    recall  f1-score   support

           0       0.75      0.03      0.05       234
           1       0.63      0.99      0.77       390

    accuracy                           0.63       624
   macro avg       0.69      0.51      0.41       624
weighted avg       0.67      0.63      0.50       624

Confusion Matrix:
[[  6 228]
 [  2 388]]

## Performance Summary

- **PennyLane Model**: Balanced performance with reasonable accuracy (0.79). Needs improvement in detecting NORMAL cases.
- **Qiskit Hybrid Model**: Strong pneumonia recall but lower precision for NORMAL cases, with overall accuracy of 0.71.
- **torch Quantum Model**: Balanced performance with accuracy of 0.79. Needs better consistency for NORMAL cases.
- **Quantum Kernel Trainer Model**: Achieves 70% accuracy and ROC AUC of 0.74, indicating promising potential.
- **Ingenii Hybrid Model**: Best performance with accuracy of 0.83 and balanced results for both classes.
- **Pegasos Kernel Model**: Accuracy of 0.55, requiring further optimization.

### Requirements

- **Python 3.9** or later
- Libraries: pennylane, qiskit, numpy, scikit-learn, torch, matplotlib, PIL (Pillow), piqture

Install the libraries via pip:

```bash
pip install pennylane qiskit numpy scikit-learn torch matplotlib pillow piqture
```

### Running the Models

Each model is in its respective notebook:

- **PennyLane Model**: pennylane_pneumonia_detection.ipynb
- **Qiskit Hybrid Model**: qiskit_hybrid_pneumonia_detection.ipynb
- **torch Quantum Model**: torch_quantum_pneumonia_detection.ipynb
- **Quantum Kernel Trainer Model**: QuantumKernelTrainer_qiskit_pneumonia_detection.ipynb
- **Pegasos Kernel Model**: Pegasos_qsvc_qiskit_pneumonia_detection.ipynb

### Dataset

Ensure the dataset is organized into separate folders for **NORMAL** and **PNEUMONIA**. Update paths in the notebooks as needed.

## Conclusion

This project highlights the promise of quantum machine learning in medical imaging, particularly for pneumonia detection. Refining models like torch Quantum Model and leveraging GPUs can enhance performance and generalization.
Yet, quantum models are swiftly closing the gap, challenging the dominance of traditional approaches 🚀
