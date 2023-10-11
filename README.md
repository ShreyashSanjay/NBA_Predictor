# NBA_Predictor

[Basketball Reference](https://www.basketball-reference.com/)

## Scraping
I used the requests library to scrape through and get data from a website. Made use of selenium for pages that did not fully load data due to JavaScript code. <be >
Then make use of the BeautifulSoup library to convert the HTML to data that can be stored in a data frame (using pandas)

## Cleaning
Cleaning up the data set by removing any unwanted columns, removing some characters and replacing NaN with 0s. <be >
All three tables were combined and cleaned using different key values for merging and added some small visualisations to see trends.

## Machine Learning
I took a CSV file and read and cleaned the data. Split the data into train and test sets. Created an initial machine learning model, and looked at initial predictions for Shares. <be >
After some diagnostics to figure out what a good error matric should be, found that average precision and mean average precision were good. <be>
Used those error matrics to create a backtesting that could train and test across several years, to get a single error matric for all those years. <be>
I did more diagnostics to see which columns were used by the model and how to improve performance, then added more predictors for a little better accuracy. <be>
Then used a different algorithm (Random Forest) to get a bit better accuracy as shown.

## Next Steps
1. Doing a little bit more investigation: what to add, or to take away and even look at other data sources.
2. Generate more predictors in the set.
3. Play around with different ML models.
4. Try getting more data from the originally used source (by going back even further).
