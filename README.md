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
   
  <p><b>Data Preparation</b></p>
   <li> Dropping rows having entire row as NAN</li>
   <li>Dropping columns which don't add value for the analysis</li>
  <li>Dropping duplicates</li><p>
<p><b>EDA</b>
  The primary goal of EDA is to support the analysis of data prior to making any conclusions. It may aid in the detection of apparent errors, as well as a deeper understanding of data patterns, the detection of outliers or anomalous events, and the discovery of interesting relationships between variables.
  
   <li> Review features are having high correlation with review score</li>
   <li>Rating columns are having highly positive correlation with dependent variable.</li>
   <li>Since economy class fares are less expensive, 77 percent of passengers opted to travel in this class.</li>
   <li>Highest travel history is present in the month of july</li>
   <li>he top 5 airlines preferred are Spirit, American, United, British, Emirates Airlines.</li><p>
     
  <p><b>IImputation of NaN values in independent and dependent columns:</b>
 <li>Using mean of sub ratings to fill NAN value in overall rating missing values.
<li>With the help of classification algorithms like GaussianNB,MultiNomialNB and GausianNB, prediction was made based on review text as input feature.
MultinomialNB is performing best in all naive bayes classifiers. Therefore now we have a model with 86% accuracy. We use this model to fill the dependent column.</li>
 <li>Using overall review score, filled the missing values in other sub-rating columns'.
</li>
</p>

<p><b>Feature Engineering</b>:
  Engineered new features based on-
  <li> review text such as polarity using VADER.</li>
  <li>overall rating column such as positive or negative review</li>
  <li>onehot encoding on cabin_type and travller_type to create new features.
</p>

<p><b>Model Building</b>
  Built different classifier models such as
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
</p>
Feature engineered performed to derive extra features from categorical and review columns. 
Built classifier models using different algorithms.
All the models give an accuracy of more than 85% and the same accuracy yielded on Cross validation also. 
Feature importance analysis done using Shap plots.
