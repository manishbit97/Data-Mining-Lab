Sessional I(a)
In our first exercise we do some basic data handling using numpy.

Read the file iris.numeric.txt into python using numpy's genfromtxt command. Explore the options available in the command. (Remember in jupyter pressing shift+tab shall show parameter hints).
Can you print some basic statistics for the four numeric attributes like the mean value, the standard deviation, the max, the min, the 25th and 75th quantile etc. Remember the kth quantile has k percent of data below that value. While functions ar available in numpy to do all these activities, try to write your own code to get the results.
Use matplotlib.pyplot to make your plots. Plot the histogram of all the four attributes, using 10 bins on four different plots. Can you provide a legend to the plot. Can you merge the four plots into one plot and add a legend.
Draw a line plot for all the sepal length values. Provide appropriate labels to the x and y axis. Can you also plot the sepal width on the same plot. Try to provide appropriate labels to the axis and a legend to the plot. Also try to turn on the grid lines and a title for the plot. (What is your observation at around the 50th flower).
Draw a scatter plot between any two attributes of the data. Try to colour the dots in the scatter plot using the different colours for the different class labels. Can we also vary the size of the dots according to a third attribute from the plot. Maybe we can also vary the transparency of the plot to see the overlaps better.
Write functions to calculate the euclidean, manhattan and cosine distance between two vectors.
If we treat each observation of a flower as a vector in a 4d space can you obtain a symmetric distance matrix containing the euclidean distances between each flower observation. You can use pyplot's matshow command to visualize the plot. What is our interpretation of the plots.
Plot a bar graph showing the mean value of sepal lengths for the three different types of flower types. (Maybe numpy's where command is useful for this. Or are there still easier ways?)
Try to read in the file bezdekIris.data into python using numpy. Why do you think this fails.