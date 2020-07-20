# Classify titanic accident victmans: Project Overview
* Created a model based on Machine Learning to predict into survival or deceased.

# Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, sklearn, matplotlib, seaborn

 
## EDA
For the first step I checked the data set about the missing values and the result was the *missing values heatmap*, that demonstrates around 20% of missing data in the age column and many missing values in the cabin column.
To dicrease the impact of the age column missing values, I calculated the average age for each class of the titanic, as presented in the *age per class boxplot* figure. And for last, after some featuring engineering, I filled the missing values with these average ages and the result is present in the last *filled missing values* heatmap figure.

The cabin column was dropped, because it were many missing values to try some similary approach as I did with the age column. 

![alt text](https://github.com/Bereoff/titanic_project/blob/master/missing_values_heatmap.png "missing_values_heatmap")
![alt text](https://github.com/Bereoff/titanic_project/blob/master/Age_avg.png "Average Age among the 3 classes of titanic")
![alt text](https://github.com/Bereoff/titanic_project/blob/master/filled_missing_values_heatmap.png "filled_missing_values_heatmap")

## Model Building 
First, I splitted the data into train and test sets with a test size of 30%.   
After training the data, I tested the model to predict the results on the splitted test data.

## Model performance

![alt text](https://github.com/Bereoff/titanic_project/blob/master/classification_report.JPG "Classification Report")

The results for the overall model performance are great. 

The precision is over 80% for both features (Survived / not survived).
The recall is a little bit lower then the others key classification metrics, but even that it is a reseanable result.
The F1-score and Accuracy are great too.

As demonstrated, the model presented a good performance to predict the survival or deceased, but it demands more improvement to do.
