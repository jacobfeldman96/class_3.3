# Class 3.3

Today's class began with a review of Pandas and a deeper dive into data analysis techniques in Pandas. We started by reviewing proper data mining procedure. Important notes are to use correct data types, i.e. if a column should consist of floats, remove anything that would convert the column into a string. Another important aspect of data mining is choosing the correct column for the index. 

Review of data mining technique: 
1. import libraries
2. import data into Pandas Datafram and explore it, take out of nulls & special characters
3. Replace missing string values with 'unknown', a 0 in all numeric columns and remove special characters from numeric columns. 
4. Check if there are any duplicates in index column and drop them. Keep original DF as a copy. 
5. Convert numeric columns into floats for further analysis. 

We spent some time reviewing the differences between loc, get_loc and iloc. The difference being how much initial data one has. If one has the indeces/columns required, iloc is appropriate. If one knows of the column but not the specific row, get_loc is appropriate. If one is just searching for a specific string value, loc is appropriate. 

Data visualization: %matplotlib inline gives one access to data visualization techniques. An important function in pandas is the following 

x = pd.to_datetime(csvfile['Date], infer_datetime_format = True, inplace = True)

Returns: 
We discussed what an ROI is and its use in the world of finance. We further discusses **Daily Returns** which is a daily ROI calculation and **Cumulative Returns** which is the total return made from the time of initial investment. 

Important point, most stock analysis is made on the adjusted closing price. pct_change() is the pandas function responsible for this. I was having trouble with the one activity and couldn't trouble shoot on my own. Will ask in office hours. .cumprod() is the cumulative variable function in pandas. 

We then discussed Data sliceing and used the variable function .loc('yyyy-mm-dd' : 'yyyy-mm-dd') to find a specific subset of data when time is the index. parse_dates=True is a helpful addition to a pd.read_csv function to separate dates as the index 

Sorting Data: we discussed various functions for sorting values and indeces. The default is ascending=True. With pd.DataFrame one can create their own DF. 

We then discussed grouping and its use. pd.groupby is the function to call data grouping. Lastly, we discussed the use of concatenation which is literally the pasting of two or more DF's together. Was having difficulty with the last exercise and will trouble shoot during office hours. 