
# Machine Learning(CICD Pipline) - Student Performance Prediction

This project end-to-end machine learning project that predicts student math scores based on demographic and academic-related features. The project follows a modular ML pipeline architecture with data ingestion, preprocessing, model training, evaluation, and prediction components.


## Data Workflow
1. Data Ingestion  
   - Load dataset
   - Split into training and testing data

2. Data Transformation  
   - Handle missing values
   - Encode categorical features
   - Scale numerical features

3. Model Training  
   - Train multiple regression models
   - Perform hyperparameter tuning using GridSearchCV
   - Select the best model based on R² score

4. Model Saving  
   - Save trained model and preprocessing pipeline using pickle/dill

5. Prediction Pipeline  
   - Load saved model and preprocessor
   - Transform user input
   - Generate predictions

6. Flask Web Application  
   - User enters student data
   - Application sends data to prediction pipeline
   - Predicted math score is displayed


## Documentation

This project predicts a student's **math score** based on input features such as:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

It demonstrates a production-ready machine learning system with modular design and deployment using Flask.

---

## Project Architecture

##### Raw Data (CSV)
   ###### ↓
##### Data Ingestion
   ###### ↓
##### Train/Test Split
   ###### ↓
##### Data Transformation (Encoding + Scaling)
   ###### ↓
##### Model Training (GridSearchCV)
   ###### ↓
##### Model Evaluation (R² Score)
   ###### ↓
##### Best Model Selection
   ###### ↓
##### Model Serialization (Pickle/Dill)
   ###### ↓
##### Flask Web App (Prediction API) 
## Tech Stack

- Python
- Flask
- Scikit-learn
- Pandas
- NumPy
- XGBoost
- CatBoost
- HTML/CSS
- Pickle / Dill
- Github
# Future Improvements
- Deploy on AWS / Render / Azure
- Add REST API (FastAPI)
- Improve UI with Bootstrap/Tailwind
- Add database integration
- Docker containerization
- CI/CD pipeline with GitHub Actions

# Flask Web Application
Workflow:
User enters student data
Flask receives form input
Data converted using CustomData
Prediction pipeline runs
Result displayed on UI

Routes:
/ → Home page
/predict_datapoint → Prediction form
## Acknowledgements

 - [Youtube Channel - Krish Naik - End to End Data Science Playlist](https://www.youtube.com/watch?v=S_F_c9e2bz4&list=PLZoTAELRMXVPS-dOaVbAux22vzqdgoGhG)
 - [stud.csv - dataset](https://github.com/krishnaik06/mlproject/blob/main/notebook/data/stud.csv)


