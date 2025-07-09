# Heart Disease Prediction App

This project is a web application for predicting the likelihood of heart disease based on user-provided health information. The app uses a machine learning model trained on a heart disease dataset and provides an easy-to-use interface for making predictions.

## Features
- User-friendly web interface built with Streamlit
- Predicts the risk of heart disease using a trained KNN model
- Input fields for all relevant health parameters
- Real-time feedback on prediction results

## Dataset
The model was trained on a heart disease dataset with the following features:
- Age
- Sex
- ChestPainType
- RestingBP
- Cholesterol
- FastingBS
- RestingECG
- MaxHR
- ExerciseAngina
- Oldpeak
- ST_Slope
- HeartDisease (target)

## Files
- `app.py`: Streamlit web application for prediction
- `heart_disease_EDA.ipynb`: Exploratory Data Analysis notebook
- `knn_heart_model.pkl`: Trained KNN model
- `heart_scaler.pkl`: Scaler used for preprocessing
- `heart_columns.pkl`: List of expected input columns for the model
- `heart.csv`: (Not included here) The original dataset used for training

## Setup Instructions
1. **Clone the repository or copy the files to your local machine.**
2. **Install the required Python packages:**
   ```bash
   pip install streamlit pandas scikit-learn joblib
   ```
3. **Ensure the following files are present in the project directory:**
   - `app.py`
   - `knn_heart_model.pkl`
   - `heart_scaler.pkl`
   - `heart_columns.pkl`

## Running the App
To start the web application, run:
```bash
streamlit run app.py
```
This will open the Heart Disease Prediction App in your web browser.

## Usage
1. Enter your health information in the provided fields.
2. Click the **Predict** button.
3. The app will display whether you are likely to have heart disease based on the model's prediction.

## Notes
- The app uses one-hot encoding and scaling consistent with the training data.
- The model and preprocessing files must match the training pipeline.
- This tool is for educational and informational purposes only. For medical advice, consult a healthcare professional.

## License
This project is provided for educational purposes.
