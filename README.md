# Recipe2Cuisine
<p align="center">
<img src="images/logo.png">
</p>

As a member of the data team at an online publishing company, one of my verticals is a food publication. The product manager of the team wanted to build a feature for this vertical that enables users to query by cuisine, not just by ingredients. Specifically, recipes can be unlabeled and it's infeasible to label them by hand. Luckily, we have a training set of about 40,000 recipes with labeled cuisines. The goal of this project is to design and execute a method to predict the cuisine of a recipe given only its ingredients.


## Data

A list of cuisine-labelled recipes is stored in a dataframe (39,774 rows). Ingredients for each recipe are provided as strings and a total of 20 unique cuisines are present:

###
<p align="center">
<img width="450" height="180" src="images/data_table.png">
</p>

## EDA
Exploratory data analysis was performed before any pre-processing was done. Figures displayed below represent how many ingredients each of the 20 cuisine typically contains as well as the number of recipes there are for each cuisine. There appears to be a class imbalance with majority of the cuisines being Italian and Mexican. 

<p align="center">
<img src="images/EDA_BP.png">
</p>

<p align="center">
<img width="700" height="350" src="images/EDA_histogram.png">
</p>


## Pre-processing and TF-IDF
Texts in the ingredients column were first tokenized using comma seperations within the string of text before removing any characters that are not alphabets. Subsequently, lemmatization was performed on the texts before they were converted to a matrix of TF-IDF features for modelling.

## Models
Logistic regression and random forest classifier were used as modelling techniques for classifying each recipe to a cuisine. The dataset was split into train and test datasets. Cross-validation and resampling of the minority classes using SMOTE were implemented.

## Evaluation of Model
To evaluate how well our models performed, confusion matrices, accuracies and F1-scores were compated. Results of logistic regression and random forest were similar. Overall, it appears we are able to classify recipes as one of twenty cuisines with an accuracy up to around 70%. 


<p align="center">
<img src="images/CM.png">
</p>


