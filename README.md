# Capstone-Project--Airline-Passenger-Referral-Prediction
<p>Problem statement: Data includes airline reviews from 2006 to 2019 for popular airlines around the world with multiple choice and free text questions. Data is scraped in Spring 2019.</p> 
<p>Obkective: The main objective is to predict whether passengers will refer the airline to their friends.</p>

<p>Description of features in the dataset:
airline: Name of the airline.
overall: Overall point is given to the trip between 1 to 10.
author: Author of the trip
review date: Date of the Review customer review: Review of the customers in free text format
aircraft: Type of the aircraft
traveller type: Type of traveler (e.g. business, leisure)
cabin: Cabin at the flight date flown: Flight date
seat comfort: Rated between 1-5
cabin service: Rated between 1-5
foodbev: Rated between 1-5 entertainment: Rated between 1-5
groundservice: Rated between 1-5</p>

Performed EDA on the features and draw inferences w.r.t. target feature i.e. Recommended. 
Filled missing values on Target variable based on Overall rating feature.
Feature engineered performed to derive extra features from categorical and review columns. 
Built classifier models using different algorithms.
All the models give an accuracy of more than 85% and the same accuracy yielded on Cross validation also. 
Feature importance analysis done using Shap plots.
