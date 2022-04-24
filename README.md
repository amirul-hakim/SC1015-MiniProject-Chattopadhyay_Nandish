## Welcome to Airline ticket Analysis Repository 

### About 
This is a Mini Project for SC1015/CE1115/CZ1115/ INTRO TO DATA SCI & ART INTELLIGENCE which focuses on the price for Air Travel Industry in India. For the walkthrough, please kindly refer to the source code below - <br>
[Flight Fare Prediction_Final](http://localhost:8888/notebooks/ntu/Y1S2/SC1015/Mini-Project/Flight%20Fare%20Prediction_Final.ipynb)

### Team members [Group C]:
Ang Han Ye<br>
Amirul Hakim<br>
Foo Siang Jen<br>
    
### Contributors
Han Ye - Code <br>
Hakim – Code/Slides <br>
Siang Jan – Slides/Script <br>

### Problem Definition
<b>When should passengers purchase their airline ticket to get the cheapest price when flying in India?</b>

Model Used: 
<li>Decision Tree</li>
<li>Confusion Matrix</li>
<li>Random Forest</li>

### Conclusion
<b>For Exploratory Data Analysis</b>
<br>
Increased in outliers on Air India price ticket as compared to the other airline and overall the prices among different airlines are estimated at six thousand mark
There is a linear correlation between days left before departure to purchase air ticket vs price. Usually about 2 weeks in advance will be the most prefer period for the lowest price
There is a positive linear relation between number of stops vs price. However, based on our understanding, it should be a negative relation as the price should decrease with the number of increasing stops. 
For time of day vs price, it seems to have a common phase when the price spike, which is in the morning period and a gradual decrease during night time

<b>For Machine Learning</b>
<br>
As for the DecisionTree, we have optimized the accuracy by adjusting the max-depth to 5 to obtain an accuracy score of 65% for our train data.

To better improve the accuracy and achieve a higher True Positive Rate, we used RandomForestClassifier. We made further optimization by adjusting the n_estimators and max_depth to 100 and 15 respectively in order to achieve a better results. Hence, we managed to obtained the following results: Accuracy = 86% TPR = 90% FPR = 15%

From the the DecisionTree and RandomForestClassifier models, we achieved a higher accuracy on the RandomForestClassifier at approximately 70 - 80% and a lower FPR below 30%. This gives us a better model to predict the flight prices near to the actual price for majority of the variables.

### What did we learn from this project?
<li>Line Plot EDA</li>
<li>Usage on OneHotEncoder from sklearn.preprocessing for categorical variables</li>
<li>Handling and categorising datasets for easier computation and visualization</li>
<li>RandomForest from scikit-learn</li>

### Reference 
https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction<br>
https://seaborn.pydata.org/generated/seaborn.lineplot.html<br>
https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html<br>
https://www.analyticsvidhya.com/blog/2022/01/flight-fare-prediction-using-machine-learning/<br>
https://medium.com/analytics-vidhya/regression-flight-price-prediction-6771fc4d1fb3<br>
