# Day 3 - DS Journey

Today I continued learning about python and its uses in Data Science.
I learnt about functions, methods and packages

```python
'''
Functions are blocks of reusable code that solve a perform a
particular task. Take a look at some examples:
'''
var1 = [1, 2, 3, 4]
var2 = True

print(len(var1))
print(type(var2))
print(int(var2))

help(pow) # help() is the function to find the documentation of a function
sorted(var1, reverse=True)

'''
Methods are functions that operate on specific objects in Python
Here are some examples of methods
'''
my_name = "Titoluwanimi David Olojotuyi"
my_name.upper()
my_name.replace("David", "Defidi")
print(my_name)

print(my_name.count("o"))
var1.reverse()
print(var1)

'''
For code to be organized properly and easily maintainable,
we split them into packages.
A package is basically a folder of python scripts
that contain the code for certain methods and functions that
solve specific problems.
Here are some examples of using packages
'''
import numpy as np
ages = [44, 14, 72, 31, 90, 43, 18, 9]
np_ages = np.array(ages) # converts the list to a numpy array

import math
circle_area = math.pi * 3**2
```

That's it for today.
Thanks for sticking around💖

We go again tomorrow! To consistency!
