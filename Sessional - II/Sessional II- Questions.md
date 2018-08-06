Sessional IIa
In today's exercise out task is to use Pandas to perform a number of simple yet highly effective data processing tasks. 
<br>
Please read in the csv file housing.csv. The file gives us a lot of detail about household in the state of California. The information is broken up according to zones (zones are like districts in India, but much smaller) of the state. 
<br>
Q.1) Obtain some cursory information about the structure of the file and the attributes using the pandas commands info and describe. Also find out about the length, size and shape of the dataset using the appropriate commands. Use the head and tail commands to peek into the data. How many unique values are there for the column "ocean_proximity". What are the values? Also, obtain an early visualization of the data using the hist() command on the dataset.
<br>
Q.2) What is the spread of the state of California in terms of latitude and longitude? Can you tell how many districts are on islands?
<br>
Q.3) In terms of average population, which are more populated, inland zones or zones "NEAR OCEAN". By how much?
<br>
Q.4) Two attributes are said to be correlated if a change in one is reciprocated by a change in the other. What is the correlation between the average number of rooms in a house to the price of the house. Can you visualize this using a scatter plot. Does the plot throw up some outliers? What is the near vertical nature of the plot suggesting? May be we can get a better understanding of the data if we view just the first fifty data points.
<br>
Q.5) Can we obtain a scatter plot of the data using the columns longitude and latitude. The scatter plot allows us to specify a colormap using the parameter cmap (e.g. cmap = plt.get_cmap('jet')). The colormap can be used by using the parameter c to set the color of a point depending on its value. Why don.t we use the median price of a house in a district to color the point. That way the more expensive a house is the more intense its color. We can also scale the size of a point using the parameter "s" by setting it equal to the population of a zone (scale the pop. by 25 to make the size manageable). Finally change the alpha value of the points to 0.1 to alter the opaqueness. There is a belief in California that the richest people stay near the coast. Does your plot support that view? But are the coast lines also more populous than the inlands?
<br><br><br>
For the next set of exercises read in the file appl.csv.  The dataset contains information about Apple Inc. stock prices over a period of time and the volume of stocks that were traded. Ensure that the Date column is used as the index column for the data and also ensure the Date column is treated as a datetime field and not a string or object field. The read_csv command takes various parameters like index_col=, parse_dates= etc. which can help you. Remember you can pass lists to these parameters to specify mot=re than one column.
<br>
Q.6) Introduce three columns into the dataset containing the date, month and year of the recording. You can obtain a value form of the index value by using df.index.values where df is the variable containing your data frame. This value is returned as an object which can be converted to a date time representation using pd.to_datetime(). The individual components like month, year, day can be obtained by using the attributes month, year and day. As an example a field containing the month value can be inserted as df["month"] = pd.to_datetime(pf.index.values).month.
<br>
Q.7) Start of by plotting the opening and closing stock prices for the first 50 days on the same plot. What does the data tell you? Remember pandas plot command requires you to explicitly specify the x and y columns. 
<br>
Q.8) Can you provide a plot for the day volatility of Apple's stock prices over time. The day volatility is the difference between the opening and closing values for a stock in a day. Is it true that Apple's stock has become more volatile in recent years?
<br>
Q.9) Can you plot the mean volume of stocks traded grouped by the day? Try to obtain a bar plot for the same. If the data seems too verbose, you can try to group by week, assuming the first day of a month is treated as the start of the first week of a month. Can we conclude that people tend to trade more stocks in the middle of the month?
<br>
Q.10) In which year on an average did Apple's stocks see the highest opening day values. Can we obtain a bar plot for the same?
<br>
Q.10) Is the volume of stock traded on a day more Gaussian in nature or more Poisson? May be a histogram will help us visualize this.
<br><br><br>
For the next set of exercises, we use the bike sharing data set. The data set gives us information about bikes loaned out to people in New York for commuting. Some of the people are registered users who take bikes every day, while others are casual users who loan bikes on an ad hoc bsis. The temp and humidity data in the data set is normalized between 0 and 1.
<br>
Q.11) Read in the file an ensure the instant field is treated as an index. The dteday field must be parsed as a date field. 
<br>
Q.12) Is it true that on an average registered users use bikes more on weekdays while casual users prefer to use bikes nearing the weekend. May be a bar chart for both grouped on week day will shed some light on this. By, the way which months are the hottest in New York on an average?
<br>
Q.13) In which, season do people prefer to use bikes the most? Plot a bar chart in support of your answer. What about the weather situation?
<br>
Q.14) In New York is it safe to say that high humidity usually leads to high temp, or are they independent of each other? What about windspeed?
<br>
Q.15) Can we have a scatter plot between windspeed and number of casual users. Another scatter plot may be plotted between wind speed and registered users. The scatter plot seem to have a similar nature but what does the scatter plots tell us? Look carefully at the values on the Y axis.
<br>
Q. 16) Can we justify that registered users usually loan their bikes at the start and end of office hours. A box plot of the registered users per column would be interesting. Data Frames have a boxplot function which can be used to visualize this data.