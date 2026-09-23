# Day 5 - DS Journey

Today I went into a bit of introduction of Data Visualization.

Like I've said many times before, Data Science is all about extracting/discovring insights from data that will help us make better informed decisions.

To draw insights from your data, you need to have an understanding of all it contains.

And the best way we, as humans, understand our data better seeing it visually.

You've probably heard "A picture is worth a thousand words". And that can't be more true in data science.

And that's the whole ides behind data visualization.

There are complex information/insights in data that really can't be fully grasped by just looking at the numbers from your spreadsheet or csv file.

But often times they become even surprisingly obvious when visualised properly.

The Mother of visualization packages in Python is __Matplotlib__.

The sub-package in it, Pyplot, is especially useful for creating visualisations such as line plot, histograms, scatter plots and so on.

Here's the overview of what I learned today:
```python
import matplotlib.pyplot as plt

plt.plot(year, pop) # line plots
plt.scatter(year, pop) # scatter plots
plt.hist(life_exp, 5) # histogram

plt.xlabel("GDP per Capita")
plt.ylabel("Life Expectancy")

plt.xscale('log')

plt.yticks([0, 2, 4, 6, 8, 10], ["0B", "2B", "4B", "6B", "8B", "10B"])
plt.xticks([1000, 10000, 100000], ["1K", "10K", "100K"])

plt.title("The title of the visualisation")
plt.grid(True)
```

A line plot is particularly useful for visualizations where the x-axis is time-series data.

Scatter plots are particularly useful to visualize the correlation between two data values.

Histograms are particularly useful for checking the distribution of data across various intervals.

Thanks for sticking around!
We go again tomorrow!

To consistency!

- Tuesday, 22 September 2026
