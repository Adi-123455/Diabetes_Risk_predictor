
**Diabetes Risk Predictor**
This project develops a machine learning model to predict the likelihood of diabetes based on several diagnostic measurements, and then deploys it as an interactive web application using Gradio.

**Project Steps**
The notebook follows these key steps:

**Import Libraries**:
Essential libraries like pandas, numpy, matplotlib, seaborn, scikit-learn, and gradio are imported.
Load Dataset: The Pima Indians Diabetes Database is loaded from a public URL into a pandas DataFrame.
Basic Info: Displaying the first few rows, checking the shape, and identifying any missing values in the dataset.
Data Visualization: A correlation heatmap is generated to understand the relationships between features.
Split Data: The dataset is split into training and testing sets for model development and evaluation.
Scale Features: Features are scaled using StandardScaler to normalize the input data for better model performance.
Train Model: A Logistic Regression model is trained on the scaled training data.
Evaluate Model: The model's performance is evaluated using accuracy score, a confusion matrix, and a classification report on the test set.
Build Gradio App: A Python function predict_diabetes is created to take user inputs, scale them, and provide a prediction using the trained model.
Launch Gradio Interface: An interactive web interface is launched using Gradio, allowing users to input various health parameters and get an immediate diabetes risk prediction.
How to Use the Gradio Application
Once the Gradio application is launched, you will see an interface with several sliders. Each slider corresponds to a health parameter:

Pregnancies: Number of times pregnant.
Glucose Level: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.
Blood Pressure: Diastolic blood pressure (mm Hg).
Skin Thickness: Triceps skin fold thickness (mm).
Insulin: 2-Hour serum insulin (mu U/ml).
BMI: Body mass index (weight in kg/(height in m)^2).
Diabetes Pedigree Function: A function which scores likelihood of diabetes based on family history.
Age: Age in years.
Adjust the sliders to input the desired values for each parameter. After making your selections, the application will display a prediction indicating whether the person is likely to have diabetes, along with a confidence percentage.

**Example**
To test the application, you can try inputting different combinations of values to see how the prediction changes. For instance, increasing glucose levels and BMI might increase the likelihood of a diabetes prediction.
