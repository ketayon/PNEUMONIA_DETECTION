PNEUMONIA_DETECTION
This project aims to develop quantum machine learning (QML) models for the screening and detection of pneumonia from chest X-ray images. The models leverage the power of quantum computing to enhance the accuracy and efficiency of pneumonia diagnosis, which is crucial for timely medical intervention.

Project Overview
Pneumonia is a serious respiratory condition that can lead to significant morbidity and mortality. Early detection is essential for effective treatment. This project explores various quantum machine learning techniques to improve the classification of chest X-ray images into two categories: NORMAL and PNEUMONIA.

Models Implemented
The project includes several models based on quantum machine learning frameworks, each demonstrating different approaches to the classification task. The following models have been implemented:

PennyLane Model (pennylane_pneumonia_detection)
Qiskit Hybrid Model (qiskit_hybrid_pneumonia_detection)
Quantum Model (quantum_pneumonia_detection)
Qiskit Machine Learning Model (qiskit_ml_pneumonia_detection)
Classification Reports
1. PennyLane Model
markdown
Copy code
              precision    recall  f1-score   support

      NORMAL       0.85      0.54      0.66       234
   PNEUMONIA       0.77      0.94      0.85       390

    accuracy                           0.79       624
   macro avg       0.81      0.74      0.75       624
weighted avg       0.80      0.79      0.78       624
2. Qiskit Hybrid Model
markdown
Copy code
              precision    recall  f1-score   support

      NORMAL       0.98      0.23      0.37       234
   PNEUMONIA       0.68      1.00      0.81       390

    accuracy                           0.71       624
   macro avg       0.83      0.61      0.59       624
weighted avg       0.80      0.71      0.65       624
3. Quantum Model
markdown
Copy code
              precision    recall  f1-score   support

      NORMAL       0.94      0.48      0.63       234
   PNEUMONIA       0.76      0.98      0.86       390

    accuracy                           0.79       624
   macro avg       0.85      0.73      0.75       624
weighted avg       0.83      0.79      0.77       624
4. Qiskit Machine Learning Model
markdown
Copy code
Accuracy from the training data: 35.1%
***************************************************
Accuracy from the test data: 33.5%
***************************************************
Accuracy: 33.75%
Performance Summary
The PennyLane Model shows the best overall performance, with a balanced precision and recall for both classes.
The Qiskit Hybrid Model exhibits high precision for the NORMAL class but struggles with recall, indicating a potential issue with false negatives.
The Quantum Model provides reasonable performance but still highlights the challenges in achieving consistent classification across both classes.
The Qiskit Machine Learning Model currently demonstrates lower accuracy and indicates that further refinement is needed to improve its performance.
Usage
Requirements
To run the models, ensure you have the following installed:

Python 3.7 or later
Required libraries:
pennylane
qiskit
numpy
scikit-learn
torch
matplotlib
PIL (Pillow)
You can install the required libraries using pip:

bash
Copy code
pip install pennylane qiskit numpy scikit-learn torch matplotlib pillow
Running the Models
Each model is implemented in its respective notebook. To execute a model, open the Jupyter Notebook and run the cells sequentially. Make sure to set the correct paths for the dataset you intend to use.

PennyLane Model: Open pennylane_pneumonia_detection.ipynb and execute the cells.
Qiskit Hybrid Model: Open qiskit_hybrid_pneumonia_detection.ipynb.
Quantum Model: Open quantum_pneumonia_detection.ipynb.
Qiskit Machine Learning Model: Open qiskit_ml_pneumonia_detection.ipynb.
Dataset
The models are designed to work with a dataset of chest X-ray images. Ensure that the dataset is organized correctly, typically with separate folders for NORMAL and PNEUMONIA classes. You can modify the dataset paths in the notebooks as necessary.

Conclusion
This project showcases the potential of quantum machine learning in the medical domain, particularly for screening pneumonia from chest X-ray images. While initial results are promising, ongoing work is required to improve accuracy and generalization across different models.

Acknowledgements
We acknowledge the contributions of the quantum computing community and the researchers in the field of medical imaging for their foundational work that enables this project.
