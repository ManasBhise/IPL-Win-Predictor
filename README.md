# IPL-Win-Predictor
![IPL Picture](IPL%20Picture.jpg)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Streamlit](https://img.shields.io/badge/streamlit-%23FF4B4B.svg?style=for-the-badge&logo=streamlit&logoColor=white)
![Pickle](https://img.shields.io/badge/pickle-898989?style=for-the-badge&logo=python&logoColor=white)

## Project Overview

The core of this project involves:

1.  **Data Preprocessing:**
    * Combining match and delivery data from CSV files.
    * Calculating relevant features like runs left, balls left, current run rate (CRR), required run rate (RRR), and wickets in hand.
    * Handling missing values and data cleaning.
2.  **Model Training:**
    * Using a Logistic to predict the outcome of the match (win/loss).
    * Splitting the data into training and testing sets.
    * Scaling the features using StandardScaler.
    * Saving the trained model and scaler using pickle.
3.  **Win Probability Prediction:**
    * Creating a function to predict win probability for any given match scenario.
    * Developing a Streamlit web application for user-friendly interaction.
4.  **Streamlit Application:**
    * A simple web interface allowing users to input match details (batting team, bowling team, target score, current score, overs completed, wickets out).
    * Displaying the predicted win probabilities for both teams.

## Model Accuracy

The Logistic Regression achieved an accuracy of approximately 31% on the test dataset. Please refer to the `app.py` or the original training script for the exact accuracy value, as it can vary slightly between runs due to the random nature of the model.

## Files

* `matches.csv`: Contains match-level information.
* `deliveries.csv`: Contains ball-by-ball delivery information.
* `ipl_prediction_model.pkl`: Serialized Random Forest Classifier model.
* `ipl_scaler.pkl`: Serialized StandardScaler.
* `app.py`: Streamlit application code.
* `ipl_win_probability_prediction.ipynb`(optional): Jupyter notebook used for data exploration and model training.
* `README.md`: Project description and instructions.

## How to Run

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/ManasBhise/IPL-Win-Predictor]
    cd [repository directory]
    ```

2.  **Install dependencies:**

    ```bash
    pip install pandas numpy scikit-learn streamlit
    ```

3.  **Run the Streamlit app:**

    ```bash
    streamlit run app.py
    ```

4.  Open your web browser and navigate to the URL displayed in the terminal.

## Usage

1.  Select the batting and bowling teams from the dropdown menus.
2.  Enter the target score, current score, overs completed, and wickets out.
3.  Click the "Predict Probability" button.
4.  The win probabilities for both teams will be displayed.

## Future Improvements

* Incorporate venue information for better predictions.
* Add more features, such as player statistics and recent form.
* Explore other machine learning models for improved accuracy.
* Create a more visually appealing and informative Streamlit app.
* Add more features to the Streamlit app, such as graphs showing the progression of win probability.
* Make the model able to handle more recent data.

## Author

Manas Vijay Bhise

Created - 27 feb 2025
