# airbnb-kaggle
Airbnb Kaggle

iPython (Jupyter) notebooks file for featuring engineering, modeling and prediction for the Kaggle's Airbnb destination prediction competition (https://www.kaggle.com/c/airbnb-recruiting-new-user-bookings) <br/>

### Summary of files:
1. Airbnb-user-explore.ipynb: User data exploratory analysis
2. Airbnb-session-explore.ipynb: User's sessions data exploratory analysis and data preparation for merging with user data
3. Airbnb-destination-prediction-main.ipynb: 'Main file' for features engineering, modeling and generating prediction file
4. Airbnb-destination-prediction-visualization.ipynb: similar to feature-engineering-and-prediction file but adding visualization along in the notebook file

### Methodology:
#### Feature selection and feature engineering:
- User's demographics e.g. age and gender
- Gender imputation using K-nearest neighborhood based on other user's features
- Age imputation with default -1
- Session time spent for each Action (action_detail) by user (from the session file)
- Date feature extraction such as day of week, month, and year from user's account creation and user's first active, and the number of days account created after first active
- Other features from user's file e.g. browser type, signup flow, device type, language

#### Model:
- XGboost classifier
- Top five predicted destination are taken from the five highest probability prediction from the model

