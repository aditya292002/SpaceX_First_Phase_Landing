# Predicting the Success of Falcon 9 Rocket Landing
### Overview
The goal of this project is to predict whether or not the first stage of SpaceX's Falcon 9 rocket will successfully land after launch. As a competitor to SpaceX, we want to be able to bid against them for rocket launches, and understanding the likelihood of success for each launch is a crucial factor in determining our bid price.

To achieve this goal, we have gathered data on previous Falcon 9 launches and landing attempts, including various features such as launch date, launch site, and weather conditions. We have used this data to build and train several machine learning models, and have evaluated their performance using cross-validation techniques.

### Data
The data used in this project was obtained through a combination of web scraping and API calls. We used various sources, including SpaceX's official website and NASA's launch database, to gather information on Falcon 9 launches and landing attempts. The data includes both successful and unsuccessful landing attempts, and spans a period of several years.

### Models
We experimented with several machine learning algorithms to predict the success of Falcon 9 landings, including logistic regression, decision trees, and random forests. We also tried various feature engineering techniques, such as adding interaction terms and creating polynomial features.

### Results
Our best-performing model achieved an accuracy of 85% on a held-out test set. We believe this level of accuracy is sufficient to make informed bidding decisions for rocket launches.

### Repository Structure
- **data/:** contains the raw data used in the project.
- **notebooks/:** contains Jupyter notebooks with exploratory data analysis, data cleaning and feature engineering, and model training and evaluation.
- **src/:** contains the Python scripts used to scrape data and preprocess it for modeling.
- **models/:** contains pickled trained models.
- **requirements.txt:** lists the required Python packages for running the code.


### Usage
To replicate our results, you can follow these steps:

Clone this repository to your local machine.
Install the required packages by running pip install -r requirements.txt.
Run the notebooks in the notebooks/ directory in the following order:
01_data_collection.ipynb: scrapes and preprocesses the raw data.
02_exploratory_data_analysis.ipynb: explores the data and visualizes its distributions.
03_feature_engineering.ipynb: creates new features and preprocesses the data for modeling.
04_model_training.ipynb: trains and evaluates several machine learning models.
The final selected model will be saved in the models/ directory.


### Future Work
In the future, we plan to incorporate additional data sources, such as weather forecasts and satellite imagery, to improve the accuracy of our predictions. We also plan to explore more advanced modeling techniques, such as neural networks and gradient boosting.



