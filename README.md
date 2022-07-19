## Python Flask which has Tableau Public 
## ML integrated into one book using Flask as an API

Basic app for serving a Tableu Public Workbook + Serving ML as an API

Requirements list: Requirements.txt file has the all the packages you want plus more

## Directory Structure
app.py
templates
	-> home.html
	-> dashboards.html
	-> machinelearning.html
	-> js -> app.js

## Steps to deploy
Create a Python Environment if you do not have Python requirement files
And pip3 install requirements.txt if you do not have Python installed to already

## Steps that are used to set up ML algorithm
1) Use the TrainAndSaveModel.ipynb notebook to train the model
2) Currently it is using BMI dataset from Kaggle to predict whether they are:
https://www.kaggle.com/datasets/yersever/500-person-gender-height-weight-bodymassindex?resource=download
3) The TrainAndSaveModel uses Label Encoder to encode 'Male' and 'Female' to be 1 or 0 and MinMaxScaler for Height and Weight
4) It saves the RandomForestClassifier Model which is 88% accurate as a pickle file, saves Male and Female encoder as a pickle file, MinMaxScaler as a pickle file

## Steps to use Tableau Page
1) Update the app.js in js folder inside the templates/js/app.js with the links of your Public Tableau and you can use that to link it to your Tableau Public


## Guide to update the webpage
1) Open the webpage - Use Dashboards link to view Tableau page
2) Open the webpage - Use MachineLearning link to view Machine learning form






