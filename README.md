
# Predicting Diabetes Onset

## Overview

Diabetes is a chronic medical condition affecting millions worldwide. According to the Canadian government, nearly 3.8 million Canadians live with diagnosed diabetes, representing 9.8% of the population. The goal of this project is to create a predictive software tool that can help individuals assess their risk of diabetes early, enabling timely consultation with healthcare professionals.

This project leverages the Pima Indians Diabetes Dataset and machine learning algorithms to create an easy-to-use interface that can predict the likelihood of diabetes onset based on key health indicators.

---

## Team

- **Ashfi Hasnain**
- **Abhinav Mishra**
- **Lakehead University**

---

## Development Stack

- **Programming Language**: Python
- **Platform**: Google Colab
- **ML Libraries**: Scikit-learn, Pandas, Matplotlib, Seaborn
- **Interface**: Graphical User Interface (via Colab Widgets)

---

## Dataset

- **Source**: Pima Indians Diabetes Dataset (National Institute of Diabetes and Digestive and Kidney Diseases)
- **Attributes**:
  1. Pregnancies
  2. Glucose
  3. Blood Pressure
  4. Skin Thickness
  5. Insulin
  6. Body Mass Index (BMI)
  7. Diabetes Pedigree Function
  8. Age
- **Size**: 768 records
- **Target**: Binary outcome (Diabetic or Non-Diabetic)

---

## Data Preprocessing

- Missing data replaced with column-wise averages.
- No duplicate entries found.
- Outlier detection performed using box plots.
- Data distribution analyzed using histograms.
- Correlation matrix generated using Pearson’s coefficient.

---

## Machine Learning Model

### Preparation

- Features (`X`) and target (`Y`) separated.
- Train-test split (80/20) with `random_state=42`.
- Standardization performed using `StandardScaler`.

### Models Tested

- Logistic Regression
- K-Nearest Neighbors
- Support Vector Machines
- Decision Tree
- Random Forest
- Gradient Boosting

### Evaluation

- Accuracy measured for each model.
- **Random Forest** achieved highest predictive accuracy.
- Final model serialized using `joblib`.

---

## GUI (Graphical User Interface)

- Built using Colab interface elements.
- Users input values for 8 health features.
- On clicking "Predict", system displays risk status.
- Example Input: `[0, 85, 82, 18.7, 91, 19.4, 0.9, 20]` → Prediction: **Not Diabetic**

---

## Challenges Encountered

- File sharing issues in Google Colab between users.
- GUI limitations in Colab – cannot open in separate window.
- Dataset limited to Pima Indian population.

---

## Future Improvements

1. Use a more ethnically diverse dataset.
2. Develop a standalone desktop/mobile application.
3. Integrate medical expert validation for clinical relevance.

---

## Conclusion

This project integrates data analysis, machine learning, and a simple user interface to offer a predictive tool for assessing diabetes risk. It showcases the power of Python for health informatics applications and encourages further development to improve public health outcomes.

---

## Citations

Sources include:
- Canadian Diabetes Association
- Cleveland Clinic
- Mayo Clinic
- Public Health Agency of Canada
- NIH, WHO, Kaggle, SimpliLearn

For full references, see the original project documentation.

---

*This README provides a comprehensive overview of the Predicting Diabetes Onset project, including motivation, technical implementation, evaluation, and potential for real-world use.*
