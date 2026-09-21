# Day 2 - DS Journey

To draw insights from data, one has to work/operate on it.

These operations are essentially mathematical.

And because there is such a large amount of data being generated in the world today, it is impractical for a human to manually process it all. It is simply too much.

So for that reason we use computers to do the processing and operation because they are able to handle large amounts of data without getting tired, needing breaks or making careless errors provided you give them the right instructions.

The right instructions? Yes, we can tell a computer what do like adding two numbers, calculating the average of a set of numbers, computing standard deviation and so on.

We give computers instructions using programming languages.

The most popular programming language used to give computers instructions to perform operations involved in extracting insight from data is Python.

Python was made by Guido van Rossum and is a general purpose programming language that is very close to the human language and very easy to learn and use.

Because it's so easy to use, the community around the Python programming language is so large and there are lots of contributions, improvements and developments being made to it.

The Python community has built so many packages (reusable code that solves a specific problem) including ones for data science too.

That's why we use Python as a primary language used in the practice of Data Science!

These are the little I learnt on using the Python programming language today from the Introduction To Python course on DataCamp:

```python
# Python Basics
print("Hello Python!")
print(1 + 1)
print(2 - 5)
print(3 * 6)
print(6 / 3)

# Variables
my_name = "Titoluwanimi David Olojotuyi" # String
age = 18 # integer
height = 9.33 # float
is_friendly = True # boolean

# Lists
all_types_list = [1.42, 2.31, "him, "1.76, "her", 5.22, True, 3.20, 7.23, 200]

list_of_lists = [
    ["bedroom", 23.4],
    ["living room", 542.2],
    ["poolhouse", 42.5]
]

# Subsetting lists
first_two_elements = all_types_list[:3]
last_three = all_types_list[-3:]
living_room_size = list_of_lists[1][1]

# manipluating_lists
all_types_list[2] = "I'M HIM!!!"
all_types_list + ["bathroom", 4.44]

# Deleting elements from a list
del all_types_list[-1]
del list_of_lists[0:2]

# Copying lists
new_all_types_list = list(all_types_list)
```

Thanks for sticking around.
We go again tomorrow! To consistency!

- Friday, 18 September 2026
