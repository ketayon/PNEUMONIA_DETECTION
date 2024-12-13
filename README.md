
# PNEUMONIA_DETECTION

This project aims to develop quantum machine learning (QML) models for screening and detecting pneumonia from chest X-ray images. By harnessing the potential of quantum computing, these models strive to improve the accuracy and efficiency of pneumonia diagnosis, supporting timely medical interventions.

## Project Overview

Pneumonia is a serious respiratory condition with high morbidity and mortality rates. Early detection is crucial for effective treatment. This project explores various quantum machine learning techniques for classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories.

## Models Implemented

The project includes multiple quantum machine learning models, each exploring different classification techniques:

- **PennyLane Model** (pennylane_pneumonia_detection)
- **Qiskit Hybrid Model** (qiskit_hybrid_pneumonia_detection)
- **Quantum Model** (quantum_pneumonia_detection)
- **Qiskit Machine Learning Model** (qiskit_ml_pneumonia_detection)
- **Piqture Library Model** (piqture_pneumonia_detection)
- **Quantum Kernel Trainer Model** (QuantumKernelTrainer_qiskit_pneumonia_detection) - Uses QuantumKernelTrainer from Qiskit.
- **Ingenii Hybrid Model** (ìngenii_pneumonia_detection)
- **Fidelity Quantum Kernel Model** (FidelityQuantumKernel_qiskit_pneumonia_detection)
- **QNNCircuit Model** (QNNCircuit_giskit_pneumonia_detection)
- **Quantum Kernel Trainer Copy** (QuantumKernelTrainer_qiskit_pneumonia_detection)

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

Accuracy from the training data: **74.4%**
Accuracy from the test data: **68.0%**

### 5. Piqture Library Model

Accuracy from the training data: **74.4%**
Accuracy from the test data: **68.0%**

### 6. Quantum Kernel Trainer Model

The QuantumKernelTrainer_qiskit_pneumonia_detection notebook provides the following classification report with **8 qubits**:

Classification Report: 
```
{
    '0': {
        'precision': 1.0,
        'recall': 0.1,
        'f1-score': 0.18181818181818182,
        'support': 10.0
    },
    '1': {
        'precision': 0.7631578947368421,
        'recall': 1.0,
        'f1-score': 0.8656716417910447,
        'support': 29.0
    },
    'accuracy': 0.7692307692307693,
    'macro avg': {
        'precision': 0.881578947368421,
        'recall': 0.55,
        'f1-score': 0.5237449118046132,
        'support': 39.0
    },
    'weighted avg': {
        'precision': 0.8238866396761134,
        'recall': 0.7692307692307693,
        'f1-score': 0.690324600772362,
        'support': 39.0
    }
}
```

Confusion Matrix:
```
[[ 1  9]
 [ 0 29]]
```

ROC AUC Score: 0.6448275862068965

### 7. Ingenii Hybrid Model

```
Classification Report:
              precision    recall  f1-score   support

      NORMAL       0.92      0.59      0.72       234
   PNEUMONIA       0.80      0.97      0.88       390

    accuracy                           0.83       624
   macro avg       0.86      0.78      0.80       624
weighted avg       0.84      0.83      0.82       624
```

### 8. Fidelity Quantum Kernel Model

Classification Report: 
```
{
    '0': {
        'precision': 0.25,
        'recall': 0.4,
        'f1-score': 0.3076923076923077,
        'support': 10.0
    },
    '1': {
        'precision': 0.7391304347826086,
        'recall': 0.5862068965517241,
        'f1-score': 0.6538461538461539,
        'support': 29.0
    },
    'accuracy': 0.5384615384615384,
    'macro avg': {
        'precision': 0.4945652173913043,
        'recall': 0.49310344827586206,
        'f1-score': 0.4807692307692308,
        'support': 39.0
    },
    'weighted avg': {
        'precision': 0.6137123745819398,
        'recall': 0.5384615384615384,
        'f1-score': 0.5650887573964497,
        'support': 39.0
    }
}
```

Confusion Matrix:
```
[[ 4  6]
 [12 17]]
```

ROC AUC Score: 0.5413793103448277

### 9. QNNCircuit Model

Accuracy: 0.5
- Precision: 0.6258064516129033
- Recall: 0.49743589743589745
- F1 Score: 0.5542857142857143

Confusion Matrix:
```
[[118 116]
 [196 194]]
```

## Performance Summary

- **PennyLane Model**: Balanced performance with reasonable accuracy (0.79). Needs improvement in detecting NORMAL cases.
- **Qiskit Hybrid Model**: Strong pneumonia recall but lower precision for NORMAL cases, with overall accuracy of 0.71.
- **Quantum Model**: Balanced performance with accuracy of 0.79. Needs better consistency for NORMAL cases.
- **Qiskit Machine Learning Model**: Test accuracy of 68%. Needs refinement for better generalization.
- **Piqture Library Model**: Similar to Qiskit ML Model with 68% accuracy. Requires further optimization.
- **Quantum Kernel Trainer Model**: Achieves 70% accuracy and ROC AUC of 0.74, indicating promising potential.
- **Ingenii Hybrid Model**: Best performance with accuracy of 0.83 and balanced results for both classes.

## Usage

### Requirements

- **Python 3.7** or later
- Libraries: pennylane, qiskit, numpy, scikit-learn, torch, matplotlib, PIL (Pillow), piqture

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
- **Quantum Kernel Trainer Model**: `QuantumKernelTrainer_qiskit_pneumonia_detection.ipynb`

### Dataset

Ensure the dataset is organized into separate folders for **NORMAL** and **PNEUMONIA**. Update paths in the notebooks as needed.

## Conclusion

This project highlights the promise of quantum machine learning in medical imaging, particularly for pneumonia detection. Refining models like Qiskit ML and leveraging GPUs can enhance performance and generalization.

## Acknowledgements

We thank the quantum computing and medical imaging communities for their foundational work, which has been instrumental in this project.
