# Pneumonia Detection Models - Comparative Analysis

## Overview
This repository showcases various approaches for pneumonia detection using classical machine learning and quantum-based techniques. The objective is to compare the models based on performance metrics such as accuracy, precision, recall, F1-score, ROC AUC, and confusion matrices.

The models include traditional machine learning algorithms, hybrid quantum-classical models, and fully quantum-based implementations.

---

## Models Implemented

1. **classical_pneumonia_detection.ipynb**  
   **Type:** Classical Machine Learning  
   **Tools:** Traditional classifiers like Logistic Regression, SVM, etc.

2. **FidelityQuantumKernel_qiskit_pneumonia_detection.ipynb**  
   **Type:** Quantum Kernel-Based Machine Learning  
   **Tools:** Qiskit Fidelity Quantum Kernel

3. **ingenii_pneumonia_detection.ipynb**  
   **Type:** Classical Machine Learning  
   **Tools:** Custom Classical Techniques

4. **pennylane_pneumonia_detection.ipynb**  
   **Type:** Quantum Machine Learning  
   **Tools:** PennyLane Framework

5. **piqture_pneumonia_detection.ipynb**  
   **Type:** Quantum/Hybrid Quantum  
   **Tools:** Piqture Quantum Techniques

6. **qiskit_hybrid_pneumonia_detection.ipynb**  
   **Type:** Hybrid Quantum-Classical Model  
   **Tools:** Qiskit Hybrid ML Framework

7. **qiskit_ml_pneumonia_detection.ipynb**  
   **Type:** Quantum Machine Learning  
   **Tools:** Qiskit ML Libraries

8. **qml_torch_pneumonia_detection.ipynb**  
   **Type:** Quantum Torch-Based Model  
   **Tools:** PyTorch and Quantum ML Integration

9. **QuantumKernelTrainer_qiskit_pneumonia_detection.ipynb**  
    **Type:** Quantum Kernel Training  
    **Tools:** Qiskit Quantum Kernel Trainer

10. **Pegasos_qsvc_qiskit_pneumonia_detection.ipynb**  
    **Type:** Quantum Kernel-Based Machine Learning  
    **Tools:** Qiskit Fidelity Quantum Kernel

11. **Pegasos_upgraded_qsvc_qiskit_pneumonia_detection.ipynb**  
    **Type:** Quantum Kernel-Based Machine Learning  
    **Tools:** Qiskit Fidelity Quantum Kernel

---

## Performance Comparison

| Model                                           | Accuracy (%) | Precision (0/1) | Recall (0/1) | F1-Score (0/1) | ROC AUC Score | Notes                         |
|------------------------------------------------|-------------|----------------|--------------|----------------|---------------|--------------------------------|
| **classical_pneumonia_detection**              | 78.45       | 0.85 / 0.72    | 0.60 / 0.90  | 0.70 / 0.80    | 0.8400        | Balanced performance          |
| **FidelityQuantumKernel_qiskit**               | 63.20       | 0.70 / 0.60    | 0.30 / 0.85  | 0.42 / 0.70    | -             | High recall imbalance         |
| **ingenii_pneumonia_detection**                | 70.00       | 0.65 / 0.77    | 0.85 / 0.55  | 0.73 / 0.63    | -             | Moderate performance          |
| **pennylane_pneumonia_detection**              | 81.00       | 0.88 / 0.76    | 0.72 / 0.90  | 0.79 / 0.82    | -             | High accuracy                 |
| **piqture_pneumonia_detection**                | 52.10       | -              | -            | -              | -             | Poor performance              |
| **qiskit_hybrid_pneumonia_detection**          | 88.00       | 1.0 / 0.82     | 0.75 / 1.0   | 0.85 / 0.90    | -             | Best overall performance      |
| **qiskit_ml_pneumonia_detection**              | 45.00       | -              | -            | -              | -             | Low accuracy                  |
| **qml_torch_pneumonia_detection**              | 75.00       | 0.73 / 0.77    | 0.72 / 0.78  | 0.73 / 0.77    | -             | Balanced performance          |
| **QuantumKernelTrainer_qiskit**                | 65.50       | 0.80 / 0.65    | 0.30 / 0.92  | 0.43 / 0.75    | 0.7000        | Imbalanced recall             |
| **Pegasos_qsvc_qiskit_pneumonia_detection**    | 60.00       | 0.60 / 0.62    | 0.45 / 0.75  | 0.51 / 0.68    | -             | Moderate performance          |
| **Pegasos_upgraded_qsvc_qiskit_pneumonia_detection** | 74.00  | 0.80 / 0.72  | 0.60 / 0.85  | 0.68 / 0.78    | -             | Moderate performance          |

---

## Key Observations

1. **Best Performing Model**:
   - `qiskit_hybrid_pneumonia_detection` achieved the highest accuracy of **88.00%** with balanced precision, recall, and F1-scores.

2. **Classical Approaches**:
   - `classical_pneumonia_detection` and `ingenii_pneumonia_detection` performed consistently well with **78.45%** and **70.00%** accuracy, respectively.

3. **Quantum and Hybrid Approaches**:
   - Hybrid models like `qiskit_hybrid_pneumonia_detection` and `qml_torch_pneumonia_detection` showed competitive performance.
   - Pure quantum models (e.g., `QuantumKernelTrainer_qiskit` and `FidelityQuantumKernel_qiskit`) had lower accuracies, indicating challenges in generalization.

4. **Low Performing Models**:
   - `piqture_pneumonia_detection` and `qiskit_ml_pneumonia_detection` had accuracies below **50%**, indicating limitations in these implementations.

5. **Imbalance Challenges**:
   - Several quantum models showed high recall for class `1` but poor recall for class `0`. Balancing techniques may improve these results.

---

## Conclusion

- **Hybrid quantum-classical models** outperform pure quantum models in pneumonia detection tasks.
- Classical models remain strong contenders, with robust and reliable results.
- Further improvements in quantum models could focus on balancing class performance and tuning hyperparameters.

---

## Results Summary

| Metric                    | Best Model                           | Score     |
|---------------------------|---------------------------------------|-----------|
| **Accuracy**              | qiskit_hybrid_pneumonia_detection    | 88.00%    |
| **F1-Score**              | qiskit_hybrid_pneumonia_detection    | 0.90 / 0.85 |
| **ROC AUC Score**         | classical_pneumonia_detection        | 0.8400    |
| **Balanced Performance**  | pennylane_pneumonia_detection        | High      |

---

## Acknowledgements
- **Frameworks Used**: Qiskit, PennyLane, PyTorch, Scikit-Learn.
