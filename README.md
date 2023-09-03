# Predicting the Success of Falcon 9 Rocket Landing
### Overview

Space X advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because Space X can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against space X for a rocket launch.   In this lab, you will create a machine learning pipeline  to predict if the first stage will land given the data from the preceding labs.

The goal of this project is to predict whether or not the first stage of SpaceX's Falcon 9 rocket will successfully land after launch. As a competitor to SpaceX, we want to be able to bid against them for rocket launches. Understanding the likelihood of success for each launch is a crucial factor in determining our bid price.

To achieve this goal, we have collected data on previous Falcon 9 launches and landing attempts, including various features such as launch date, launch site, payloads, core, launchpad, and more. We have utilized this data to develop and train several machine learning models and have evaluated their performance.

<table>
  <tr>
    <td><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0701EN-SkillsNetwork/lab_v2/images/landing_1.gif" alt="Successful landing"></td>
    <td><p><strong>Following is an example of successful Landing</strong></p></td>
  </tr>
  <tr>
    <td><img src="https://hips.hearstapps.com/pop.h-cdn.co/assets/17/37/1505395625-sep-14-2017-09-25-38.gif?crop=1xw:0.898876404494382xh;center,top&resize=640:*" alt="Unsuccessful landing"></td>
    <td><p><strong>Several examples of an unsuccessful landing are shown here</strong></p></td>
  </tr>
</table>


### Data
The data used in this project was obtained through a combination of web scraping and API calls. We utilized SpaceX's official API, which can be accessed at the following link: <a href = 'https://api.spacexdata.com/'>SpaceX API</a>.

Additionally, we utilized Python's BeautifulSoup library to extract data from Wikipedia tables about Falcon 9 rockets. By combining these data sources, we were able to gather a comprehensive set of features for each Falcon 9 launch and landing attempt, including launch date, launch site, payloads, core, launchpad, and more.

### Models
To predict the success of Falcon 9 landings, we experimented with various machine learning algorithms, including logistic regression, decision tree classifier, Support Vector Machine (SVM), and K-Nearest Neighbor (KNN). Each model was evaluated using test accuracy and a confusion matrix was generated to compare actual versus predicted values.

### Results
| Model | Accuracy on Train Data | Accuracy on Test Data | True Positive | False Positive | True Negative | False Negative |
|-------|-----------------------|----------------------|---------------|----------------|---------------|----------------|
| Logistic Regression | 0.846 | 0.83 | 12 | 3 | 3 | 0 |
| Decision Tree Classifier | 0.848 | 0.83 | 12 | 3 | 3 | 0 |
| SVM | 0.875 | 0.89 | 11 | 1 | 5 | 1 |
| KNN | 0.848 | 0.83 | 12 | 3 | 3 | 0 |


### Repository Structure

This repository is organized into the following folders:

1. Data Collection: This folder contains scripts for collecting data from the SpaceX API and webscraping data from relevant websites.

2. Data Wrangling: This folder contains scripts for cleaning and preprocessing the collected data.

3. EDA: This folder contains notebooks and scripts for exploratory data analysis, including SQL queries and various visualization techniques using Matplotlib, Seaborn, and Folium.

4. Predictive Analysis: This folder contains scripts for implementing and evaluating various machine learning algorithms for predicting the success of Falcon 9 landings.

5. **requirements.txt:** lists the required Python packages for running the code.
    <code>pip install -r requirements.txt</code>


### Usage
To replicate our results, you can follow these steps:

- Clone this repository to your local machine.
- Install the required packages by running pip install -r requirements.txt.
- Run the notebooks in the respective order.

### Future Work
In the future, we plan to incorporate additional data sources, such as weather forecasts and satellite imagery, to improve the accuracy of our predictions. We also plan to explore more advanced modeling techniques, such as neural networks and gradient boosting.



