# Dry-Beans-Classification

<h3 align="center">A competition on Kaggle held by ITI AI-Pro. </h3>
<h3 align="center">Winning 2nd place (with the same private score of the 1st team and higher public score) in the competition. 🏆💪🔥</h3>

![various-kidney-beans](https://user-images.githubusercontent.com/49573699/191672305-90384a56-08c7-44c5-a53e-3eec7f50c264.jpg)


## Dataset Information

Given a set of features extracted from the shape of the beans in images and it's required to predict the class of a bean given some features about its shape. There are 7 bean types in this dataset.


![7_types](https://user-images.githubusercontent.com/49573699/191672504-73287eea-b5a2-410c-8281-ca3c24fe324c.jpg)

- Observations:
  - Training: 10834
  - Test: 2709
- Features: 16

### Data Fields
* ID - an ID for this instance
* Area - (A), The area of a bean zone and the number of pixels within its boundaries.
* Perimeter - (P), Bean circumference is defined as the length of its border.
* MajorAxisLength - (L), The distance between the ends of the longest line that can be drawn from a bean.
* MinorAxisLength - (l), The longest line that can be drawn from the bean while standing perpendicular to the main axis.
* AspectRatio - (K), Defines the relationship between L and l.
* Eccentricity - (Ec), Eccentricity of the ellipse having the same moments as the region.
* ConvexArea - (C), Number of pixels in the smallest convex polygon that can contain the area of a bean seed.
* EquivDiameter - (Ed), The diameter of a circle having the same area as a bean seed area.
* Extent - (Ex), The ratio of the pixels in the bounding box to the bean area.
* Solidity - (S), Also known as convexity. The ratio of the pixels in the convex shell to those found in beans.
* Roundness - (R), Calculated with the following formula: (4piA)/(P^2)
* Compactness - (CO), Measures the roundness of an object: Ed/L
* ShapeFactor1 - (SF1)
* ShapeFactor2 - (SF2)
* ShapeFactor3 - (SF3)
* ShapeFactor4 - (SF4)
* y - the class of the bean. It can be any of BARBUNYA, SIRA, HOROZ, DERMASON, CALI, BOMBAY, and SEKER.


## Exploratory Data Analysis (EDA)

- Exploring the dataset.
- Getting summary statistics. 
- Checking for null values and duplicated records.
- Apllying Some visualizations for more insights.

## Data Import
Importing needed libraries to get started, training and testing data.

## Feature engineering
Applying some feature engineering techniques trying to extract new features that help our model more to classify. 

## Data visualization
- Viewing Featurs Correlation: (using heatmaps) to help us in features selection
- Features Importance: to get our most important features

## Data Preparation
- Label Encoding
- Features Normalization

## Dimensionality Reduction
Apllied using PCA to our features.

## Modeling
Training differnt classifiers and selecting best ones to be combined together in a VotingClassifier which performed better than individual ones.

## Models Evaluation
Metrics Used:
* F1 Score
* Recall
* Precision

## Results
- Our Final VotingClassifier is used resulting F1-score 0.95378 on the Public Score and 0.94003 on the final testing set.
- Our Team could achieve the 2nd place (with the same private score of the 1st team and higher public score than them) in this competition among 35 other Teams. 💪🔥
- [Competetion Link](https://www.kaggle.com/competitions/dry-beans-classification-iti-ai-pro-intake02/discussion/329172)
