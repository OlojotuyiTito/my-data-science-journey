# Day 4 - DS Journey

Remeber how we said Data Science was all about drawing insight from data that translate into answers to questions and data-driven decisions?
And how that to draw insight from data, we have to work/operate on it and those operations are essentially mathematical?

Well, there is a python package that is created specifically for scientific computing and high-volume mathematical operations. The perfect library for us to use.
It's called NumPy and is particularly suited for this kind of work because of its speed and ability to perform the desired mathematical caluations with ease.

Here are some things I learnt on NumPy:
```python
import numpy as np
heights_inches = [2.14, 1.77, 1.75, 2.25, 1.49]
np_heights_inches = np.array(heights_inches) # creating a numpy array from a list
np_heights_meters = np_heights_inches * 0.0254 # converting the heights in inches to meters

# A NumPy array can only be on one type. No mixing.
names = ['tito', 'david', 'teni']

np_names = np.array(names)
values = [4, 5, 10, False, True]
np_values = np.array(values)
print(np_values) # This will output [4, 5, 10, 0, 1], converting the booleans to integers so that the array is of one type

# 2D & Subsetting
list_of_lists = [
    [1.75, 26],
    [2.42, 18],
    [2.22, 32],
    [1.04, 41],
    [2.18, 39],
    [1.18, 76]
]
np_expanded_list = np.array(list_of_lists) # This creates a 2D NumPy array with 6 rows and 2 columns
print(np_expanded_list[3][0]) # or print(np_expanded_list[3, 0]) works exactly the same
print(np_expanded_list[:, 0]) # prints out all the values in the first column


# Some basic summary statistics using NumPy
the_mean_age = np.mean(np_expanded_list[:, 1])
the_median_height = np.median(np_expanded_list[:, 0])
the_standard_deviation_of_ages = np.std(np_expamded_list[:, 1])
the_correlation_between_age_and_height = np.corrcoef(np_expanded_list[:, 0], np_expanded_list[:, 1])
```

That's it for today! Thanks for stickcing around.

We go again tomorrow. To consistency!

- Monday, 21 September 2026
