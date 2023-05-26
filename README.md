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
