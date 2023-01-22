# numpy CheatSheet

numpy uses ndarray struct to store elements of same data types in a fast manner.

## Creation

> array: Convert an already provided python list or tuple to ndarray
> ones: Create an ndarray filled with 1's to specified size and shape
> zeroes: Create an ndarray with 0's to size and shape
> empty: Create with garbage values or empty cells almost same as zeroes
> full: Fill with value specified

## Data types

numpy habits many data types, in the back end they are treated accordingly.
Don't really need deep knowledge, but sometimes a table is useful when needed.

## Indexing Slicing

numpy supports standard list indexing `list[i]` and slicing `list[i:j]`
By dimensions, we can list the dimension we want to slice by passing them in separated by commas.

## Boolean indexing

We can work on arrays with boolean operators which produces us a new boolean array

`data[oherdata > 5]` gives an array of elements of data where at the same index `otherdata` has a value greater than 5.

## Arithmetic operators on arrays

There are also many provided functions with arrays to compute fast, faster than the user's python approach

**Unary:**
> abs
> sqrt
> square
> exp
> log10
> modf

**Binary:**
> add
> substract
> multiply: sequentially not dot product
> divide
> power
> maximum

## Logic with arrays

_where_ function takes (condition, trueval, falseval)

replaces the occurences in the array of the condition 'true' with trueval and so on.

## Stats
> sum: sum all elements
> mean
> std
> min, max
> argmin, argmax: index of min,max
> cumsum: cumulative sum where ith is sum of all elements before i and i
> cumprod: same as cumsum but multiplied, if zero all zero

## Boolean methods

> any: true if any element is true
> all: true if any element is true

It is possible to derieve the counter parts for false.

## Sort

`array.sort()` sorts the array in-place

