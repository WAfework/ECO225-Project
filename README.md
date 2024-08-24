This repository contains the paper, notebooks, code and final dataset for my project for ECO225 (Winter-2024) on Airbnb pricing determinants in NYC. All code is my own and the research question was unique for the course. In particular my approach to using tourist attractions data and their associated reviews to calculate popularity and tourism proximity scores was a novel method. My finding that that a listing's proximity to a larger number of popular tourist destinations was the biggest determinant of price was also novel. The findings were statistically significant and served to explain a larger portion of variance (53.8%) than similar papers in the field (Toader et al., 2020; Gibbs et al,. 2017; Deboosere et al., 2019).

## Methods

To explore and analyze the factors influencing Airbnb pricing, I employed a variety of data analysis and machine learning techniques:

- **Exploratory Data Analysis (EDA)**: Visualizations, including scatter plots and heatmaps, were used to identify patterns and correlations in the data. Key variables such as location, room type, and number of reviews were examined.
  
- **Multi-variable Regressions**: Regression models were used to quantify the relationship between various predictors (e.g., number of reviews, room type, proximity to tourist attractions) and Airbnb prices. These models helped isolate the impact of individual variables while controlling for others.
  
- **Decision Trees and Random Forests**: To capture non-linear relationships and interactions between features, decision trees and random forests were employed. These models provided insights into the importance of different variables in predicting Airbnb prices, with `Normalized_Tourism_Proximity` emerging as the most significant predictor.
  
- **Feature Engineering**: Custom features, such as `Tourism Proximity Scores`, were created by analyzing the spatial distribution of tourist attractions and their associated popularity. This novel approach provided a new perspective on how tourism impacts local rental markets.

## Key Findings

Some findings of the project were novel (explained further in the paper) or strengthened the existing literature. The analysis showed that a listing's proximity to popular tourist destinations is a major determinant of price, which was a unique contribution to the field. The findings were statistically significant and served to explain a larger portion of variance (53.8%) than similar papers in the field (Toader et al., 2020; Gibbs et al,. 2017; Deboosere et al., 2019).

## Documents

- [Final Paper](./Final_Paper.pdf): The final version of the paper, including all figures and results. *Highlights results from project.*
- [Final Notebook](./final_jupyter_notebook.pdf): PDF version of the final jupyter notebook. *Contains a more 'walk-through' like explanation of the code and methods.*
- [Final Dataset](./final_df.csv): Contains aggregated data from Airbnb, NYC DCP, American Community Survey, US Census and scraped data from Google. 

## Figures

All figures used in the paper are stored in the [paper-figures](./Paper%20Figures) directory. Some example paper figures are shown below.

![Tourism Maps](./Paper%20Figures/fig4-tourismmaps.png)

*Figure 4: Distribution of Airbnb Listings and Tourist Attractions in NYC.*

![Random Forest Model](./Paper%20Figures/fig9-rfm.png)

*Figure 9: Feature Importance in Predicting Airbnb Prices Using Random Forest.*
