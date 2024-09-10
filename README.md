
## Placement Prediction Web App

## Project Overview

This project is a web application designed to predict student placement outcomes using a machine learning model. The application is built using Flask for the backend and HTML/CSS for the frontend. A Random Forest classifier is utilized to make predictions based on student data.

## Features

- User-friendly web interface for inputting student data.
- Backend server built with Flask to handle requests and predictions.
- Random Forest classifier model to predict placement outcomes.
- Responsive design using HTML and CSS.

## Installation

Follow these steps to set up the project on your local machine.

### Prerequisites

- Flask
- numpy
- joblib
- Pandas
- matplotlib
- scikit-learn==1.2.2
- gunicorn
- seaborn

### Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/pragmaticdev798/decisiontreesclassifier.git
    cd decisiontreeclassifier

    ```

2. **Create a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Run the application:**

    ```bash
    python app.py
    ```

    The web app should now be running on `http://127.0.0.1:5000/`.

## Usage

1. **Home Page:**

    Enter the required student information into the form provided on the home page.

2. **Submit:**

    Click the "Predict placement" button to make a prediction. The result will display whether the student is likely to be placed or not.

## Project Structure

- **app.py**: The main Flask application file.
- **model.py**: Script to train and save the Random Forest model.
- **templates/**: Directory containing HTML templates.
    - **index.html**: The main page where users input data.
    
- **static/**: Directory containing static files like CSS.
    - **mystyle.css**: The CSS file for styling the web pages.
- **requirements.txt**: List of required Python packages.

## Model Training

The model is trained using a dataset of student information from kaggle. The features used for training include academic scores, extracurricular activities, and other relevant data points. The Random Forest classifier is chosen for its robustness and accuracy in handling classification problems.


working link:-  https://drive.google.com/file/d/1Kvc3oQQE1YNPPATWCaJRiGdDkUKpZdjF/view?usp=sharing


How Does it Work? <br> 
<br>
Decision Trees: At its core, a Random Forest is made up of many decision trees. A decision tree is like a flowchart where each decision leads to a new question until we get a final answer (e.g., pass or fail).

Random Sampling: To build these decision trees, the Random Forest algorithm uses random samples of the data. It picks a random subset of students, a random subset of study habits, attendance records, etc. This ensures that each tree is a little different.

Making Predictions: When we want to predict whether a new student will pass or fail, each decision tree in the forest makes its own prediction. Then, the Random Forest combines all these predictions to make a final decision. Usually, it takes a majority vote: if most trees say "pass," the forest says "pass."








 


  

