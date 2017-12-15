
# Bank Marketing:

## Introduction:

The data is related with direct marketing campaigns of a Portuguese banking institution. 

The marketing campaigns were based on phone calls Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

With the provided dataset I am trying to analysis and predict if the clients after marketing campaign will subscribe to term deposit or not.

Portuguese banking institution is the client, it will help them to analyze

1) whether their marketing campaign is success, 
2) what other methods or changes they can do to improve in the campaign
3) What's the effectiveness  of the campaign and points to continue from their last campaign
4) Whether they are targeting the right set of audience.

My analysis will help them to make a decision as to how to improve their campaigns so that they can achieve more clients subscribing to their term deposit.

## Information on dataset:

Bank Marketing Data Set: https://archive.ics.uci.edu/ml/datasets/bank+marketing

We have four datasets list below
* bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]
* bank-additional.csv with 10% of the examples (4119), randomly selected from 1), and 20 inputs.
* bank-full.csv with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs). 
* bank.csv with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs). 

And below are the key attributes 
* Job
* Education
* Default which gives if the have any default credit or not
* housing
* loan
* previous outcome of campaign 
* whether client has subscribed to term deposit or not.

## Limitations on dataset:

The given dataset has limited amount of data present regarding previous campaign outcome, so its difficult to determine if the previous campaign is successful or not with small sample of data.

## Data cleaning and Wrangling:

The dataset was clean with all the null and missing fields filled with unknown.
The data was present in csv format, using padas read_csv with delimiter we were able to get the dataframe

We had around 4 datasets with information which we could use for our analysis.


## Observations based on preliminary exploration:

Here is the link to data analysis - https://github.com/SoundaryaViji/capstone_project/blob/master/BankDetails.ipynb with a single set of data

* From the given data we can observe that the clients who have management jobs with secondary degree and who doesnt have any loans and in between age of 27 to 37 are the ones who have subscribed to term deposit the most.
* Protugal has fiscal year from January to December and we expected the term deposit to be more during these months but it turned out that during month of May there are more number of clients subscribing to term deposit. It may be due to performance apparisal cycle or bonus pay cycle but we dont have substantial information to confirm this theory.
* We have around 18 percent of clients who have subscribed to term deposit after pervious campaign and current campaign.
* From the campaign results its clear that unemployed clients are not susbcribing to term deposit. Students contribute to very low percentage of clients who subscribed to term deposit.
* From our initail analysis clients who are married and who have management/blue collar and those who are finanically stable are the clients who subscribe for term deposit.
* With the given data we can find that for a successful campaign the category of clients we need to contact and for category of clients are not subscribing.


## Approach:

The inital exploration has been useful to understand trends in the data.
The the main goal of the project to create a predictive model which can predict if the clients will subscribed to term deposit.

We will use supervised training with classification to predict the clients subscription 

