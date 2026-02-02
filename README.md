# BrickMetrics-A-Data-Driven-Machine-Learning-Approach-to-Real-Estate-Price-Prediction
This project is a full stack machine learning web application that predicts house prices based on user inputs such as location, square footage, number of bedrooms (BHK), and bathrooms. It combines frontend development, backend API integration, and machine learning into a complete end-to-end solution.
The machine learning model was built using the Bengaluru House Data dataset. The workflow includes data cleaning, handling missing values, feature engineering, outlier detection and removal, and one-hot encoding of categorical features such as location. After preprocessing, a Linear Regression model was trained and evaluated using Scikit-learn. The final trained model was exported as a .pickle file, along with a columns.json file to store feature metadata for prediction consistency.
The frontend is developed using HTML, CSS, and JavaScript, providing a simple and interactive interface where users can enter property details. When the user submits the form, the data is sent to the Flask backend through an HTTP request. The Flask server loads the trained model, processes the input data, and returns the predicted price as a JSON response. The frontend dynamically displays the predicted house price without refreshing the page
## Project Overview
  - Data cleaning and preprocessing
  - Feature engineering
  - Handling missing values
  - Outlier detection and removal
  - One-hot encoding for location
  - Model training using Linear Regression
  - Model evaluation and testing
  - Exporting the trained model as a .pickle file
  - Exporting column metadata as a columns.json file
## How It Works
 1. User enters:
    - Location
    - Total square feet
    - Number of BHK
    - Number of bathrooms
  2. Frontend sends data to Flask backend via HTTP request.
  3. Flask: Loads the trained pickle model,Processes input data,Returns predicted house price
  4. Frontend displays the predicted price dynamically.
## Tech Stack
Frontend: HTML,CSS,JavaScript
Backend: Python, Flask
Machine Learning & Data Processing: Pandas, Numpy,Matplotlib,Scikit-learn,Pickle,JSON
## Project Structure

├── model/
│   ├── bangalore_home_prices_model.pickle
│   └── columns.json
├── server.py (Flask backend)
├── templates/
│   └── index.html
├── static/
│   ├── style.css
│   └── script.js
├── Project1.ipynb (Model training notebook)
└── README.md
