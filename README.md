# Graph-Plotting

This series will introduce you to graphing in python with Matplotlib, which is arguably the most popular graphing and data visualization library for Python.

Installation

Easiest way to install matplotlib is to use pip. Type following command in terminal:

pip install matplotlib

Customization of Plots

![image](https://user-images.githubusercontent.com/22562694/120806767-dec84380-c564-11eb-9d04-5d616d3559ab.png)

As you can see, we have done several customizations like

setting the line-width, line-style, line-color.
setting the marker, marker’s face color, marker’s size.
overriding the x and y axis range. If overriding is not done, pyplot module uses auto-scale feature to set the axis range and scale.
 
Bar Chart

Here, we use plt.bar() function to plot a bar chart.

![image](https://user-images.githubusercontent.com/22562694/120807057-2c44b080-c565-11eb-8078-8cf2f1382bf9.png)

x-coordinates of left side of bars are passed along with heights of bars.

you can also give some name to x-axis coordinates by defining tick_labels

Histogram

Here, we use plt.hist() function to plot a histogram.

![image](https://user-images.githubusercontent.com/22562694/120807096-35358200-c565-11eb-953a-ff633b20bc4e.png)

frequencies are passed as the ages list.
Range could be set by defining a tuple containing min and max value.
Next step is to “bin” the range of values—that is, divide the entire range of values into a series of intervals—and then count how many values fall into each interval. Here we have defined bins = 10. So, there are a total of 100/10 = 10 intervals.

Scatter Plot

![image](https://user-images.githubusercontent.com/22562694/120807191-4d0d0600-c565-11eb-9c30-f44ee913629a.png)

Here, we use plt.scatter() function to plot a scatter plot.
Like a line, we define x and corresponding y – axis values here as well.
marker argument is used to set the character to use as marker. Its size can be defined using s parameter.

Pie Chart

Here, we plot a pie chart by using plt.pie() method.

![image](https://user-images.githubusercontent.com/22562694/120807314-72017900-c565-11eb-8a9c-64e90051a9a7.png)

First of all, we define the labels using a list called activities.
Then, portion of each label can be defined using another list called slices.
Color for each label is defined using a list called colors.
shadow = True will show a shadow beneath each label in pie-chart.
startangle rotates the start of the pie chart by given degrees counterclockwise from the x-axis.
explode is used to set the fraction of radius with which we offset each wedge.
autopct is used to format the value of each label. Here, we have set it to show the percentage value only upto 1 decimal place.

Plotting curves of given equation

![image](https://user-images.githubusercontent.com/22562694/120807430-8f364780-c565-11eb-9b95-dd96be28e355.png)

Here, we use NumPy which is a general-purpose array-processing package in python.

To set the x – axis values, we use np.arange() method in which first two arguments are for range and third one for step-wise increment. The result is a numpy array.
To get corresponding y-axis values, we simply use predefined np.sin() method on the numpy array.
Finally, we plot the points by passing x and y arrays to the plt.plot() function.

So, in this repository, I have discussed various types of plots we can create in matplotlib. 
