# Project 503 Overview

Team name: GPT Chasers
Team Member: Hongxuan An, Xingjian Liu, Yi Liu

NHANES dataset to analyze: 
2017-2018 Dietary Interview - Individual Foods, First Day (DR1IFF_J)
https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/DR1IFF_J.htm 

Data description: The dietary intake data are used to estimate the types and amounts of foods and beverages (including all types of water) consumed during the 24-hour period prior to the interview (midnight to midnight) and to estimate intakes of energy, nutrients, and other food components from those foods and beverages. 

We only focus on studying snacks: filtering data to DR1_030Z = 6

Two questions to explore:
The general goal is to predict the amount of different types of fatty acids in the snack from other features of the snack.  
Compare the performance of different machine learning models in predicting the amount of fatty acids
Identify key factors in predicting the amount of fatty acids

Response variables: 
We will build three separate models to predict the following variables:
DR1ISFAT - Total saturated fatty acids (gm)
DR1IMFAT - Total monounsaturated fatty acids (gm)
DR1IPFAT - Total polyunsaturated fatty acids (gm)
Approaches to investigate the two questions:
For the first question, we will try KNN, svm, trees and compare their performances, and investigate possible optimization methods (such as cross-validation and lasso/ridge penalties).
For the second question, we will investigate the feature importance in prediction using both statistical methods and machine learning methods.
