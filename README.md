# PNEUMONIA_DETECTION

This project aims to develop quantum machine learning (QML) models for screening and detecting pneumonia from chest X-ray images. By harnessing the potential of quantum computing, these models strive to improve the accuracy and efficiency of pneumonia diagnosis, supporting timely medical interventions.

## Download Latest Version
Chest X-ray Pneumonia Dataset

## Project Overview

Pneumonia is a serious respiratory condition with high morbidity and mortality rates. Early detection is crucial for effective treatment. This project explores various quantum machine learning techniques for classifying chest X-ray images into NORMAL and PNEUMONIA categories.

## Models Implemented

The project includes multiple quantum machine learning models, each exploring different classification techniques:

1. **PennyLane Model** (`pennylane_pneumonia_detection.ipynb`)
   - **Accuracy**: 89.80%
   - **Precision**: 1.00 (Normal), 0.88 (Tumor)
   - **Recall**: 0.58 (Normal), 1.00 (Tumor)
   - **F1-Score**: 0.74 (Normal), 0.94 (Tumor)
   - **ROC AUC Score**: 0.8964

2. **Qiskit Hybrid Model** (`qiskit_hybrid_pneumonia_detection.ipynb`)
   - **Accuracy**: 81.70%
   - **Precision**: 0.80 (Normal), 0.82 (Pneumonia)
   - **Recall**: 0.38 (Normal), 0.97 (Pneumonia)
   - **F1-Score**: 0.52 (Normal), 0.89 (Pneumonia)

3. **torch Quantum Model** (`torch_quantum_pneumonia_detection.ipynb`)
   - **Accuracy**: 81.41%
   - **Precision**: 0.89 (Normal), 0.81 (Pneumonia)
   - **Recall**: 0.31 (Normal), 0.99 (Pneumonia)
   - **F1-Score**: 0.46 (Normal), 0.89 (Pneumonia)
   - **ROC AUC Score**: 0.6501

4. **Qiskit Machine Learning Model** (`qiskit_ml_pneumonia_detection.ipynb`)
   - **Training Accuracy**: 72.36%
   - **Test Accuracy**: 66.67%
   - **Overall Accuracy**: 62.92%

5. **Piqture Library Model** (`piqture_pneumonia_detection.ipynb`)
   - **Training Accuracy**: 63.45%
   - **Test Accuracy**: 55.1%
   - **Overall Accuracy**: 58.56%

6. **Quantum Kernel Trainer Model** (`QuantumKernelTrainer_qiskit_pneumonia_detection.ipynb`)
   - **Accuracy**: 76.92%
   - **Precision**: 1.00 (Normal), 0.76 (Pneumonia)
   - **Recall**: 0.10 (Normal), 1.00 (Pneumonia)
   - **F1-Score**: 0.18 (Normal), 0.87 (Pneumonia)
   - **ROC AUC Score**: 0.6448

7. **Ingenii Hybrid Model** (`ingenii_pneumonia_detection.ipynb`)
   - **Test Accuracy**: 89.87%
   - **Precision**: 0.93 (Normal), 0.89 (Pneumonia)
   - **Recall**: 0.65 (Normal), 0.98 (Pneumonia)
   - **F1-Score**: 0.76 (Normal), 0.94 (Pneumonia)

8. **Fidelity Quantum Kernel Model** (`FidelityQuantumKernel_qiskit_pneumonia_detection.ipynb`)
   - **Accuracy**: 70%
   - **Precision**: 0.67 (Normal), 0.75 (Pneumonia)
   - **Recall**: 0.80 (Normal), 0.60 (Pneumonia)
   - **F1-Score**: 0.73 (Normal), 0.67 (Pneumonia)

9. **QNNCircuit Model** (`QNNCircuit_qiskit_pneumonia_detection.ipynb`)
   - **Accuracy**: 50%
   - **Precision**: 0.63
   - **Recall**: 0.50
   - **F1-Score**: 0.55

10. **Pegasos Kernel Model** (`Pegasos_qsvc_qiskit_pneumonia_detection.ipynb`)
    - **Accuracy**: 52%
    - **Precision**: 0.39 (Normal), 0.64 (Pneumonia)
    - **Recall**: 0.50 (Normal), 0.53 (Pneumonia)
    - **F1-Score**: 0.43 (Normal), 0.58 (Pneumonia)

11. **Upgraded Pegasos Kernel Model** (`Pegasos_upgrated_qsvc_qiskit_pneumonia_detection.ipynb`)
    - **Accuracy**: 63%
    - **Precision**: 0.75 (Normal), 0.63 (Pneumonia)
    - **Recall**: 0.03 (Normal), 0.99 (Pneumonia)
    - **F1-Score**: 0.05 (Normal), 0.77 (Pneumonia)

## Comparison and Conclusions

- **Highest Accuracy**: Ingenii Hybrid Model (89.87%) and PennyLane Model (89.80%) demonstrated the best performance overall in terms of accuracy.
- **Best Precision and F1-Score**: PennyLane Model exhibited excellent precision (1.00 for Normal and 0.88 for Tumor) and high F1-scores.
- **Challenges in Recall**: Models like the Quantum Kernel Trainer and Upgraded Pegasos Kernel showed high precision but struggled with recall for specific classes.
- **Balanced Performance**: Qiskit Hybrid and torch Quantum models provided a balanced trade-off between precision and recall, making them suitable for general-purpose usage.

Overall, the Ingenii Hybrid and PennyLane models are recommended for their superior accuracy and robust performance across multiple metrics.

---
