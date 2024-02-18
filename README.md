# Project_Starbuscks_Capstone

Blog link [here](https://medium.com/@tatiana.gnz7/capstone-project-7fc875cec915)

## Libraries

This project requires Python 3 and the following Python libraries installed: Package Version.txt

## Motivation for the Project 

The project is a representation of an experiment development for Starbucks. The data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers. <br>
Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. <br>
Each person in the simulation has some hidden traits that influence their purchasing patterns and are associated with their observable traits. People produce various events, including receiving offers, opening offers, and making purchases.<br>
The basic task is to use the data to identify which groups of people are most responsive to each type of offer, and how best to present each type of offer.<br>

## Data Sets
The data is contained in three files:

- portfolio.json
id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)

- profile.json
age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income

- transcript.json
event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record

## Summary

Understanding and define which are the groups and offers that really excited people. 
Build a machine learning model that predict offer success based on the demographic information and the offer details that are provided in the data.

The Random Forest Classifier model can be used to predict whether an offer is going to be successfully completed based on customer and offer characteristics. The final model has an accuracy of 74%, which is a decent number for business purposes, although there is certainly room for improvement. <br>

__Who spends more money? male or female?__
And by graph data we can say that Female spend more money, and that can help in targeting customers for starbucks


## File Descriptions

This github repo contains

* Starbucks_Capstone_notebook.ipynb -> Consists of a notebook with all the work. 
* model_data_prepared.csv -> Consists of a database with the cleaned and prepared data for model.
* Package Version.txt -> Consist of a list with all the libraries and packages.


## Project Components

- Project Definition
- Analysis
- Methodology
- Results
- Conclusion

## Acknowledgement

Data used in this project is taken from Starbucks in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed
