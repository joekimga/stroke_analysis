# Stroke Analysis

Background: According to the CDC (https://www.cdc.gov/stroke/facts.htm), 1 in 6 cardiovascular disease related deaths are due to stroke. Someone dies of stroke every 4 minutes, and billions are spent on health care costs related to stroke each year.

This Dashboard shows the Stroke Mortality Rate by Race/Ethnicity and Gender.
![image](https://user-images.githubusercontent.com/28760237/123574445-d64add80-d79d-11eb-98f4-8667b3a982b3.png)
<img src="https://user-images.githubusercontent.com/28760237/123574445-d64add80-d79d-11eb-98f4-8667b3a982b3.png" width=75% height=75%>

Our goal was to create a machine learning model that would predict the likelihood of stroke based on a given set of parameters, including known risk factors. We used the stroke prediction dataset from Kaggle (https://www.kaggle.com/fedesoriano/stroke-prediction-dataset) to examine possible models. Using pandas in jupyter notebooks, we evaluated the following models: KNN, Random Forest, Logistic Regression, SVM, Decision Tree, Gaussian Naive Bayes, Neural Networks, and Gradient Boosting. Jupyter notebooks for each model can be referenced, as the names of the model correspond with what was examined inside of the notebook. We ultimately selected the Gaussian Naive Bayes model as our best performing model (GaussianNaiveBayes_FinalModel.ipynb).

The Dashboard below shows a comparison of Stroke and Non-Stroke Population Social Factors.
![image](https://user-images.githubusercontent.com/28760237/123574526-01cdc800-d79e-11eb-9784-5c03803a7c80.png)
<img src="https://user-images.githubusercontent.com/28760237/123574526-01cdc800-d79e-11eb-9784-5c03803a7c80.png" width=75% height=75%>

![image](https://user-images.githubusercontent.com/28760237/123574718-6426c880-d79e-11eb-9495-a048d0b7abcc.png)
<img src="https://user-images.githubusercontent.com/28760237/123574718-6426c880-d79e-11eb-9495-a048d0b7abcc.png" width=75% height=75%>

![image](https://user-images.githubusercontent.com/28760237/123574800-86b8e180-d79e-11eb-887a-764652d2eb72.png)


![image](https://user-images.githubusercontent.com/28760237/123574850-9801ee00-d79e-11eb-8320-46502d5f9f03.png)


![image](https://user-images.githubusercontent.com/28760237/123574905-af40db80-d79e-11eb-8cad-64a806225684.png)


A tableau dashboard with a predictive questionnaire was created based on our dataset and model (StrokePrediction.twbx). This connects to our Gaussian Naive Bayes Final Model jupyter notebook via a Tabpy server.


Instructions:

  1. Start Tabpy server(Use the command pip install tabpy-server in the command prompt to install the Tabpy and then type Tabpy to start the server)
  2. Start Jupyter notebook and run the GaussianNaiveBayes_FinalModel.ipynb, which is the jupyter notebook with the final model.
  3. Open up the Tableau workbook in Tableau Desktop and navigate to
Help --> Setting and Performance ---> Manage External Service Conenction Type in the server as localhost and and port as 9004 and that is it, Tabpy is configured and you should able to run the predictive questionnaire dashboard
