<h1>Cardivascular Risk Prediction - Classification</h1>

<p>In this notebook I have explored different Machine Learning Models for predicting whether a patient has 10-year risk of developing Coronary Heart Disease using the Farmingham Dataset </p>

<h2> Data Description</h2>
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 3,300 records and 15 attributes.

Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk
factors. </br>

* Sex: male or female("M" or "F")
* Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to
whole numbers, the concept of age is continuous)

Behavioral
* is_smoking: whether or not the patient is a current smoker ("YES" or "NO")
* Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be
considered continuous as one can have any number of cigarettes, even half a cigarette.)

Medical(history)
* BP Meds: whether or not the patient was on blood pressure medication (Nominal)
* Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)
* Prevalent Hyp: whether or not the patient was hypertensive (Nominal)
* Diabetes: whether or not the patient had diabetes (Nominal)

Medical(current)
* Tot Chol: total cholesterol level (Continuous)
* Sys BP: systolic blood pressure (Continuous)
* Dia BP: diastolic blood pressure (Continuous)
* BMI: Body Mass Index (Continuous)
* Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in
fact discrete, yet are considered continuous because of large number of possible values.)
* Glucose: glucose level (Continuous)

Predict variable (desired target)
* 10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”) - DV


<h2> Steps performed </h2>

1. Exploratory Data Analysis
2. Data preprocessing:
    * Handle Missing Values
    * Binning
    * Transformation
    * Scaling
3. Data resampling using SMOTE to treat class imbalance
4. Built 4 different machine learning models to predict TenYearCHD:
    *  Logistic Regression
    *  Random Forest Classification
    *  Decision Tree Classification
    *  Gradient Boosting Classification
5. Hyperparameter tuning for the models
6. Evaluated each model (Accuracy, Recall, ROC-AUC Score)
