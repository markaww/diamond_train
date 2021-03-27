# Diamond train
## Dataset analysis 


### Part 1 - Analysis

In this project, I explored a dataset of 40.000 diamonds. The data set displayed a number of columns containing qualitative details for each diamond along with it's price. The goal of this project was to visually identify trends/insights in this dataset. 

In the first stage, I explored the data on a jupyter notebook, plotting as many graphs as possible to identify interesting features in the dataset

Quite quickly, I could see a correlation between the 4 C's (Color, Carat, Cut and Clarity) and the price, as is often stated on diamond related narrative. However, what quickly also emerged is that some of the C's had a stronger impact on the price than others. Namely, carat and color affected the price more than clarity and cut. 

With this in mind, I took the dataset to tableau, and visually explored the dataset further. My findings are available in this public tableau project:

https://public.tableau.com/profile/mark.a.westmacott#!/vizhome/Diamond_train/Story3

Indeed, it seems like while clarity and cut do increase price from low quality to mid quality diamonds, after a certain point, as we progress towards higher clarity and better cut diamonds, the price does not appear to increase as much. 


### Part 2 - Machine learning model

In the second part of this project I took the same dataset and applied a machine learning model to predict the price of new diamonds, based on the features of the existing ones

The model uses SimpleImputer, RobustScaler and OrdinalEncoder to prepare the data, and then applies a LGBMRegressor as model. The hyperparameters of the model were also optimized with RandomizedSearchCV and GridSearch. The results were uploaded to kaggle for an internal Ironhack competition
