# Capstone-Project--Airline-Passenger-Referral-Prediction
<p><b>Problem statement</b>: Data includes airline reviews from 2006 to 2019 for popular airlines around the world with multiple choice and free text questions. Data is scraped in Spring 2019.</p> 

<p><b>Objective</b>: The main objective is to predict whether passengers will refer the airline to their friends.</p>

<p><b>Description of features in the dataset</b>:
  <li>airline: Name of the airline.</li>
  <li>overall: Overall point is given to the trip between 1 to 10.</li>
   <li>author: Author of the trip</li>
   <li>review date: Date of the Review customer review: Review of the customers in free text format</li>
   <li>aircraft: Type of the aircraft</li>
   <li>traveller type: Type of traveler (e.g. business, leisure)</li>
   <li>cabin: Cabin at the flight date flown: Flight date</li>
  <li>seat comfort: Rated between 1-5</li>
   <li>cabin service: Rated between 1-5</li>
   <li>foodbev: Rated between 1-5 entertainment: Rated between 1-5</li>
   <li>groundservice: Rated between 1-5</li></p>
   
  <p><b>Data Preparation</b>:
   <li> Dropping rows having entire row as NAN</li>
   <li>Dropping columns which don't add value for the analysis</li>
  <li>Dropping duplicates</li></p>
  
<p><b>EDA</b>:
 The primary goal of EDA is to support the analysis of data prior to making any conclusions. It may aid in the detection of apparent errors, as well as a deeper understanding of data patterns, the detection of outliers or anomalous events, and the discovery of interesting relationships between variables.</p>
  
   <li> Review features are having high correlation with review score</li>
   <li>Rating columns are having highly positive correlation with dependent variable.</li>
   <li>Since economy class fares are less expensive, 77 percent of passengers opted to travel in this class.</li>
   <li>Highest travel history is present in the month of july</li>
   <li>he top 5 airlines preferred are Spirit, American, United, British, Emirates Airlines.</li><p>
     
  <p><b>IImputation of NaN values in independent and dependent columns</b>:
 <li>Using mean of sub ratings to fill NAN value in overall rating missing values.
<li>With the help of classification algorithms like GaussianNB,MultiNomialNB and GausianNB, prediction was made based on review text as input feature.
MultinomialNB is performing best in all naive bayes classifiers. Therefore now we have a model with 86% accuracy. We use this model to fill the dependent column.</li>
 <li>Using overall review score, filled the missing values in other sub-rating columns'.
</li>
</p>

<p><b>Feature Engineering</b>:
  Engineered new features based on-
  <li>Date of travel</li>
  <li> review text such as polarity using VADER.</li>
  <li>overall rating column such as positive or negative review</li>
  <li>onehot encoding on cabin_type ,Airlines and travller_type to create new features.</li>
</p>

<p><b>Model Building</b>:
  Built different classifier models such as
  <li>Logistic Regression</li>
  <li>DecisionTree</li>
  <li>Random Forest</li>
  <li>Gradient Boosting</li>
  <li>XG Boost</li>
  <li>SVM</li>
  
 <strenght>The performance is exceptionally good but we saw a scope of improvement where we can detect anomalies and replace the recommended column with the correct one.
All models are working great on this dataset and getting a good range of accuracies around 95%, which is pretty good. But to make sure our model is not in an overfitting condition performing cross validation techniques would help.GridSearchCV and Cross Validation techniques used are K-fold and Repeated K-fold. At every fold accuracy is 95% only this means that the models are actually working well on models.</strenght>
</p>
<p>

<p><b>Conclusions</b>:
  <li>We have built classifier models using 6 different types of classifiers and all these are able to give accuracy of more than 95%.</li>
  <li>The most important features are Overall rating and Value for money that contribute to a model's prediction.</li>
  <li>The classifier model developed will enable airlines ability to identify impactful passengers who can help in bringing more revenue by referring more acquaintances.</li></p>
