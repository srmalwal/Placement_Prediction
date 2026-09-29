# Student Placement Predictor

A machine learning application that predicts whether a student is likely to be placed based on academic performance and other student-related attributes.

The project includes a trained machine learning model, a student placement dataset, a Jupyter Notebook for model development, and a web application for making predictions.

## Overview

Student placement prediction uses historical student information to estimate placement outcomes.

The system takes relevant student attributes as input and predicts the student's placement status.

The project follows an end-to-end machine learning workflow:

```text
Student Dataset
       ↓
Data Preprocessing
       ↓
Feature Selection
       ↓
Train/Test Split
       ↓
Machine Learning Model
       ↓
Model Evaluation
       ↓
Save Trained Model
       ↓
Web Application
       ↓
Student Input
       ↓
Placement Prediction
       ↓
Prediction History
```

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook
- Flask
- HTML/CSS
- Pickle
- CSV

## Dataset

The project uses:

```text
students_placement.csv
```

The dataset contains student-related information used to train the placement prediction model.

The target variable represents the student's placement outcome.

## Machine Learning

The model is trained using the student placement dataset.

The training and experimentation process is available in:

```text
student-placement-predictor.ipynb
```

The trained model is saved as:

```text
model.pkl
```

The saved model is loaded by the web application to make predictions without retraining the model every time.

## Model Workflow

```text
Input Student Data
        ↓
Data Preprocessing
        ↓
Feature Transformation
        ↓
Trained ML Model
        ↓
Placement Prediction
```

## Web Application

The project includes a web application implemented using **Flask**.

The application allows users to enter student information and obtain a placement prediction.

After submitting the form, the application:

1. Collects the student's input.
2. Preprocesses the input.
3. Loads the trained machine learning model.
4. Generates a prediction.
5. Displays the prediction to the user.
6. Stores the prediction in the prediction history.

## Prediction History

Previous predictions are stored in:

```text
prediction_history.csv
```

This allows the application to maintain a record of predictions made through the web interface.

## Project Structure

```text
Student-Placement-Predictor/
│
├── app.py
├── students_placement.csv
├── student-placement-predictor.ipynb
├── model.pkl
├── prediction_history.csv
└── README.md
```

## Installation

Install the required Python libraries:

```bash
pip install pandas numpy scikit-learn flask
```

If Jupyter Notebook is required:

```bash
pip install notebook
```

## Running the Application

Make sure the following files are present in the project directory:

```text
app.py
model.pkl
prediction_history.csv
```

Run the Flask application:

```bash
python app.py
```

The application will start a local web server. Open the URL displayed in the terminal in a web browser.

## How to Use

1. Start the Flask application.
2. Open the application in a browser.
3. Enter the required student information.
4. Submit the form.
5. The trained model generates the placement prediction.
6. The result is displayed on the web page.
7. The prediction is recorded in `prediction_history.csv`.

## Model Development

The complete model development process is documented in:

```text
student-placement-predictor.ipynb
```

The notebook contains the data preparation, model training, evaluation, and related experimentation used to develop the predictor.

## Files

| File | Purpose |
|---|---|
| `app.py` | Flask web application |
| `students_placement.csv` | Student placement dataset |
| `student-placement-predictor.ipynb` | Model development and training notebook |
| `model.pkl` | Trained machine learning model |
| `prediction_history.csv` | Stored prediction records |
| `README.md` | Project documentation |

## Future Improvements

- Compare multiple machine learning algorithms.
- Improve model performance through hyperparameter tuning.
- Add prediction probability or confidence.
- Add data visualizations to the web application.
- Add an admin dashboard for prediction history.
- Improve the user interface.
- Deploy the application online.
- Add input validation and error handling.

## Conclusion

The Student Placement Predictor demonstrates an end-to-end machine learning application, from dataset preparation and model training to deployment through a Flask web application.

The system provides a simple interface for entering student information and obtaining a machine learning-based placement prediction while maintaining a history of previous predictions.
