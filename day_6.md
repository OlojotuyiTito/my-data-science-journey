# Day 5 - DS Journey

Today I learnt the basics of Dictionaries and Pandas

So up till now we've been using lists and the numpy array to store our data.
But both of those have their limitations in certain areas of application.

Take for example these two lists, countries and their corresponding capitals

```python
countries = ['spain', 'france', 'germany', 'norway']
capitals = ['madrid', 'paris', 'berlin', 'oslo']
```

If I wanted to get the capital of any country, I would have to first get the index of the country and then use that index to select the capital from its list.
Look at what I mean: This is how I'd get the capital of Germany

```python
ger_ind = countries.index('germany')
germany_capital = capitals[ger_ind]
```

This worked, but it isn't very intuitive and convenient.
Wouldn't it be nice if there was a way the country and capitals could just be directly linked together somehow?

Well, that's where the Dictionary data type comes in.
A dictionary stores data in key-value pairs meaning that there is a direct link between them and that makes it easier when it comes to selection, especially for data that doesn't need to be ordered
in any specific way.

Let me show you how the same example I used previously would be implemented using a dictionary

```python
countries_and_caps = {
    'spain': 'madrid',
    'france': 'paris',
    'germany': 'berlin',
    'norway': 'oslo',
}

germany_captial = countries_and_caps['germany']
```

Isn't that beautiful?

You remember that for a NumPy array all the values can only be of one type?
Well, in reality, when we are working with data, it often includes different data types.
For example, if we were dealing with student data, we would expect to see attributes such as: names, matric_number, CGPA, Date of Birth, Gender, course_of_study, is_undergrad, is_postgrad, etc.
So there are different data types here.

So to work on that data in python, we need a way to store it just like a spreadsheet where we can accommodate different data types.

That's where Pandas comes in.
Pandas is a powerful data manipulation tool that was actually built on top of NumPy but gives some greater capabilities we need as data scientists.
The Pandas library offers a data type called the DataFrame that essentially allows us to store data in Python like tables in a spreadsheet.

Enough talk. Let's see:

```python
import pandas as pd

student_data = {
    "names": ["Titoluwanimi Olojotuyi", "Ibukunoluwa James", "Otenaike David", "Adeniyi Oluwajomiloju"],
    "matric_no": ["cs21", "cs53", "cs01," "cs84"],
    "CGPA": [4.85, 4.99, 5.0, 5.4],
    "is_undergrad": [True, True, False, False],
    "age": [18, 21, 99, 102],
}

students = pd.DataFrame(student_data)
print(students)
```

Now we have this data in a tabular format with all the different data types accounted for.

This is a run down of all I specifically learnt on Dictionaries and Pandas

```python
countries_and_caps["Rwanda"] = "Kigali"
print('france' in countries_and_caps) # True
countries_and_caps['france'] = "another random state"
del(countries_and_caps['norway'])

europe = { 'spain': { 'capital':'madrid', 'population':46.77 },
           'france': { 'capital':'paris', 'population':66.03 },
           'germany': { 'capital':'berlin', 'population':80.62 },
           'norway': { 'capital':'oslo', 'population':5.084 } }

pop_of_france = europe['france]['population']

data = {
    'capital': 'rome',
    'population': 59.83
}

# Add data to europe under key 'italy'
europe["italy"] = data

import pandas as pd

# Build cars DataFrame
names = ['United States', 'Australia', 'Japan', 'India', 'Russia', 'Morocco', 'Egypt']
dr =  [True, False, False, False, True, True, True]
cpc = [809, 731, 588, 18, 200, 70, 45]
cars_dict = { 'country':names, 'drives_right':dr, 'cars_per_cap':cpc }
cars = pd.DataFrame(cars_dict)
print(cars)

# Definition of row_labels
row_labels = ['US', 'AUS', 'JPN', 'IN', 'RU', 'MOR', 'EG']

# Specify row labels of cars
cars.index = row_labels

# Print cars again
print(cars)

# Import the cars.csv data: cars
cars = pd.read_csv('cars.csv', index_col=0)

# Print out cars
print(cars)

# Print out country column as Pandas Series
print(cars['country'])

# Print out country column as Pandas DataFrame
print(cars[['country']])

# Print out DataFrame with country and drives_right columns
print(cars[['country', 'drives_right']])

print(cars[0:3])

# Print out fourth, fifth and sixth observation
print(cars[3:6])

# Print out observation for Japan
print(cars.loc["JPN"])

# Print out observations for Australia and Egypt
print(cars.iloc[[1, -1]])

# Print out drives_right value of Morocco
print(cars.loc[['MOR'], 'drives_right'])

# Print sub-DataFrame
print(cars.loc[['RU', 'MOR'], ['country', 'drives_right']])

# Print out drives_right column as Series
print(cars.loc[:, 'drives_right'])

# Print out drives_right column as DataFrame
print(cars.loc[:, ['drives_right']])

# Print out cars_per_cap and drives_right as DataFrame
print(cars.loc[:, ['cars_per_cap', 'drives_right']])
```

That's all for today.
Thanks for sticking around!

We go again tomorrow!

To consistency!

- Wednesday, 23 September 2026
