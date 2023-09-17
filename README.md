IMDB Rating Prediction
================
IS 407 Group 6

## Summary

Our objective was to answer the research question: How will the IMDB Score of a movie change based on various variables? We started with an initial hypothesis of choosing a certain set of predictor variables based on our intuition which we thought would be a good predictor for movie ratings. We performed a preliminary EDA while working on the proposal of the project where we summarized the statistics of the dataset, explored the missing columns to understand whether the variables we will be working with have a higher percentage of missing values and explored a few visualizations to understand basic trends about the dataset and how ideal they are with real-life. Next was the data cleaning which included removal of spurious characters from few columns, duplicate removal and conversion of currency dependent columns to USD for uniform data. We explored the Genre variables as part of the data cleaning process, doing a frequency analysis with bar chart and word-cloud to determine the most viewed genre in the dataset. For the word-cloud we loaded the Genre data as a corpus and created a document-term-matrix giving us a matrix with words and their frequencies. This was followed by building a correlation matrix to explore which variables have a stronger correlation to predict the IMDB score. Next, we continued the project with multiple visualizations to draw insights from multiple variables in the dataset including building a boxplot to explore the relationship between the IMDB Score with Content Rating variables, a Scatter plot between the IMDB Score and the median of the Director Facebook Likes to determine the relationship between the score and directors, a scatterplot to draw insights about the relationship between title year and the gross revenue of a movie. These visualizations gave us the opportunity to understand different trends in the data and to determine how each variable impacted the IMDB score. These visualizations helped us make decisions about our model. We incorporated the extraction of alt text from a plot where the function will return texts that could be used as alt-text in webpages. Next, we built our first model using Linear Regression by splitting the dataset into a 70-30 training and test data to predict the IMDB Score based on Duration, Gross and Year. Unfortunately, this model had a low R-squared value leading to inaccuracy in drawing insights about the IMDB score so we continued with a new linear model. The p-values and r-squared indicated that we needed to explore other types of variables to make a more accurate model. In the new model, we wanted to use categorical variables that were not included in the correlation matrix. We decided to add Profitability to our model, and we also added Number of Voted Users and Number of Critics Reviews. We weren’t able to add other variables like Actor like we mentioned in our initial proposal due to the large number of unique values. Our new models’ variables were chosen based on their correlation to the IMDB Score variable. When we fit this model, we saw a better R-squared score and all the p-values of each of the variables were lower than 0.05 which was the significance level we chose for our model. We also made a residual plot to see the spread of the data points and to see how much they differed from the original data. Our residual plot was not evenly distributed across the residual line, and we could see a curved pattern in that plot. This indicated that our linear model was not able to capture IMDB score based on the data variables provided. We tried a variety of different types of combinations but failed to get a random residual plot. This indicated that our dataset needed a different type of model other than the linear regression model. It could also be because none of our numerical variables were highly correlated to the IMDB score variable which may suggest that the dataset needs more rows of data or that the variables that would make a difference on IMDB score are not currently included in this dataset. Our predicted values from the model were pretty close to the original when we predicted our test dataset. However, we need to incorporate other variables that can be more significant to the model. In conclusion, through this project, we gained an insight into the relationship between IMDB scores and other variables like Gross and Duration and learned more about these independent variable’s relationship in regard to our dependent variable the IMDB score.

## Presentation

Our presentation can be found here (presentation_Dec5/presentation.html).

## Data
Yueming, Ilmi, F, ME2MLE,2017,IMDB 5000 Movie Dataset, Kaggle, <https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset>

## References

1. https://towardsdatascience.com/create-a-word-cloud-with-r-bde3e7422e8a

2. https://www.dataquest.io/blog/load-clean-data-r-tidyverse/

3. https://bookdown.org/Maxine/tidy-text-mining/tidying-a-document-term-matrix.html

4. https://analyticsindiamag.com/a-guide-to-term-document-matrix-with-its-implementation-in-r-and-python/

5. https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset


