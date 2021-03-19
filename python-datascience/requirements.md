Install Anaconda, so that you can access Jupyter Notebook
or 
You can login to Colab.research.google.com 

https://www.youtube.com/watch?v=LHBE6Q9XlzI
freeCodeCamp.org course on Python

Data Structures - Slide 
List, Dictionary, Tuple, 
list of same type, heterogenous data type

Numpy - way more faster

import numpy as np
a = np.array([1,2,3,4,], dtype = 'i')a.

b = np.array((2,3,5), dtype ='f')
a.dtype
a.ndim
a = np.array([1,2,3],[4,5,6]])
b.shape[0]

nbytes

np.arange(start, end, increment)
np.rando.permutation
np.reshape
np.zeroes

a = np.arange(100)
[0,1,...99]

slicing 

a[1:5] -- index 1 till 5 but not 5
a[:5]. -- index 0 till 5 but not 5
a[2:] -- index 2 till end including the last element
a[::-1] -- from end till start (reverse the array)
a[::2] -- from start till end eveery other element

a[::2,:] ?


Row
Column
sub matrix

Transpose - A.T
import numpy.linalg as la -- Linear Algebra Library

la.inv (np.random.rand(3,3))

Sorting 

A.sort(axis=0) -- column wise 2 dimensional array
A.sort(axis=1) -- row wise in 2 dimensional array

multi-dimensional array axis can go beyond 2

for one-d


Fancy Indexing (Masking) - Copy of the Array vs View (in case of slicing)
selective picking
a[[1,4,6]] index 1, 4, 6 elements

Boolean Mask - 
a[[True, True, False, False, True, True]]

elements less than 8 - boolean array
a[a<8]

and (single objects), & (arrays)

a[(a<8) & (a>4)]
a[a<8 and a>4]

&, |, ~ and, or, not

Broadcasting 

A = A + 5

Matches the size of the A

Possible with other combinations 

A + (np.arange(2).reshape(2,1))

universal functions


np.hstack
np.vstack
np.sort


b = np.random.rand(100000)
%timeit sum(b)
%timeit np.sum(b)

%%timeit
s=0
for x in b:
  s+=x
  

pandas was built on top of numpy

handle large amount of data 

handle missing entries

read and write CSV, Excel 

Series and DataFrame 

import pandas as pd

data = pd.Series ([1,2,4,53], index=['a','b','c','d'])
data.values 
data.index

print (pd.__version__)

you can create a dictionary and then create a series

explicit index and implicit index
what if the explicit index is also a number


DataFrames:



