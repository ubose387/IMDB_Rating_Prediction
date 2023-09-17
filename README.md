# IMDB Rating Prediction

The main goal of this project was to investigate how various factors influence the IMDB Score of movies. Initially, I formulated a hypothesis and selected a set of predictor variables that I believed would be strong indicators of movie ratings. The project progressed through several stages, starting with preliminary Exploratory Data Analysis (EDA) during the proposal phase.

Data Exploration and Cleaning:
During the preliminary EDA, I conducted basic statistical summaries of the dataset and examined missing data to assess the quality of variables. Additionally, I performed data cleaning tasks such as removing unwanted characters from columns, eliminating duplicates, and converting currency-related columns to USD for consistency. I also delved into the Genre variables, conducting frequency analysis through bar charts and word clouds to identify the most prevalent movie genres.

Correlation Analysis:
To gain insight into which variables had the most significant correlation with the IMDB Score, I constructed a correlation matrix. This analysis helped me identify potential predictor variables for the IMDB Score.

Data Visualization:
I created multiple visualizations to extract insights from various dataset variables. These visualizations included a boxplot to explore the relationship between IMDB Score and Content Rating, a scatter plot to assess the correlation between IMDB Score and the median of Director Facebook Likes, and another scatter plot to investigate the relationship between the release year and movie gross revenue. These visualizations aided in understanding different trends and determining the impact of each variable on the IMDB Score.

Model Building and Refinement:
I proceeded to build a linear regression model, initially using Duration, Gross, and Year as predictors. However, this model yielded a low R-squared value, indicating its inadequacy in predicting IMDB Scores accurately. To improve the model, I introduced categorical variables such as Profitability, Number of Voted Users, and Number of Critics Reviews, based on their correlation with the IMDB Score. The new model exhibited a better R-squared score, with all p-values below the significance level of 0.05.

Model Evaluation:
I created a residual plot to assess the model's performance, which revealed a non-linear pattern in the residuals. This indicated that a linear regression model might not be suitable for predicting IMDB Scores accurately. Possible reasons for this included the need for additional variables not present in the dataset or an insufficiency of data points to establish strong correlations.

Conclusion:
In conclusion, this project provided valuable insights into the relationship between IMDB Scores and various factors, including Gross, Duration, Profitability, Number of Voted Users, and Number of Critics Reviews. While the linear regression model showed promise, further exploration is needed to identify and incorporate additional variables that could enhance the model's accuracy. This project underscores the complexity of predicting IMDB Scores accurately and highlights the importance of continuous data exploration and model refinement.


## Data
Yueming, Ilmi, F, ME2MLE,2017,IMDB 5000 Movie Dataset, Kaggle, <https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset>

## References

1. https://towardsdatascience.com/create-a-word-cloud-with-r-bde3e7422e8a

2. https://www.dataquest.io/blog/load-clean-data-r-tidyverse/

3. https://bookdown.org/Maxine/tidy-text-mining/tidying-a-document-term-matrix.html

4. https://analyticsindiamag.com/a-guide-to-term-document-matrix-with-its-implementation-in-r-and-python/

5. https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset


