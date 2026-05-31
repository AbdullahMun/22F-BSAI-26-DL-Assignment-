**Deep Learning Assignment**

**Overview**

This project focuses on predicting patient survival outcomes using a healthcare dataset containing patient demographics, medical measurements, and hospital-related information. Different deep learning models were implemented and compared to evaluate their performance on the prediction task.

The main objective was to analyze how various neural network architectures perform on real-world medical data and identify the most effective model.

**Dataset**

The dataset used in this project is a hospital patient dataset containing approximately 91,000 records and 85 attributes.

Target Variable

- hospital_death
  - 0 = Patient Survived
  - 1 = Patient Died

Features

The dataset includes:

- Patient age and BMI
- Height and weight
- Medical history information
- ICU admission details
- Laboratory measurements
- Physiological indicators
- Hospital-related attributes

**Data Preprocessing**

Several preprocessing steps were performed before training the models:

1. Removed records with missing target values.
2. Selected numerical features for model training.
3. Handled missing values using imputation techniques.
4. Standardized feature values using scaling.
5. Split the dataset into training and testing sets.
6. Converted data into PyTorch tensors for deep learning models.

**Models Implemented**

1. Deep Neural Network (DNN)

A fully connected neural network was used as the baseline model. Multiple hidden layers, ReLU activation functions, dropout, and batch normalization were applied to improve performance and reduce overfitting.

2. Long Short-Term Memory (LSTM)

An LSTM-based model was implemented to learn complex patterns from sequential representations of patient data.

3. Bidirectional LSTM (Bi-LSTM)

A Bidirectional LSTM was trained to capture information from both forward and backward directions.

4. Gated Recurrent Unit (GRU)

A GRU model was developed as an alternative recurrent architecture with fewer parameters than LSTM.

5. ClinicalBERT (Frozen)

A pre-trained ClinicalBERT model was used for medical text classification while keeping the transformer layers frozen.

6. ClinicalBERT (Fine-Tuned)

The ClinicalBERT model was further fine-tuned on the medical dataset to improve predictive performance.

**Evaluation Metrics**

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Training Time

**Libraries and Tools**

The project was developed using:

- Python
- PyTorch
- NumPy
- Pandas
- Scikit-Learn
- Matplotlib
- Seaborn
- Hugging Face Transformers

**Results**

All models were trained and evaluated on the same dataset. Their performance was compared using standard classification metrics. The comparison helped determine which architecture produced the best balance between prediction accuracy and computational efficiency.

**Conclusion**

This project demonstrates the application of deep learning techniques in healthcare prediction tasks. By comparing DNN, LSTM, Bi-LSTM, GRU, and transformer-based models, valuable insights were obtained regarding their effectiveness in predicting patient survival outcomes.

Future improvements may include hyperparameter tuning, feature selection, ensemble learning, and testing on additional healthcare datasets.
