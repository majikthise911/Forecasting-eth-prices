# Forecasting Eth Prices Using Prophet

## Background

We will analyze patterns in hourly ETH prices and output a csv with 

## Instructions

Load the starter notebook into Google Colab and complete the following steps:

1. Execute the code cells under the "Notebook Set Up" section.

2. Label the columns `ds` and `y` so that the syntax is recognized by Prophet.

3. View dataframe shape, and the first and last five rows of the  DataFrame.

4. Sort the DataFrame by `ds` in ascending order, so as to arrange the data chronologically from past to present. With that done, visually inspect the price data using `hvplot`.

5. Call the `Prophet` function, and store it as an object.

6. `Fit` the time-series model.

7. Create a `future_trends` dataframe to hold predictions, using the `make_future_dataframe` function. (Make the prediction go out as far as 1,000 hours).

8. Make the predictions for the trend data using the `future_trends` DataFrame, and preview the first five rows of the DataFrame.

9. Plot the Prophet predictions for the `forecast_trends` data.

10. Use the `plot_components` function to visualize the forecast results.

11. Set the `datetime` index of the `forecast_trends` data, using the `ds` column.

12. From the `forecast_trends` DataFrame, use `hvPlot` to visualize the `yhat`, `yhat_lower`, and `yhat_upper` columns over the last 10 days (i.e., the last 240 rows).

13. Create a `forecast` Dataframe, which contains just forecasts for that month. The DataFrame should include the columns `yhat_upper`, `yhat_lower`, and `yhat`. Replace the column names to something less technical sounding: `Best Case`, `Worst Case`, and `Most Likely Case`, respectively.

14. Display the forcasted prices for the next 12 hours starting with the date specified. 