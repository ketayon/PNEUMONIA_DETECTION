
# PNEUMONIA_DETECTION

This project aims to develop quantum machine learning (QML) models for screening and detecting pneumonia from chest X-ray images. By harnessing the potential of quantum computing, these models strive to improve the accuracy and efficiency of pneumonia diagnosis, supporting timely medical interventions.

## Project Overview

Pneumonia is a serious respiratory condition with high morbidity and mortality rates. Early detection is crucial for effective treatment. This project explores various quantum machine learning techniques for classifying chest X-ray images into **NORMAL** and **PNEUMONIA** categories.

## Models Implemented

The project includes multiple quantum machine learning models, each exploring different classification techniques:

- **PennyLane Model** (`pennylane_pneumonia_detection`)
- **Qiskit Hybrid Model** (`qiskit_hybrid_pneumonia_detection`)
- **Quantum Model** (`quantum_pneumonia_detection`)
- **Qiskit Machine Learning Model** (`qiskit_ml_pneumonia_detection`)
- **Piqture Library Model** (`piqture_pneumonia_detection`)
- **Quantum Kernel Trainer Model** (`QuantumKernelTrainer_qiskit_pneumonia_detection`) - Uses `QuantumKernelTrainer` from Qiskit.
- **Ingenii Hybrid Model** (`ìngenii_pneumonia_detection`)

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
Accuracy from the training data: 74.4%
***************************************************
Accuracy from the test data: 68.0%
***************************************************
Accuracy: 68.00%
```

### 5. Piqture Library Model

```
Accuracy from the training data: 74.4%
***************************************************
Accuracy from the test data: 68.0%
***************************************************
Accuracy: 68.00%
```

### 6. Quantum Kernel Trainer Model

The `QuantumKernelTrainer_qiskit_pneumonia_detection` notebook provides the following classification report with **8 qubits**:

```
Classification Report:
{
    '0.0': {
        'precision': 0.6875,
        'recall': 0.7333333333333333,
        'f1-score': 0.7096774193548387,
        'support': 30.0
    },
    '1.0': {
        'precision': 0.7142857142857143,
        'recall': 0.6666666666666666,
        'f1-score': 0.6896551724137931,
        'support': 30.0
    },
    'accuracy': 0.7,
    'macro avg': {
        'precision': 0.7008928571428572,
        'recall': 0.7,
        'f1-score': 0.699666295884316,
        'support': 60.0
    },
    'weighted avg': {
        'precision': 0.7008928571428572,
        'recall': 0.7,
        'f1-score': 0.6996662958843161,
        'support': 60.0
    }
}

Confusion Matrix:
 [[22  8]
 [10 20]]

ROC AUC Score: 0.74
```

### 7.Ingenii Hybrid Model

```
Classification Report:
              precision    recall  f1-score   support

      NORMAL       0.92      0.59      0.72       234
   PNEUMONIA       0.80      0.97      0.88       390

    accuracy                           0.83       624
   macro avg       0.86      0.78      0.80       624
weighted avg       0.84      0.83      0.82       624

```

## Performance Summary

**PennyLane Model**: Shows good overall performance with a high recall for PNEUMONIA but struggles with NORMAL case detection. It achieves a balanced precision for both classes but requires improvement in the recall for NORMAL cases. The overall accuracy is reasonable (0.79).
- **Qiskit Hybrid Model**: Has very high precision for NORMAL but a low recall, making it good at identifying correct NORMAL cases but missing many others. The recall for PNEUMONIA is perfect (1.00), indicating it detects all pneumonia cases but at the cost of lower precision for PNEUMONIA. The model’s overall accuracy is 0.71, showing an imbalance between precision and recall.
- **Quantum Model**: Provides reasonable performance with a balanced approach compared to other models. It performs well for PNEUMONIA detection (high recall of 0.98) but needs improvement in the detection of NORMAL cases (recall of 0.48). It achieves an accuracy of 0.79, but consistency across classes can be improved.
- **Qiskit Machine Learning Model**: Requires further refinement, as it shows relatively low accuracy (68%) on the test data. Although the training accuracy is higher, the model struggles with generalization, indicating a need for better parameter optimization and potential use of GPUs.
- **Piqture Library Model**: Like the Qiskit Machine Learning Model, it demonstrates lower accuracy (68%) and needs refinement to better generalize on test data. This model shows potential but is limited by inconsistent performance.
- **Quantum Kernel Trainer Model**: Achieves an accuracy of 70% and a ROC AUC score of 0.74, reflecting promising potential in distinguishing between classes. It has a relatively balanced performance in terms of precision and recall but can be further improved for higher accuracy.
- **Ingenii Hybrid Model**: Best overall performance with an accuracy of 0.83. It shows a strong F1-score for PNEUMONIA (0.88) and performs well in NORMAL detection, though it could benefit from better recall for NORMAL (0.59). This model strikes the best balance across both classes and shows the most consistent performance.


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
- **Quantum Kernel Trainer Model**: `QuantumKernelTrainer_qiskit_pneumonia_detection.ipynb`

### Dataset

Ensure that the dataset of chest X-ray images is organized into separate folders for **NORMAL** and **PNEUMONIA** classes. Update dataset paths as needed in each notebook.

## Conclusion

This project highlights the promise of quantum machine learning in medical imaging, particularly for detecting pneumonia from chest X-ray images. **Improving accuracy and generalization of models, especially the `qiskit_ml_pneumonia_detection`, requires powerful GPUs for faster parameter optimization and better consistency**.

## Acknowledgements

We thank the quantum computing and medical imaging communities for their foundational work, which has been instrumental in this project.
