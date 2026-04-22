# 📈 Project Summary: Student Academic Success Prediction

This project aims to predict student outcomes (**Dropout, Graduate, or Enrolled**) based on a comprehensive set of demographic, socio-economic, and academic performance data.

---

## 1. Data Foundation
The project utilizes a dataset containing **4,424 records** and **37 features**[cite: 5]. These features cover multiple dimensions of a student's life and academic journey:

*   **Demographics:** Marital status, nationality, gender, and age at enrollment[cite: 5].
*   **Socio-economic Factors:** Parents' qualifications and occupations, unemployment rate, inflation rate, and GDP[cite: 5].
*   **Academic History:** Previous qualifications, admission grade, application mode, and course of choice[cite: 5].
*   **Performance Metrics:** Detailed tracking of curricular units for both the 1st and 2nd semesters, including units enrolled, approved, and grades[cite: 4, 5].

---

## 2. Exploratory Data Analysis (EDA)
Initial visualizations reveal the distribution of the **Target** variable[cite: 6]:

*   The dataset is somewhat imbalanced: **"Graduate"** is the most frequent outcome, followed by **"Dropout"**, while **"Enrolled"** represents the smallest group[cite: 6].
*   **Correlation Analysis:** A heatmap analysis indicates strong correlations between semester-specific academic performance (e.g., units approved) and the final target outcome[cite: 7].

---

## 3. Methodology & Technical Stack
The project is built using standard data science libraries:

*   **Data Handling:** `pandas` and `numpy`[cite: 3].
*   **Visualization:** `matplotlib` and `seaborn`[cite: 3].
*   **Modeling Strategy:**
    *   **Pre-processing:** Uses `StandardScaler` for feature normalization and `LabelEncoder` for target labels[cite: 3].
    *   **Algorithms:** Implementation focuses on **K-Nearest Neighbors (KNN)** and **Random Forest Classifier**[cite: 3].
    *   **Optimization:** Employs `GridSearchCV` for hyperparameter tuning and `train_test_split` for model validation[cite: 3].

---

## 4. Key Technical Note
A critical detail identified in the source code is the data format: the `data.csv` file uses a **semicolon (`;`)** as a separator rather than a standard comma[cite: 4]. This is vital for correct data ingestion and subsequent analysis.
