# Hints for Exercise 8
## Contents
- [General hints for Exercise 8](#general-hints)
- [Problem 1 hints](#problem-1)
- [Problem 2 hints](#problem-2)

## General hints
### Sigma notation
***Sigma notation*** is used to indicate values that should be added together or summed.
It is a shorthand notation to indicate the sum of *N* values, where each value in the set can be represented by the subscript *i*.
The example below shows how *sigma notation* works.

![Sigma notation](../Images/sigma-notation.png)<br/>
*Equation H1. Sigma notation indicating the sum of N values, each indicated by x*.

As you can see, the complete form explicitly states the starting and ending values for the sum (*i* = 1 and *N*), but often these values are not written as it can be assumed that all *N* values will be summed.

## Problem 1


## Problem 2
### Example plot for Problem 2
Below is an example of the type of plot you should produce for Problem 2.

![Gaussian plot for Problem 2](../Images/Gaussian-plot.png)

### Creating arrays of numbers between two values
As you may recall from [Lesson 6](https://github.com/Python-for-geo-people/Lesson-6-Intro-to-NumPy/blob/master/Lesson/intro-to-numpy.md#functions), we can use NumPy to create NumPy arrays of values between a starting and ending value.
Consider the simple example below using the `np.linspace()` method:

```python
>>> import numpy as np
>>> numberArray = np.linspace(0.0, 1.0, 11)
>>> print(numberArray)
[ 0.   0.1  0.2  0.3  0.4  0.5  0.6  0.7  0.8  0.9  1. ]
```
Here you can see we start with `0.0`, end with `1.0`, and produce an array of `11` equally spaced values that includes the starting and ending numbers.
This is probably the easiest way to create most arrays of this kind.

### Creating and appending to lists
This is mostly a reminder of something we had seen [back in Lesson 2](https://github.com/Python-for-geo-people/Diving-into-Python/blob/master/Lesson/python-basic-elements1.md#lists-and-indices).
When you are calculating the values for the normal distribution, one option is to create an empty list and append the calculated values to the list, calculating one value for each age in an age list/array from 0-10 Ma by 0.1 Ma.
You can see an example below, which assumes you have created the NumPy array `numberArray` as shown the previous hint:

```python
>>> dummyList = []
>>> for i in range(len(numberArray)):
...     dummyList.append(numberArray[i]**2.0)
...
>>> print(dummyList)   # I have rounded the values below to fit better on the screen
[0.0, 0.01, 0.04, 0.09, 0.16, 0.25, 0.36, 0.49, 0.64, 0.81, 1.0]
```
As you can see, `dummyList` ends up with the same number of values as `numberArray` (see previous hint), with one calculated value in `dummyList` for each corresponding value in `numberArray`.
