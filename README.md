# car price prediction
car price predictor predicts the selling price of the used car.

## URL
Run this App [HERE](https://carprice--predic.herokuapp.com)

Created By
----------
Sri hari K V
https://bit.ly/34R7lrj

## Dataset
Thanks to Kaggle
You can find dataset [HERE](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho)

## installation
one can install required packages for this application using 
```bash
pip install -r requirements
```
## Separate environment
Alwas create a separate `conda environment/any environment` so that you can avoid version errors between packages

## usage
After installing the required packages use the following command to start the flask app
```bash
python app.py
```

## folder structure
```bash
'
.
├── templates                                           #contains required HTML files
    ├── index.html 
├── Procfile                                            #file for Heroku deployment
├── README.md
├── car data.csv                                        #dataset
├── random_forest_regression_model.pkl.ipynb            #File which generated all pkl files
├── requirements.txt
└── app.py                                              #web server gateway Interface
```

## Important Tools used
* python 3.7
* anaconda-jupyternotebook
* conda environment
* flask
* html

## Steps for training models
* cleaning the data - `totalcharges` from object to float
* Check for `Null` values (no null values)
* Remove carname column - uniques values
* converting the year to no of yrs
* Encoding all the labels in data using `sklearn.preprocessing-LabelEncoder`
* Visualise `correlation` between each variable and target(churn)
* Check `Multicollinearity`
* split into `train and test` data - `0.8:0.2`
* Tune hyperparameter 
* Fitting models

## Model used
 Random Forest

## Performance
MAE: 0.8849978021977988
MSE: 3.9544237722813156
RMSE: 1.9885733007061408

## Input 
Fill the Information about car required by model in web app's UI

## Output
It will say the price of car with which it can be sold

## Deployment
This Application is Deployed in Heroku Platform. 
To Run this App [CLICK HERE](https://carprice--predic.herokuapp.com)
