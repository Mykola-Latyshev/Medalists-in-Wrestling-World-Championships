# Medalists-of-Wrestling-World-Championships

### Table of Contents 
1. Introduction
2. Aim
3. Technology
3. Data
4. Preprocessing
5. Early EDA
6.  Final EDA
7. Modelling
8. Future Development

### Introduction

Analysis and prediction of athletes’ results are important tasks of sports science (sports psychology). In the short term, the solution of this problem allows  to determine the selection of more promising athletes and, in the long term, to optimise the athletes training.

### Aim

The project aims to predict wrestling medalists in world championships and to determine the features which are the most crucial ones for the prediction process. 

### Technology used

Python
Pandas
Numpy
Matplotlib
Seaborn
Scikit-Learn

### Data 
The data contain information about the sports careers of the freestyle and Greco-Roman male wrestlers who participated in the World Championships 2017, 2018. Before preprocessing, the information included such components: full name, date of birth, and international level results (name of competition, date, and rank).
The data of the results have been taken from the official site of the “United World Wrestling” (unitedworldwrestling.org).

The data were collected in the following format:
![01_raw_data_example](https://user-images.githubusercontent.com/82052288/161391241-e0ca2907-9a5f-4477-9748-48240d6c381c.jpg)

### Preprocessing
The DataFrame was created for the final analysis and modelling during preprocessing. Each row of the DataFrame contains the achievements of a particular athlete for the entire career period prior to participating in the World Championship.
A set of 16 features was compiled: age, relative age effect (RAE, including month/quarter/half year of birth), achievements in U18 competitions (participation/medalist/winner), achievements in U21 competitions (participation/medalist/winner) and achievements in continental and world championships until the moment of participation in the analysed competitions.
The final DataFrame looks like this:
![02_dataframe_example](https://user-images.githubusercontent.com/82052288/161391213-dd9dda0e-3f19-4d1e-abc5-16b4c6baab2c.jpg)
### Early EDA
At the first stage of the EDA, I identified outliers/errors/inaccuracies made at the stage of data preprocessing. They were removed (less than 1% of the sample).
### Final EDA
At the next stage of the analysis, I studied the relationship between the target and features. Histograms of targets were compiled; the first graph shows the dependence of the number of athletes on the place taken. It is worth noting that according to the new wrestling rules, there is no 4th place.

Percentage of medalists, %: 13.359528487229863
