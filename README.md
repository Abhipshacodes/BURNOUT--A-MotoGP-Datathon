# BURNOUT--A-MotoGP-Datathon
Burnout is a MotoGP datathon where we predict lap times using machine learning. I explored features like tire strategy, weather, and track to train my model. My final model achieved a MAE close to 10.29—tuned, tested, and ready to race! 

This project was developed as part of a Kaggle competition where the task was to predict MotoGP lap times using various race and rider attributes.

## 📂 Repository Structure

- `YourTeamName_output.csv`: Final submission file with predicted lap times.
- `solution.csv`: Intermediate prediction output.
- `README.md`: Project overview and methodology.

---

## 📎 Kaggle Notebook

👉 [Click here to view the  Notebook](https://colab.research.google.com/drive/11JF2cWmPaN_wzSeAw9ZP2G-u2KCdFYXj)

---

## 🧠 Problem Statement

Predict the `Lap_Time_Seconds` for each rider in the test dataset using features such as tire strategy, circuit length, weather, grid position, etc.

---

## 📊 Dataset Files Used

- `train.csv`: Historical lap time data with features and targets.
- `val.csv`: Separate validation set for MAE performance monitoring.
- `test.csv`: Unlabeled data to predict `Lap_Time_Seconds`.
- `sample_submission.csv`: Provided submission format.

---

## 🛠️ Tools & Technologies

- **Python 3**
- **Pandas** for data processing
- **Scikit-learn** for preprocessing and evaluation
- **XGBoost**, **LightGBM**, and **CatBoost** for model experimentation
- **Label Encoding** for categorical variables
- **Mean Absolute Error (MAE)** as the evaluation metric

---

## 🧪 Workflow Summary

1. **Data Preprocessing**:
   - Combined and cleaned `train`, `val`, and `test` datasets.
   - Handled missing values and categorical feature inconsistencies.
   - Encoded categorical variables using LabelEncoder.

2. **Feature Engineering**:
   - Created additional features like `Tire_Degradation`, `Pit_Stop_Impact`, etc.
   - Aligned features between train and test sets.

3. **Model Training**:
   - Experimented with multiple models (XGBoost, CatBoost, LightGBM).
   - Tuned hyperparameters and monitored MAE.
   - Used early stopping to avoid overfitting.

4. **Final Submission**:
   - Best model's predictions saved as `YourTeamName_output.csv`.

---

## 🏆 Final MAE Score

- **Validation MAE:** ~5.51  
- **Kaggle Public Score:** ~10.29 *(initial)* 

---



