Open In Colab
Forecasting Bitcoin Prices Using Prophet
Background
We will analyze patterns in hourly Bitcoin prices, believing that building a model which can forecast prices into the future will give an idea if investing in Bitcoin is worth or not.

Instructions
Load the starter notebook into Google Colab and complete the following steps:

Execute the code cells under the "Notebook Set Up" section.

Read in the bitcoin_hourly CSV file. Drop the volume column.

Label the columns ds and y so that the syntax is recognized by Prophet.

View dataframe shape, and the first and last five rows of the DataFrame.

Sort the DataFrame by ds in ascending order, so as to arrange the data chronologically from past to present. With that done, visually inspect the price data using hvplot.

Call the Prophet function, and store it as an object.

Fit the time-series model.

Create a future_trends dataframe to hold predictions, using the make_future_dataframe function. (Make the prediction go out as far as 1,000 hours).

Make the predictions for the trend data using the future_trends DataFrame, and preview the first five rows of the DataFrame.

Plot the Prophet predictions for the forecast_trends data.

Use the plot_components function to visualize the forecast results.

Set the datetime index of the forecast_trends data, using the ds column.

From the forecast_trends DataFrame, use hvPlot to visualize the yhat, yhat_lower, and yhat_upper columns over the last 10 days (i.e., the last 240 rows).

Create a forecast_march_2021 Dataframe, which contains just forecasts for that month. The DataFrame should include the columns yhat_upper, yhat_lower, and yhat. Replace the column names to something less technical sounding: Best Case, Worst Case, and Most Likely Case, respectively.

Display the average forecasted price for March 2021
