# **Calorie Burn Prediction System (BurnMeter)**

## **Overview**
This project aims to develop an AI-based system to accurately predict the calories burned during various exercises and provide personalized recommendations for improving fitness and health. By leveraging individual user data and the XGBoost machine learning model, the system overcomes the limitations of generalized calorie-tracking tools, offering tailored insights to users.

---

## **Features**
1. **Accurate Calorie Burn Prediction**: Predicts calories burned during exercises using personalized user data.
2. **Personalized Recommendations**: Suggests tailored fitness routines and goals based on user profiles.
3. **Data Insights**: Provides detailed visualizations of calorie burn patterns and relationships between exercise metrics.

---

## **Data Description**
The project uses two datasets:
1. **Exercise Data (`exercise.csv`)**:
   - `User_ID`: Unique identifier for each user.
   - `Gender`: Gender of the user (male/female).
   - `Age`: Age of the user (in years).
   - `Height`: Height of the user (in cm).
   - `Weight`: Weight of the user (in kg).
   - `Duration`: Exercise duration (in minutes).
   - `Heart_Rate`: Average heart rate during exercise (bpm).
   - `Body_Temp`: Average body temperature during exercise (\u00b0C).

2. **Calories Data (`calories.csv`)**:
   - `User_ID`: Unique identifier (matches `User_ID` in `exercise.csv`).
   - `Calories`: Total calories burned.

---

## **Methodology**
1. **Data Preprocessing**:
   - Merged datasets using `User_ID`.
   - Cleaned and normalized data to handle inconsistencies.
2. **Feature Engineering**:
   - Analyzed correlations between exercise metrics and calories burned.
   - Converted categorical data (e.g., gender) into numerical values.
3. **Model Development**:
   - Used the **XGBoost Regressor** to train a model on the processed data.
   - Evaluated the model's performance using metrics such as Mean Absolute Error (MAE).
4. **Personalized Insights**:
   - Used model predictions to provide individualized exercise recommendations.

---

## **Technologies Used**
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost
- **Tools**: Jupyter Notebook

---

## **Usage**
1. **Setup**:
   - Install required Python libraries using:
     ```bash
     pip install pandas numpy scikit-learn matplotlib seaborn xgboost
     ```
   - Clone the repository and navigate to the project directory.

2. **Run the Notebook**:
   - Open the provided Jupyter Notebook (`BurnMeter.ipynb`).
   - Load and preprocess the data.
   - Train and evaluate the machine learning model.

3. **Generate Predictions**:
   - Use the trained model to predict calories burned for new user profiles.

---

## **Results**
- The XGBoost model achieved reliable accuracy in calorie burn predictions.
- Highlighted significant relationships between exercise metrics and calories burned through visualizations.
- Demonstrated personalized fitness insights for different user profiles.

---

## **Future Enhancements**
1. Expand the dataset with more diverse user profiles and exercise types.
2. Incorporate additional features such as dietary habits and stress levels.
3. Develop a mobile or web application for real-time calorie tracking and recommendations.

---

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for details.

