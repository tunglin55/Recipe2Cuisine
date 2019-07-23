# Recipe2Cuisine
<p align="center">
<img src="images/logo.png">
</p>

Assuming you've just joined the data team at an online publishing company, and one of your verticals is a food publication. A product manager wants to build a feature for this vertical that enables users to query by cuisine, not just by ingredients. Specifically, recipes can be unlabeled and it's infeasible to label them by hand. But luckily, we have a small training set of about 40,000 recipes with labeled cuisines. Thus, the goal of this project is to design and execute a method to predict the cuisine of a recipe given only its ingredients.


## Data

Lists of ingredients of various recipes are stored in a dataframe. A total of 20 different cuisines are present in the dataset with 39774 different recipes. Figures below represent the number of counts of cuisines as well as boxplots of how many ingredients each dish per cuisine contains. 

###
<p align="center">
<img src="images/data_table.png">
</p>


## EDA

###
<p align="center">
<img src="images/EDA_histogram.png">
</p>

<p align="center">
<img src="images/EDA_BP.png">
</p>


## Pre-processing and TF-IDF
Texts of the 

## Models
Logistic regression and 


## Evaluation of Model
Give that the webapp is deployed, there are several key performance indicators that can be used to evaluations. For example, how far do the accuracy of the predictions deviate from the needs of the companies? Are traffic delays reduced after the deployment of the webapp? and how many users are using this webapp? Additionally, the ability to predict car traffic in this project can be generalized to other domains as well: network traffic, social traffic and even population flow. 

<p align="center">
<img src="images/CM.png">
</p>
