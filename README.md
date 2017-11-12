Stephanie Le Grange
Mercyhurst University Grad Student
DATA 550 Data Visualization

## This repository contains the following:
1. This readme
2. Animals in Shelters from Kaggle: Shelter animal outcomes.
3. My project from my Jupyter notebook

## Table of Contents

- [Background] (#background)
- [Programs Used] (#programs used)
- [Reason for Data Set] (#reson for data set)
- [Project Explaination] (#project explaination)
- [Acknowledgements] (#acknowledgements)

### Background

The data that was used inthis project is from data that was collected from October 2013 to March 2016 by Austin Animal Center. 
The data show the outcomes of animals that are in shelters, all the animals were given an ID during the intake.
The outcomes include: Adoption, Death, Euthanasia, Returned to owner, and Transfers.

Approximately 7.6 million dogs and cats end up in US shelters. Most of these animals are given up by their owners, while other are pickedup or taken from cruelty situations. 2.7 million of these dogs and cats are euthanized int he US each year.
We are going to be usign breed, color, sex, and age to prodect the outcome of each animal.

This data will help us understand the trends in shelters when it comes to the animasl outcomes, which could help help sheelters focus their energy on the specific needs of the animals and help them find their forever homes.

This data was evaluated usint the multi-class logarithmic loss, a set of probabilities were submitted fro every class and the belwo formula was then used. 

logloss=−1N∑i=1N∑j=1Myijlog(pij).

### Programs Used

Python along with the following packages 
pandas
numpy
matplotlib
seaborn
the following zip files were added as well
train.csv - Training set
test.csv - Test set
sample_submission.csv - Sample submission file 

### Reason for Data Set

This is a class project that is similar to projects being doen by other students in the class. 

### Project Explaination

In this data we are going to take a look at the outcome of animals in shelters based on their age, gender, neutered/spayed, and species.
First we will look at the date in both the train and test files, I pulled the first ten sets of data from each file.

AnimalID	Name	DateTime	OutcomeType	OutcomeSubtype	AnimalType	SexuponOutcome	AgeuponOutcome	Breed	Color
0	A671945	Hambone	2014-02-12 18:22:00	Return_to_owner	NaN	Dog	Neutered Male	1 year	Shetland Sheepdog Mix	Brown/White
1	A656520	Emily	2013-10-13 12:44:00	Euthanasia	Suffering	Cat	Spayed Female	1 year	Domestic Shorthair Mix	Cream Tabby
2	A686464	Pearce	2015-01-31 12:28:00	Adoption	Foster	Dog	Neutered Male	2 years	Pit Bull Mix	Blue/White
3	A683430	NaN	2014-07-11 19:09:00	Transfer	Partner	Cat	Intact Male	3 weeks	Domestic Shorthair Mix	Blue Cream
4	A667013	NaN	2013-11-15 12:52:00	Transfer	Partner	Dog	Neutered Male	2 years	Lhasa Apso/Miniature Poodle	Tan
5	A677334	Elsa	2014-04-25 13:04:00	Transfer	Partner	Dog	Intact Female	1 month	Cairn Terrier/Chihuahua Shorthair	Black/Tan
6	A699218	Jimmy	2015-03-28 13:11:00	Transfer	Partner	Cat	Intact Male	3 weeks	Domestic Shorthair Mix	Blue Tabby
7	A701489	NaN	2015-04-30 17:02:00	Transfer	Partner	Cat	Unknown	3 weeks	Domestic Shorthair Mix	Brown Tabby
8	A671784	Lucy	2014-02-04 17:17:00	Adoption	NaN	Dog	Spayed Female	5 months	American Pit Bull Terrier Mix	Red/White
9	A677747	NaN	2014-05-03 07:48:00	Adoption	Offsite	Dog	Spayed Female	1 year	Cairn Terrier	White

We then take a look at how many dogs and cats are in our data and that were evaluated for this data.
Second we look at the outcome for all the cats and dogs that were used for this data. We can see that majority of the animals are either adopted or transfered to other shelters.

Now that we know the outcome fro majority of the animals in shelters is either adoption, transfer or returned back to tthei owners we want to look into the sex of the animals and how that effects the outcome.
Using sex we see that males and females are pretty close in comparrison which does not help us much, so we add in wether the animals are neutered or intact. this shows us that neutered animals are favored. 
For fun we can even add wether animals that are mixed breeds are favored or pure bred animals. From the data we see that mix breeds are faovred, but we cannot rely on this as most animals in shelters are either mix breeds or unknown.
Finally, we add the information together to narrow dow the outcome of the animals. The next few graphs will look at the outcome bewteen both cats and dogs.
We see that both cats and dogs have a high probability of beign adopted and transfered, but dogs have a higher rate of being returned back to their owners. 

Lastly we look at age of the animals in shelters and the outcome. Most animals in shelters are between age 1 and 2 as shown from the below graph and younger animals are favored over older animals. we can also see that older animals have a higher chance of being returned back to their owners. 




### Acknowledgements

The dataset is brought to us by Austin Animal Center and the shelter animal statistics were taken from the ASPCA
