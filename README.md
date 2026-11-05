# Human Activity Recognition (HAR)

##  Description
This project focuses on classifying human physical activities—idle, running, walking, and climbing stairs—based on raw 3-axis smartphone accelerometer data. The dataset exhibits a significant class imbalance, providing a realistic challenge for predictive modeling. The project demonstrates feature engineering from raw sensor data and compares the performance of different classification algorithms.

##  Technologies
- **Language:** Python
- **Data Manipulation:** Pandas
- **Machine Learning:** Scikit-learn (SVM, Random Forest, StandardScaler)
- **Environment:** Google Colab

##  Functionality
- **Feature Engineering:** Extracts key statistical features (mean, standard deviation, min, and max) from raw X, Y, and Z accelerometer signals to capture movement patterns effectively.
- **Data Preprocessing:** Handles data scaling using `StandardScaler` to ensure optimal model performance.
- **Model Training:** Trains two robust classifiers: Support Vector Machine (SVM) with an RBF kernel and a Random Forest Classifier.
- **Model Evaluation:** Compares model performance using metrics like Precision, Recall, and F1-score, with a specific focus on handling the dataset's inherent class imbalance.
- **Imbalance Handling Analysis:** Evaluates model robustness on minority classes (e.g., stairs), where Random Forest demonstrated superior performance over SVM.
