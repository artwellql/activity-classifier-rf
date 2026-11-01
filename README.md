# Human Activity Recognition (HAR) using Accelerometer Data

**Overview**
This project classifies human physical activities (idle, running, walking, climbing stairs) using raw 3-axis smartphone accelerometer data. The main challenge was handling a highly imbalanced dataset and extracting temporal features to improve accuracy.

**Tech Stack**
* Python
* Pandas (Data processing and feature engineering)
* Scikit-Learn (Random Forest, Support Vector Machine)

**Methodology**
* **Feature Engineering:** Extracted basic statistical features (mean, standard deviation, min, max) for each axis to capture movement patterns.
* **Model Evaluation:** Trained and compared SVM and Random Forest classifiers.
* **Imbalance Handling:** Used Precision, Recall, and F1-score to evaluate how well the models handle minority classes.

**Key Results**
* The **Random Forest Classifier** achieved perfect overall accuracy (1.0) and handled the class imbalance effectively.
* For the minority class (`stairs`, only 165 samples), Random Forest perfectly classified it with an F1-score of 1.0, while SVM achieved an F1-score of 0.88.
* Adding min/max features alongside mean/std was critical for recognizing complex movements like stair-climbing.

**How to Run**
1. Clone this repository.
2. Make sure the `data` folder is in the root directory.
3. Install requirements: `pip install pandas scikit-learn`
4. Run the `sensor_activity_classification.ipynb` notebook.
