# DataCamp-basics
Python lessons during the [DataCamp](https://app.datacamp.com/learn/courses/intro-to-python-for-data-science) course.

## Calcs

```py
# Addition, subtraction
print(12 + 5)
print(12 - 5)

# Multiplication, division, modulo, and exponentiation
print(8 * 5)
print(16 / 2)
print(32 % 7)
print(4 ** 3)

# Calculate two to the power of five
print(2**5)
```

## Variables and Types

Variable types and how to discover each type is the variable. Note that we create the variable but we don't need to say witch type it is.
```py
# Create a variable savings
savings = 100
type (savings) #returns variable type (int)
print(type(savings)) #prints the type of savings variable

# Create a variable growth_multiplier
growth_multiplier = 1.1  #returns variable type (float)

# Calculate result
result = savings * growth_multiplier ** 7

# Print out result
print(result)

# Create a variable desc
desc1 = "compound interest" #returns variable type (str)
desc2 = 'compound interest' #also works

# Create a variable profitable
profitable = True
type (profitable) #returns variable type (Bool)
```
Converting variable types:

```py
# Definition of savings and result
savings = 100
result = 100 * 1.10 ** 7

# Fix the printout
print("I started with $" + str(savings) + " and now have $" + str(result) + ". Awesome!")

# Definition of pi_string
pi_string = "3.1415926"

# Convert pi_string into float: pi_float
pi_float = float(pi_string)
```
## Python List

The *list* is a compound data type. They work as arrays in C, but I can add different types, or even lists inside lists (sublists).

```py
# area variables (in square meters)
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

# house information as list of lists
house = [["hallway", hall],
         ["kitchen", kit],
         ["living room", liv],
         ["bedroom",bed],
         ["bathroom",bath]]

# Print out house
print (house)

# Print out the type of house
print(type(house))
```

And the output will be: 
```
<script.py> output:
    [['hallway', 11.25], ['kitchen', 18.0], ['living room', 20.0], ['bedroom', 10.75], ['bathroom', 9.5]]
    <class 'list'>
```

## Subsetting lists

* Select a value using an index. It can be positive or negative, depending the value that I want.
* Values starts from [0], but if I want to reach the last value of the *list* I can simply use [-1].
* I can select multiple values by using ```[start:end]``` where for the example [3:5] it returnts the values 3 and 4 (end not included). I can also use [:6] to start from index 0 or even [6:] to go up to the last index.
* To subset lists of lists I must use for example ```x[2][:2]```.
 
## Changing list elements

* Changing value is similar to array in C. Select the index and use the = value, as example ```array[4] = "atualiza valor"```.
* To add values I can use ```array + ["value",value]```.
* To delet a value, I can use ```del(array[4])```.

When you have an array *x = [1,2,3]* and you copy to another variable, such as *y = x*, you are copying the address of the array and not the values. To create a new list with same values it is used ```y = list(x)``` or ```y = x[:]```.
 
## Adding commands at the same line

```py
# Same line
command1; command2

# Separate lines
command1
command2
```
## Functions

To get helo on a function I can use: ```help(len)``` or ```?len```. Next a few examples of Functions:

```py
max(list_name)  # return the maximum number of the list.

round(1.68,1) # to round number to ony one house.

round(1.68) # returns the value of the number of houses after the dot.

len(var1) # returns the length of the variable.

sorted(list_name,reverse=False) # To sort a list, reverse=False = ascending order.


```
## Methods

Methods: function that belong to objects. Python is object-oriented, but not only.
Python is a structured, object-oriented and functional programming language.

```py
list_name.index("example") # Call method index () on list_name
list_name.count("example") # Shows how many times "example" appears on the list_name
list_name.reverse() # Reverses the order of the elements in the list
list_name.remove() # Removes the first element of a list that matches the input
```

Other examples: 

```py
word = 'word'
word.capitalize() # Returns 'Word'
word.replace("r","rl") # Returns 'World'
word.upper() # Returns WORLD

```

Instead of ```list_name + "me"``` I can ```list_name.append("me")```.

## Packages

Packages are directories of Python Scripts, it specifies functions, methods and types for particular problemns. Examples are NumPy and Matplotlib.
First it is needed to install on the system by using the pip. To install pip using the terminal use ```get-pip.py```, then ```python3 get-pip.py``` and then the package, ```pip3 install numpy```. The examples are for Python version 3.
On Python code, we need to import this, by using ```import numpy```.
Also, I can do:

```py
import numpy
numpy.array([1, 2, 3])
```
or 
```py
import numpy as np # Preferred
np.array([1, 2, 3])
```
or 
```py
import numpy as array
array([1, 2, 3]) # Directly uses the array from numpy package
```
I can ```import math``` to use the pi value by ```math.pi```. If only the pi is used from that package, I can be more selective by ```from math import pi```.

I can also import only a subpackage, such as ```import scipy.linalg```.
